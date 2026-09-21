---
theme: default
title: 'Making your first Bitcoin open-source contribution'
info: 'Hack4Freedom · A practical contribution journey, grounded in personal experience.'
class: h4f cover
colorSchema: light
canvasWidth: 1200
aspectRatio: 16/9
fonts:
  sans: Segoe UI
  mono: DejaVu Sans Mono
  provider: none
duration: 30min
transition: fade
drawings:
  persist: false
---

<div class="cover-mark"><span class="bitcoin-mak" aria-label="Bitcoin"></span> Hack4Freedom</div>
<div class="cover-grid">
<div>

# Making your first<br><span class="orange-word">Bitcoin</span> open-source<br>contribution

<p class="lead">A practical path from “where do I start?”<br>to a useful first pull request.</p>
</div>
<!-- <div class="cover-path" aria-label="Contribution journey: find your fit, learn the project, make a change, share for review">
<p><carbon:search /> Find your fit</p>
<span class="path-arrow">↓</span>
<p><carbon:events /> Learn the project</p>
<span class="path-arrow">↓</span>
<p><carbon:code /> Make a change</p>
<span class="path-arrow">↓</span>
<p class="last"><carbon:pull-request /> Share for review</p>
</div> -->
</div>

<!--
1 minute. This talk follows my process: start with familiar skills, shortlist about three projects, learn how people work together, and then choose a useful task. No purchase of bitcoin is needed. Ask who has used GitHub but has not opened a PR yet. We will reserve five minutes to find a real opportunity.
Visual attribution: IBM Carbon icons, Apache-2.0, https://github.com/carbon-design-system/carbon/tree/main/packages/icons
All repository, issue and PR mockups in this deck are original teaching examples, not screenshots of live projects. Bitcoin mark is typeset text.
-->

---
class: h4f
---

<div class="eyebrow">01 / Your starting point</div>

# Start with skills you already have

<div class="split">
<div>
<p class="lead">Which language or technology<br>can you work with today?</p>
<div class="tags"><span class="tag orange">Python</span><span class="tag orange">JavaScript / TypeScript</span><span class="tag orange">Ruby on Rails</span><span class="tag orange">Rust</span><span class="tag orange">C++</span><span class="tag orange">C#</span></div>
<br/><br/>
<p class="small muted">These are just examples, not prerequisites. Writing, testing and design are useful skills too.</p>
</div>
<div class="card orange" v-click>
<carbon:code class="icon" />
<h2>Familiar tools help</h2>
<p>Spend your energy learning the codebase and contribution process.</p>
<p class="small">You can learn another language later.</p>
</div>
</div>
<!-- <div class="callout"><strong>Quick show of hands:</strong> code, documentation, testing or design?</div> -->

<!--
1 minute. Personal experience supplied by the speaker: I first identify the programming languages I am comfortable using. Invite attendees to name one skill. The language examples are illustrative; don't imply that every project uses these stacks. Non-code contributions are valid too.
-->

---
class: h4f
---

<div class="eyebrow">02 / Discovery</div>

# Find projects that interest you

<div class="split wide-left">
<div>
<p class="lead">Start with the Bitcoin developer<br>project directory.</p>
<p><a href="https://bitcoindevs.xyz/contribute" target="_blank" rel="noopener noreferrer">bitcoindevs.xyz/contribute ↗</a></p>
<div class="personal"><small>My approach</small>“I shortlist about three projects<br>that fit my skills and interests.”</div>
<p class="small muted">Open each project's own repository to verify its current needs.</p>
</div>
<div class="mock">
<div class="mock-bar"><carbon:search /> Your discovery notes</div>
<div class="mock-body stack">
<p><strong>Project A</strong><br><span class="small muted">A purpose I care about</span></p>
<p><strong>Project B</strong><br><span class="small muted">A stack I can work with</span></p>
<p><strong>Project C</strong><br><span class="small muted">A community I can learn from</span></p>
</div>
</div>
</div>

<!--
1 minute. Open the directory link if there is time; use the project search and repository links available on the site. The notes visual is a blank shortlist, not the directory's interface or a recommendation of specific projects. The directory returned HTTP 200 during preparation; individual listings and available issues can change.
Source: https://bitcoindevs.xyz/contribute
-->

---
class: h4f
---

