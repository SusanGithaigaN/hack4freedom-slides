<script setup>
import { computed, onUnmounted, ref } from 'vue'
const remaining = ref(600)
const running = ref(false)
let interval
let deadline = 0
const clock = computed(() => `${Math.floor(remaining.value / 60)}:${String(remaining.value % 60).padStart(2, '0')}`)
function pause() { running.value = false; clearInterval(interval) }
function toggle() {
  if (running.value) return pause()
  if (!remaining.value) remaining.value = 600
  deadline = Date.now() + remaining.value * 1000
  running.value = true
  interval = setInterval(() => {
    remaining.value = Math.max(0, Math.ceil((deadline - Date.now()) / 1000))
    if (!remaining.value) pause()
  }, 250)
}
function reset() { pause(); remaining.value = 600 }
onUnmounted(pause)
</script>

<template>
  <div class="activity-timer" @click.stop @keydown.stop>
    <div class="timer-label">YOUR TURN</div>
    <div class="timer-clock" role="timer" aria-label="Time remaining">{{ clock }}</div>
    <p class="timer-message" aria-live="polite">{{ remaining === 0 ? 'Time to share your question.' : 'One project. One opportunity.' }}</p>
    <div class="timer-controls">
      <button type="button" @click="toggle">{{ running ? 'Pause' : remaining === 600 ? 'Start 10 minutes' : remaining === 0 ? 'Start again' : 'Resume' }}</button>
      <button class="secondary" type="button" @click="reset">Reset</button>
    </div>
  </div>
</template>

<style scoped>
.activity-timer { padding: 22px; background: #fff0dc; border: 1px solid #e4b678; border-radius: 18px; text-align: center; }
.timer-label { color: #9a4700; font-size: 17px; font-weight: 750; letter-spacing: 2px; }
.timer-clock { color: #242424; font-size: 76px; font-weight: 750; line-height: 1.2; margin: 10px 0; font-variant-numeric: tabular-nums; letter-spacing: -3px; }
.timer-message { font-size: 20px !important; margin-bottom: 22px !important; }
.timer-controls { display: flex; gap: 10px; justify-content: center; }
button { border: 1px solid #ab5b00; background: #f7931a; color: #242424; border-radius: 8px; padding: 10px 14px; font-size: 18px; font-weight: 700; cursor: pointer; }
button.secondary { background: #fffdf9; border-color: #c7b69e; }
</style>