<script setup>
import { ref } from 'vue'
const items = [
  'I read the contribution guidelines.',
  'I searched for related issues and pull requests.',
  'I confirmed that the task is available.',
  'I understand the change I am making.',
  'I kept the change small and focused.',
  'I ran the relevant tests and checks.',
  'I wrote a clear pull request description.',
  'I am ready to receive and respond to feedback.',
]
const checked = ref([])
</script>

<template>
  <div @click.stop @keydown.stop>
    <div class="pr-checklist">
      <label v-for="(item, index) in items" :key="item" :class="{ complete: checked.includes(index) }">
        <input v-model="checked" type="checkbox" :value="index">
        <span>{{ item }}</span>
      </label>
    </div>
    <p class="checklist-count" aria-live="polite">{{ checked.length }} / 8 ready <span>•</span> A useful contribution starts with care.</p>
  </div>
</template>

<style scoped>
.pr-checklist { display: grid; grid-template-columns: 1fr 1fr; grid-auto-flow: column; grid-template-rows: repeat(4, auto); gap: 14px 34px; }
label { display: flex; gap: 15px; align-items: center; padding: 12px 19px; border: 1px solid #dedbd5; border-radius: 12px; background: #fff; font-size: 25px; line-height: 1.3; cursor: pointer; min-height: 80px; }
label.complete { border-color: #d8892c; background: #fff0dc; }
input { flex-shrink: 0; width: 25px; height: 25px; accent-color: #9a4700; cursor: pointer; }
input:focus-visible { outline: 3px solid #9a4700; outline-offset: 4px; }
.checklist-count { font-size: 21px !important; margin-top: 16px !important; color: #5d6065; }
.checklist-count span { margin: 0 12px; color: #9a4700; }
</style>