<div class="eyebrow">02 / Narrow your shortlist</div>

# Compare the three projects

<table class="comparison">
<thead><tr><th>Look at</th><th>Ask yourself</th></tr></thead>
<tbody>
<tr><td>Language &amp; stack</td><td>Can I understand and run a small part?</td></tr>
<tr><td>Purpose</td><td>Do I care about the problem it solves?</td></tr>
<tr><td>Activity</td><td>Are issues answered and PRs reviewed?</td></tr>
<tr><td>Documentation</td><td>Can I follow the setup and contribution guide?</td></tr>
<tr><td>Community</td><td>Where can I ask a useful question?</td></tr>
<tr><td>First tasks</td><td>Is there something small I can verify?</td></tr>
</tbody>
</table>

<!--
1 minute. Use this as a comparison worksheet for all three projects; there is no universal numeric score. Review dates and the quality of responses, not just stars. A quiet week alone does not prove that a project is inactive. Start with the project where you can explain a useful next step.
Source: https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github
-->

---
class: h4f
---

<div class="eyebrow">03 / Repository scanning</div>

# Read the guide before the code

<div class="split repository-diagram">
<div class="mock">
<div class="mock-bar"><carbon:logo-github /> example / bitcoin-project</div>
<div class="file-row"><carbon:document /><code>README.md</code><span>Purpose &amp; setup</span></div>
<div class="file-row active"><carbon:document-tasks /><code>CONTRIBUTING.md</code></div>
<div class="file-row"><carbon:document /><code>LICENSE</code><span>Reuse terms</span></div>
<div class="file-row"><carbon:folder /><code>src/</code><span>Implementation</span></div>
<div class="file-row"><carbon:folder /><code>tests/</code><span>Expected behavior</span></div>
<div class="file-row"><carbon:folder /><code>docs/</code><span>Guides</span></div>
</div>
<div class="mock" v-click>
<div class="mock-bar"><carbon:document-tasks /> CONTRIBUTING.md</div>
<div class="mock-body doc-lines">
<div class="doc-heading">How to contribute</div>
<p><strong>Before starting</strong><br>Discuss the scope and read our policies.</p>
<p><strong>Local checks</strong><br>Follow our setup, formatting and tests.</p>
<p><strong>Submitting</strong><br>Use our PR template and commit style.</p>
</div>
</div>
</div>
<p class="caption">Illustrative repository and guide. File names and rules vary by project.</p>

<!--
1.5 minutes. A repository is the project's files plus history. Reveal the guide and explain that it is a simplified example, not a quotation. Some projects host contribution guidance on a website instead. Check the license, code of conduct and AI policy too. Read the actual setup instructions rather than guessing commands from this example.
Source: https://opensource.guide/how-to-contribute/
-->

---
class: h4f
---

<div class="eyebrow">03 / Project checklist</div>

# Understand how the project works

<div class="split">
<div>
<h2><carbon:folder /> Explore the work</h2>
<ul class="checklist">
<li>Read the README and guidelines.</li>
<li>Explore folders and nearby code.</li>
<li>Review recently merged PRs.</li>
<li>Read open <strong>and closed</strong> issues.</li>
</ul>
</div>
<div>
<h2><carbon:events /> Meet the community</h2>
<ul class="checklist">
<li>Notice how maintainers give feedback.</li>
<li>Find the public communication channel.</li>
<li>Join the chat, forum or mailing list.</li>
<li>Read recent discussions before posting.</li>
</ul>
</div>
</div>
<div class="callout"><strong>Look for context:</strong> what has already been tried, accepted or put on hold?</div>

<!--
1 minute. Merged PRs show what a completed contribution looks like. Closed issues and PRs may explain why an idea is unsuitable. Use the public channel linked from the repository or official project site; it might be IRC, Discord, Slack, a forum or a mailing list. You do not need to understand the entire repository before asking a focused question.
-->

---
class: h4f
---

<div class="eyebrow">04 / Learn through the community</div>

# Join a dev call, if the project holds one

<div class="split">
<div>
<div class="personal"><small>In my experience</small>“Calls help me understand the priorities and contribution process before I open a PR.”</div>
<p class="small">Listen for open PRs, proposed features,<br>technical challenges and unclaimed work.</p>
<p class="small muted">No calls? Use the project's public discussions.</p>
</div>
<div class="card orange">
<h2>Your first conversation</h2>
<ul class="checklist">
<li>Listen and take notes.</li>
<li>Introduce yourself briefly.</li>
<li>Ask where help is useful.</li>
<li>Check who is already working on it.</li>
</ul>
</div>
</div>
<p class="caption">It is fine to listen on your first visit. <a href="https://bitcoincore.reviews/" target="_blank" rel="noopener noreferrer">Bitcoin Core PR Review Club ↗</a> is an example of learning through public IRC discussion.</p>

<!--
1.5 minutes. The personal experience comes from the speaker's supplied process. Calls can surface missing work before it has an issue. Ask relevant questions without feeling you must speak at length. Not all projects have calls, and not all meetings are voice or video: the Bitcoin Core PR Review Club is an IRC learning space. Check its site for current meeting details; do not infer a schedule from this slide.
Source: https://bitcoincore.reviews/
-->

---
class: h4f section
transition: slide-left
---

<div class="eyebrow">Choose your first task</div>
<div class="section-index">1 task → 1 PR</div>

# One useful problem.<br>A small, understood change.

<p class="lead">Your first contribution can be a PR review,<br>a test, or a bug someone else can reproduce.</p>

<!--
30 seconds. Transition from finding a community to finding useful work. This is a framing principle, not a promise of a merge. Ask: what would make a task small enough to explain and verify?
-->

---
class: h4f
---

<div class="eyebrow">05 / Find an issue</div>

# Labels are a starting point

<div class="split wide-left">
<div class="mock">
<div class="mock-bar"><carbon:logo-github /> Issues · teaching example</div>
<div class="mock-body">
<div class="search-line">is:issue is:open label:"good first issue"</div>
<span class="status">○ Open</span>
<div class="issue-title">Clarify the setup error message</div>
<div class="tags"><span class="tag">good first issue</span><span class="tag neutral">documentation</span></div>
<p class="small muted">Read the description, comments and linked work.</p>
</div>
</div>
<div>
<p>Also look for:</p>
<div class="tags"><span class="tag">beginner friendly</span><span class="tag">help wanted</span><span class="tag neutral">tests</span></div>
<div class="callout" v-click><strong>Before you start</strong><br>Is anyone already working on it?<br>Is your approach welcome?</div>
</div>
</div>
<p class="caption">Labels vary. “Help wanted” does not necessarily mean easy.</p>

<!--
1 minute. The issue is an original mockup, not a real available task. Use this filter inside a chosen repository. Read the entire discussion and check linked PRs as well as assignees: an empty assignee field is not proof that work is free. If unclear, leave a brief comment asking if the issue is available and explain your proposed approach.
Source: https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github
-->

---
class: h4f
---

<div class="eyebrow">05 / Small contributions</div>

# Useful work comes in many sizes

<div class="split">
<div class="stack">
<p><strong><carbon:document /> Documentation</strong><br><span class="small">Explain a missing step or outdated instruction.</span></p>
<p><strong><carbon:test-tool /> Tests &amp; bug reports</strong><br><span class="small">Add coverage or reproduce a bug clearly.</span></p>
<p><strong><carbon:accessibility /> Accessibility &amp; UI</strong><br><span class="small">Improve keyboard use or a confusing label.</span></p>
</div>
<div class="stack">
<p><strong><carbon:code /> Small fixes</strong><br><span class="small">Correct a focused bug or error message.</span></p>
<p><strong><carbon:document /> Translation</strong><br><span class="small">Follow the project's translation process.</span></p>
<p><strong><carbon:renew /> Outdated code</strong><br><span class="small">Discuss cleanup first</span></p>
</div>
</div>
<div class="callout"><strong>Choose something you can explain and check.</strong> A major feature can wait.</div>

<!--
1 minute. Reuse the earlier deck's point that contributions extend beyond code. A bug report should include steps, expected and actual results, and environment details. Cleanup is not universally suitable for beginners: Bitcoin Core explicitly discourages refactoring PRs from new contributors. Follow each project's guidance. Core translations also use a separate workflow.
Sources: https://bitcoincore.org/en/contribute/ and https://docs.btcpayserver.org/Contribute/ and https://github.com/bitcoin/bitcoin/blob/master/CONTRIBUTING.md
-->

---
class: h4f
---

<div class="eyebrow">06 / Research before coding</div>

# Confirm the context and the approach

<div class="split">
<div>
<h2><carbon:search /> Search the repository</h2>
<ul>
<li>Related issues and earlier PRs</li>
<li>Design discussions and decisions</li>
<li>Similar code already in the project</li>
</ul>
<p class="small muted">Include closed work. Search the public chat or meeting notes too.</p>
</div>
<div class="mock" v-click>
<div class="mock-bar"><carbon:chat /> Example issue comment</div>
<div class="mock-body">
<p>“I'd like to work on this. I found the earlier discussion about the setup error.</p>
<p>Is this still available? Would clarifying the message and adding a test fit the intended approach?”</p>
</div>
</div>
</div>
<div class="callout">Check for duplicate work, paused proposals and decisions you may have missed.</div>

<!--
1.5 minutes. This reflects my habit of researching before committing to work. Search exact error strings, relevant symbols and synonyms. Check whether someone has already volunteered. The comment is a fictional example, not a message to send unchanged. Do not claim to have read a discussion you haven't read. Significant or unclear work merits explicit discussion before coding.
-->

---
class: h4f
---

<div class="eyebrow">06 / AI as a research assistant</div>

# Ask for evidence you can verify

<div class="split wide-left">
<div class="card orange">
<h2>A prompt I would use</h2>
<p class="small">“I want to work on <strong>[task]</strong> in <strong>[public repo]</strong>. Find related issues, earlier PRs and design discussions. Link the evidence and dates.</p>
<p class="small">What should I ask a maintainer before starting? Separate confirmed facts from assumptions.”</p>
</div>
<div>
<ul class="checklist small">
<li>Open every cited link and check its date.</li>
<li>Verify current status in the project.</li>
<li>Keep secrets, credentials and private code out.</li>
<li>Follow the project's AI policy.</li>
<li>Understand every change you submit.</li>
</ul>
</div>
</div>
<div class="callout"><strong>ChatGPT or Claude can help you research.</strong> Maintainers confirm project direction.</div>

<!--
1.5 minutes. Personal practice: ask an AI assistant for references and advice because a newcomer may miss context. AI can help with search terms, code explanations, summaries and questions, but it may lack browsing or invent references. It does not know the current task status by default. Use only public, non-sensitive material and read the actual repository policy before using AI for a contribution. This prompt is a research aid, not a product-specific feature claim.
Source for one project's policy requirements: https://github.com/bitcoin/bitcoin/blob/master/CONTRIBUTING.md
-->

---
class: h4f section
transition: slide-left
---

<div class="eyebrow">07 / Work on the issue</div>

# Make one focused change

<p class="lead">Once the task and approach are appropriate:</p>
<div class="flow" aria-label="Local contribution workflow">
<div class="node"><carbon:branch /><strong>Fork / clone</strong>Follow the project setup.</div>
<span class="arrow">→</span>
<div class="node" v-click><carbon:code /><strong>Branch &amp; edit</strong>Fix the agreed problem.</div>
<span class="arrow" v-after>→</span>
<div class="node" v-after><carbon:test-tool /><strong>Test &amp; commit</strong>Check and record the change.</div>
<span class="arrow" v-after>→</span>
<div class="node" v-click><carbon:pull-request /><strong>Push &amp; propose</strong>Open a PR for review.</div>
</div>
<p class="caption">A pull request proposes your changes to the original project.</p>

<!--
1 minute. Explain the diagram: a fork is your hosted copy; clone downloads files and history; a branch isolates a task; a commit records work; push uploads commits. Follow the repository workflow—some contributors can branch directly and do not need a fork. Reveal in two steps. Keep the smallest useful change and follow coding conventions. The project chooses the target branch.
-->

---
class: h4f
---

<div class="eyebrow">07 / Check your work locally</div>

# Verify the change before sharing it

<div class="split">
<div>
<ul class="checklist">
<li>Follow the coding conventions.</li>
<li>Add or update relevant tests.</li>
<li>Run formatting and lint checks.</li>
<li>Run the relevant test commands.</li>
<li>Update affected documentation.</li>
</ul>
</div>
<div class="card orange">
<carbon:test-tool class="icon" />
<h2>What proves it works?</h2>
<p>For a bug fix, show the failing behavior and verify the correction.</p>
<p class="small">For docs or UI, walk through the instructions or interaction yourself.</p>
</div>
</div>
<p class="caption">Use commands from the project guide. Report limitations honestly.</p>

<!--
1 minute. Meaningful tests depend on the change. Keep formatting and unrelated cleanup out of the patch. Document the commands and results for the PR. For a manual check, record the environment and steps. Do not imply checks passed if you could not run them; state why and ask what additional verification is needed.
-->

---
class: h4f pr-example
---

<div class="eyebrow">08 / Open the pull request</div>

# Make your PR easy to review

<div class="split wide-left">
<div class="mock">
<div class="mock-bar"><carbon:pull-request /> Pull request · teaching example</div>
<div class="mock-body">
<div class="issue-title">Clarify the missing-config error</div>
<dl class="pr-details">
<dt>Why</dt><dd>New users cannot tell which file is missing.</dd>
<dt>Change</dt><dd>Name the file and link the setup instructions.</dd>
<dt>Related</dt><dd>Link the issue and earlier discussion.</dd>
<dt>Checked</dt><dd>Describe tests, commands and results.</dd>
<dt>Open point</dt><dd>Ask about wording that needs input.</dd>
</dl>
</div>
</div>
<div class="stack">
<p><strong>Use the PR template.</strong><br><span class="small">Explain what changed and why.</span></p>
<p><strong>Show visual changes.</strong><br><span class="small">Include before-and-after screenshots.</span></p>
<p><strong>State limitations.</strong><br><span class="small">Flag decisions that need input.</span></p>
<p><strong>Keep it focused.</strong><br><span class="small">Separate unrelated changes.</span></p>
</div>
</div>

<!--
1.5 minutes. Reuse the previous deck's problem, change, verification and context structure. This is a schematic PR description, not a completed upstream PR or evidence of real test results. Replace prompts with what you actually did. A clear title names the affected behavior; use any required project title prefix.
-->

---
class: h4f
---

<div class="eyebrow">09 / Review feedback</div>

# Check both automation and people

<div class="split">
<div class="card">
<carbon:test-tool class="icon" />
<h2>Automated checks</h2>
<ul class="small">
<li>Tests and GitHub Actions</li>
<li>Linters and security checks</li>
<li>AI review, if the project uses it</li>
</ul>
<p class="small muted">Examples include CodeRabbit, Copilot or Claude-based reviewers.</p>
</div>
<div class="card orange" v-click>
<carbon:events class="icon" />
<h2>Human review</h2>
<ul class="small">
<li>Correctness and design</li>
<li>Fit with project priorities</li>
<li>Maintainability and edge cases</li>
</ul>
<p class="small"><strong>Automated feedback does not replace maintainer review.</strong></p>
</div>
</div>
<p class="caption">Tools and their order vary. GitHub Actions is workflow automation, not inherently an AI reviewer.</p>

<!--
1 minute. The tool examples are from the speaker's supplied brief, not a claim that most Bitcoin projects use them. Look at the repository's actual checks and bot identities. Read failures and suggestions; do not blindly accept an automated suggestion. Maintainers may comment before, during or after checks complete.
-->

---
class: h4f
---

<div class="eyebrow">09 / Respond to feedback</div>

# Show what you changed and checked

<div class="review">
<div class="mock">
<div class="mock-bar"><carbon:chat /> Before · reviewer asks</div>
<div class="mock-body"><blockquote>“What happens when the config file is missing? Please cover that case.”</blockquote><p class="caption">A specific request for evidence</p></div>
</div>
<carbon:arrow-right class="review-arrow" />
<div class="mock" v-click>
<div class="mock-bar"><carbon:checkmark-outline /> After · author responds</div>
<div class="mock-body"><blockquote>“Added the missing-file test and reran the relevant suite. The error now names the file.”</blockquote><p class="caption">Example only: report your actual checks</p></div>
</div>
</div>
<p class="small" style="margin-top:24px">Ask if unclear. Explain disagreements respectfully. Resolve addressed threads, then request another review.</p>
<div class="callout"><strong>Commit history:</strong> squash only when the guide or maintainer asks. Follow the project's Git practices.</div>

<!--
1.5 minutes. Reveal the response after asking the audience what useful evidence would look like. Update the existing PR rather than opening a duplicate. Do not resolve a thread before addressing it. If you disagree, explain the tradeoff and ask for clarification. Squashing all commits into one is not a universal rule.
Source for an example of conditional squashing and review: https://github.com/bitcoin/bitcoin/blob/master/CONTRIBUTING.md
-->

---
class: h4f
---

<div class="eyebrow">10 / Stay involved</div>

# Give review time. Keep learning.

<div class="split">
<div>
<p class="lead">Maintainers may be volunteers<br>with limited time.</p>
<p>A slow response does not necessarily mean your contribution was rejected.</p>
<div class="personal"><small>A polite follow-up</small>“I've addressed the feedback. Is there anything else I can clarify before another review?”</div>
</div>
<div class="card orange">
<carbon:time class="icon" />
<h2>While you wait</h2>
<ul>
<li>Follow project discussions.</li>
<li>Test another contributor's change.</li>
<li>Review a guide or help a newcomer.</li>
</ul>
</div>
</div>
<p class="caption">Allow a reasonable interval for the project. Avoid repeated pings.</p>

<!--
1 minute. Review time depends on scope and project capacity; do not promise a deadline or a merge. Follow up respectfully in the project's preferred channel. If a proposal is declined, understand the reason and use that context for the next contribution.
Source: https://opensource.guide/how-to-contribute/
-->

---
class: h4f
transition: slide-left
---

<div class="eyebrow">Audience activity / 5 minutes</div>

# Find your first opportunity

<div class="activity-grid">
<div>
<ol class="activity-steps">
<li>Visit <a href="https://bitcoindevs.xyz/contribute" target="_blank" rel="noopener noreferrer">bitcoindevs.xyz/contribute ↗</a>.</li>
<li>Pick one project that matches your skills.</li>
<li>Find its contribution guidelines.</li>
<li>Locate a beginner issue or another small task.</li>
<li>Write one question to ask before starting.</li>
</ol>
</div>
<div>
<ActivityTimer />
<p class="caption">Pair up if helpful. Share your project,<br>opportunity and question afterward.</p>
</div>
</div>
<div class="callout small"><strong>No connection?</strong> Use the example issue from slide 9 and draft your question.</div>

<!--
5 minutes. The timer starts only when clicked and can be paused or reset. Participants need only browse and take notes, not post a comment or claim a task. Suggested pacing: one minute for discovery, one for the guide, two for the issue and one for the question. If no beginner labels exist, identify a documentation gap or testing opportunity. With no connection, revisit the mock issue and ask what context is missing. Share back briefly during the summary.
Source: https://bitcoindevs.xyz/contribute
-->

---
class: h4f section summary
---

<div class="eyebrow">Your contribution journey</div>

# A path you can repeat

<div class="journey" aria-label="Nine-step contribution journey, read left to right then down">
<div class="lane-caption">FIND YOUR FIT ↓</div>
<div class="journey-row">
<div class="journey-item"><em>01</em> Choose your skills</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>02</em> Discover projects</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>03</em> Study the community</div>
</div>
<div class="lane-caption">MAKE A USEFUL CHANGE ↓</div>
<div class="journey-row">
<div class="journey-item"><em>04</em> Find an issue</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>05</em> Confirm your approach</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>06</em> Build and test</div>
</div>
<div class="lane-caption">COLLABORATE ↓</div>
<div class="journey-row">
<div class="journey-item"><em>07</em> Open a pull request</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>08</em> Respond to feedback</div><span class="journey-arrow">→</span>
<div class="journey-item"><em>09</em> Keep contributing</div>
</div>
</div>

<!--
1 minute. Invite one person to share the question they wrote. Walk through the journey from left to right, then down. Learning about the community and confirming the task are part of the contribution, not delays before the real work. The workflow is an original editable HTML diagram.
-->

---
class: h4f
---

<div class="eyebrow">Save this checklist</div>

# Before opening your first PR

<PrChecklist />

<!--
1 minute plus optional questions. This is the final checklist, with interactive checkboxes for a group recap or individual use. The state lasts for the current page session and is not sent anywhere. Ask the audience to choose the next action they can take. A useful first contribution is a beginning, not the end of participation.
-->
