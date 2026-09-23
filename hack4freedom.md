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
duration: 45min
transition: fade
drawings:
  persist: false
---

<!-- <div class="cover-mark"><span class="bitcoin-mark" aria-label="Bitcoin"></span> Hack4Freedom</div> -->
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
1 minute. This talk follows my process: start with familiar skills, shortlist about three projects, learn how people work together, and then choose a useful task. No purchase of bitcoin is needed. Ask who has used GitHub but has not opened a PR yet. We will reserve ten minutes to find a real opportunity.
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
<tr class="activity-priority"><td><strong>Activity</strong></td><td>Are issues answered and PRs reviewed?</td></tr>
<tr><td>Language &amp; stack</td><td>Can I understand and run a small part?</td></tr>
<tr><td>Purpose</td><td>Do I care about the problem it solves?</td></tr>
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
<div class="file-row"><carbon:folder /><code>tests/</code><span>Expected behaviour</span></div>
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

<div class="eyebrow">03 / Why the guidelines matter</div>

# 

<div class="split guideline-joke">
<div>
<p class="lead"><strong>Me:</strong> “I’ll read CONTRIBUTING.md after I open the PR.”</p>
</div>
<img class="guideline-meme" src="./diagrams/after.gif" alt="Reaction meme: a man peeks around a doorway with a knowing smile." />
</div>


---
class: h4f
---

<div class="eyebrow">03 / Why the guidelines matter</div>

# 

<div class="split guideline-joke">
<div>
<p class="lead"><strong>Maintainer:</strong>Closes PR</p>
<div class="callou"><a href="https://github.com/fedimint/fedimint-sdk/pull/249#issuecomment-4088409313" target="_blank" rel="noopener noreferrer">Example</a></div>
</div>
<img class="guideline-meme" src="./diagrams/close.gif" alt="Reaction meme: a man peeks around a doorway with a knowing smile." />
</div>
<div class="caption">That was fast</div>

<!--
The speaker supplied the reaction meme. Pause for the joke, then explain the consequences aloud. This is humorous exaggeration, not a claim about every maintainer or how quickly they respond. Projects have different contribution rules. Explain that ignoring them can cause avoidable rework or a PR closing without a merge.
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
<li>Read the README and docs.</li>
<li>Explore folders and nearby code.</li>
<li>Review recently merged and open PRs.</li>
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

<div class="eyebrow">Choose your first contribution</div>
<div class="section-index">1 task → 1 PR</div>

# One useful problem.<br>A small, understood change.

<p class="lead">Your first contribution can be a good first issue, <br> a PR review, a test, or a bug someone else can reproduce.</p>

<!--
30 seconds. Before coding, find something you can work on. The next slides show alternative routes, not a checklist where everyone must do every type of contribution. First find an opportunity, check whether it still needs work, then agree on a focused next step. A useful contribution does not always require a PR.
-->

---
class: h4f
---

<div class="eyebrow">05 / Find work · Existing issues</div>

# Labels are a starting point

<div class="split wide-left">
<div class="mock">
<div class="mock-bar"><carbon:logo-github /> Issues </div>
<div class="mock-body">
<div class="search-line">is:issue state:open label:"good first issue"</div>
<span class="status">○ Open</span>
<div class="issue-title">Clarify the setup error message</div>
<div class="tags"><span class="tag">good first issue</span><span class="tag neutral">documentation</span></div>
<p class="small muted">Read the description, comments and linked work.</p>
</div>
</div>
<div>
<p class="small">Open the repository’s <strong>Issues</strong> tab and filter by label. Also look for:</p>
<div class="tags"><span class="tag">beginner friendly</span><span class="tag">help wanted</span><span class="tag neutral">tests</span></div>
<div class="callout" v-click><strong>Next: check the status</strong><br>Does this still need work?<br>Has someone already proposed a fix?</div>
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

<div class="eyebrow">05 / Check the issue</div>

# What is the issue’s current status?

<div class="issue-status-content">
<div>
<h2>Open can mean several things</h2>
<ul class="small">
<li><strong>A fix exists:</strong> it may need review, testing or closure. <a href="https://github.com/bitcoin-dev-project/bitcoin-dev-project/issues/358" target="_blank" rel="noopener noreferrer">Issue #358</a></li>
<li><strong>On the roadmap:</strong> planned work may have low priority or no urgent deadline. <br><a href="https://github.com/orgs/btcpayserver/projects/16?pane=issue&itemId=152837554&issue=btcpayserver%7Cbtcpayserver%7C7145" target="_blank" rel="noopener noreferrer">Issue #7145</a></li>
</ul>
</div>
<!-- <div>
<h2>Read the context before starting</h2>
<p class="small">Check the description, comments, labels, linked PRs and project roadmap for decisions and priorities.</p>
<p class="small">Check <strong>Development</strong> too. A timeline mention alone does not create a Development link.</p>
<p class="small muted">An empty Development section does not prove the issue is up for grabs</p>
</div> -->
</div>
<div class="callout">Confirm that the work is still needed and welcome now. If it is deferred, ask what would make it ready to work on.</div>

<!--
1 minute. An open issue is not automatically a request to start coding. Some remain open after a fix, while others are deferred pending future implementation plans, a design decision or prerequisite work. A roadmap entry can record an accepted idea without making it a current priority or urgent fix. Read the latest decisions and ask whether a contribution is welcome now. For an existing fix, offer review or testing. For deferred work, ask about the blocker or choose another task. Follow every relevant reference before assuming the work is available. Speaker-supplied example: issue #358 has the timeline entry “jrakibi mentioned this — update get funding page #359” while Development is empty. This shows a cross-reference, not necessarily a formal link. Open #359 and inspect its status and changes before concluding it resolves #358. The linked example’s current resolution status has not been verified for this presentation.
Source: https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue
-->

---
class: h4f
---

<div class="eyebrow">05 / Find work · Test the project</div>

# Expected behaviour comes from the docs

<ol>
<li><strong>Understand the feature.</strong> Read the README and relevant project docs.</li>
<li><strong>Try it yourself.</strong> Follow the documented setup and workflow.</li>
<li><strong>Compare results.</strong> What happened, and what should have happened?</li>
<li><strong>Repeat the problem.</strong> Record the version, environment and exact steps.</li>
<li><strong>Search GitHub issues.</strong> Add evidence to an existing report or create a new issue using the project’s template.</li>
</ol>

<!--
1 minute. You need enough understanding of the feature to distinguish a bug from intended behaviour or a setup mistake. You do not need to understand the entire codebase. If expected behaviour is unclear, ask a focused question and link the documentation. Search both open and closed issues before filing a duplicate. Testing someone else's fix or adding a missing test is also useful work.
Source: https://opensource.guide/how-to-contribute/
-->

---
class: h4f bug-report
---

<div class="eyebrow">05 / Report a bug/issue</div>

# A report someone else can reproduce

<div class="split">
<div>
<h2>What to include</h2>
<ul class="small">
<li><strong>Context:</strong> “While doing X, Y and Z, I found…”</li>
<li><strong>Current behaviour:</strong> describe the result. Add a screenshot or log if useful.</li>
<li><strong>Reproduction:</strong> numbered steps, version and environment.</li>
<li><strong>Expected behaviour:</strong> what should happen. Link the relevant docs.</li>
</ul>
</div>
<div>
<h2>Help the right person see it</h2>
<p class="small">Follow the project’s reporting process. If a specific maintainer’s input is needed, <strong><u>@mention</u></strong> them once and explain why.</p>
<p class="small muted">A relevant mention can notify them. Many maintainers contribute around other commitments, so give them time to respond.
</p>
</div>
</div>
<div class="callout"><a href="https://github.com/btcpayserver/btcpayserver-plugin-builder/issues/189" target="_blank" rel="noopener noreferrer">Sample issue report</a></div>

<!--
1.5 minutes. Use the issue template first. Screenshots help show a visual problem, but include exact error text and steps too. Example phrasing: “@maintainer, the contribution guide lists you for this component. Could you confirm whether this matches the intended behaviour?” Mention the relevant person when project guidance supports it or their specific input is needed, rather than tagging every maintainer. Mentions can trigger notifications, subject to settings, but do not guarantee immediate attention. Many maintainers volunteer or balance this work with other responsibilities. Keep discussion on the issue and avoid repeated pings.
Source: https://opensource.guide/how-to-contribute/
-->

---
class: h4f meme-slide
---

<div class="meme-stack">
<img class="reproduction-meme" src="./diagrams/it works.jpeg" alt="Meme: It works on my computer. Yes, but we are not going to give your computer to the client." />
<div class="callout">Clear reproduction steps help us get past “but it works on my laptop!”</div>
</div>

<!--
Pause for the joke after the bug-report slide, then return to why reproduction steps and environment details matter. Image supplied by the speaker.
-->

---
class: h4f
---

<div class="eyebrow">05 / Find work · Maintenance</div>

# Updating outdated code

<p class="lead">My merged PR replaced a dependency used for two fixed CRC calculations.</p>

<dl class="pr-details">
<dt>Opportunity</dt><dd>A dependency audit identified <code>crc_all</code> for review.</dd>
<dt>Change</dt><dd>Replace it with CRC-5-USB and CRC-16-CCITT-FALSE implementations.</dd>
<dt>Scope</dt><dd>Keep the public functions and their callers unchanged.</dd>
<dt>Evidence</dt><dd>Existing test vectors plus comparisons against the old implementation.</dd>
</dl>
<div class="callout">For outdated or unnecessary code, agree on the need and scope first. Show how you checked the behaviour.</div>
<p class="caption"><a href="https://github.com/256foundation/mujina/pull/103" target="_blank" rel="noopener noreferrer">256foundation/mujina · PR #103</a> · Merged 31 August 2026</p>

<!--
1.5 minutes. Open my PR to explain a concrete maintenance contribution. Its title is “chore(deps): replace crc_all with inline CRC implementations”. The dependency audit is discussion #8 and issue #29. The PR describes crc_all as a niche, single-maintainer crate whose generic abstraction was unnecessary for these two fixed configurations. Do not call it deprecated or claim the version was outdated. The public functions crc5, crc5_is_valid and crc16 and their protocol.rs call sites stayed unchanged. The PR reports nine CRC-5 vectors from esp-miner and one CRC-16 vector from a serial capture, plus local differential tests across all 256 one-byte and 65,536 two-byte inputs for both algorithms. These are the author's reported checks, not checks rerun for this presentation. GitHub confirms the PR merged on 31 August 2026. This example is about justified scope and verification, not a recommendation that beginners rewrite cryptographic or protocol code without understanding it.
Source: https://github.com/256foundation/mujina/pull/103
-->

---
class: h4f
---

<div class="eyebrow">05 / Find work · Other small contributions</div>

# A task you can explain and check

<div class="split">
<div class="stack">
<p><strong>Translation</strong><br><span class="small">Follow the project’s translation process and terminology.</span></p>
<p><strong>Small fixes</strong><br><span class="small">Correct a focused bug or error message, then verify it.</span></p>
<p><strong>Documentation</strong><br><span class="small">Fix an outdated instruction or explain a missing step.</span></p>
</div>
<div class="stack">
<p><strong>PR review</strong><br><span class="small">Read a proposed change. Ask a focused question or report what you tested.</span></p>
<p><strong>Tests</strong><br><span class="small">Add coverage for expected behaviour or reproduce a reported bug.</span></p>
<p><strong>Accessibility &amp; UI</strong><br><span class="small">Improve keyboard use or a confusing label.</span></p>
</div>
</div>
<div class="callout"><strong>Next:</strong> choose one opportunity, confirm it still needs work and discuss your approach.</div>

<!--
1 minute. These are alternative contribution routes. Follow the project's translation platform and review process, which may be separate from GitHub PRs. For review, distinguish reading the code from running it and report exactly what you checked. For small fixes, show the problem before the change and verify the result afterward. Now return to the shared workflow: research the chosen task and confirm the approach before coding.
Sources: https://opensource.guide/how-to-contribute/ and https://bitcoincore.org/en/contribute/
-->


---
class: h4f
---

<div class="eyebrow">06 / Research before you start coding</div>

# Confirm the context and the approach

<h2><carbon:search /> Search the repository</h2>
<ul>
<li>Related issues and earlier PRs</li>
<li>Design discussions and decisions</li>
<li>Similar code already in the project</li>
</ul>
<p class="small muted">Include closed work. Search the public chat or meeting notes too.</p>
<div class="callout">Check for duplicate work, paused proposals and decisions you may have missed.
<br>An empty Development section does not prove the issue is up for grabs.
</div>

<!--
1 minute. This reflects my habit of researching before committing to work. Search exact error strings, relevant symbols and synonyms. Check whether someone has already volunteered. Significant or unclear work merits explicit discussion before coding. Next, show how AI can help find references to verify before asking to take on the issue.
-->

---
class: h4f
---

<div class="eyebrow">06 / Use AI as a research assistant</div>

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
<div class="callout"><strong>ChatGPT or Claude in Chrome can help you research.</strong> Maintainers confirm project direction.</div>

<!--
1.5 minutes. Personal practice: ask an AI assistant for references and advice because a newcomer may miss context. AI can help with search terms, code explanations, summaries and questions, but it may lack browsing or invent references. It does not know the current task status by default. Use only public, non-sensitive material and read the actual repository policy before using AI for a contribution. This prompt is a research aid, not a product-specific feature claim.
Source for one project's policy requirements: https://github.com/bitcoin/bitcoin/blob/master/CONTRIBUTING.md
-->

---
class: h4f assignment-examples
---

<div class="eyebrow">06 / Ask to work on the issue</div>

# Ask to be assigned the issue

<div class="split">
<div class="mock">
<div class="mock-bar"><carbon:chat /> Example 1 · Request assignment</div>
<div class="mock-body small">
<p>“Hi <span v-mark><strong><u>@maintainer</u></strong></span>, I'd like to work on this issue. Is it still available?”</p>
</div>
</div>
<div class="mock" v-click>
<div class="mock-bar"><carbon:chat /> Example 2 · Confirm the approach</div>
<div class="mock-body small">
<p>“I'd like to work on this. I found the earlier discussion about the setup error.</p>
<p>Is this still available? Would clarifying the message and adding a test fit the intended approach?”</p>
</div>
</div>
</div>
<p class="caption"><a href="https://github.com/bitcoin-dev-project/bitcoin-dev-project/issues/340#event-27090589023" target="_blank" rel="noopener noreferrer">Example</a></p>
<div class="callout">Follow the project’s process for taking on work. Confirm availability and scope with a maintainer.
</div>

<!--
1 minute. Show the first comment immediately, highlight the maintainer mention on the first click, and reveal the second comment on the next click. These are example comments to adapt, not quotations from issue #340. Replace the placeholders with an approach and test you understand. Only mention research you actually completed. The linked issue is the speaker-supplied reference, not evidence that this exact comment was posted or that the issue is currently available. Ask for assignment where the project uses it, and follow the maintainer's guidance. Next, check the project’s branch workflow before making changes.
-->

---
class: h4f
---

<div class="eyebrow">07 / <carbon:warning-alt /> Before you change code</div>

# Your change needs its own branch

<p class="lead">Check the contribution guide for the correct base branch.</p>

<div class="branch-flow" aria-label="Start from the required base branch, create a feature branch, then open a pull request back to the required base">
<div><carbon:branch /><h2>Project’s base</h2><p><code>main</code>, <code>develop</code><br>or <code>staging</code></p></div>
<span class="branch-arrow" v-click="1" aria-label="Create a branch">→</span>
<div class="feature-branch" v-click="1"><carbon:code /><h2>Your feature branch</h2><p><code>fix/setup-error</code><br>Edit, commit and test here.</p></div>
<span class="branch-arrow" v-click="2" aria-label="Open a pull request">→</span>
<div v-click="2"><carbon:pull-request /><h2>PR to the base</h2><p>Review and required checks<br>before merging.</p></div>
</div>
<div class="callout branch-warning"><carbon:warning-alt /><div><strong>Do not make your contribution directly on main or staging.</strong><br>Create a separate branch for your change. Check the PR’s target branch.</div></div>

<!--
1 minute. Show the project base immediately, reveal the feature branch and its arrow on click 1, and reveal the PR and its arrow on click 2. Remind contributors to check the commit policy. Squashing combines commits into one, but is not a universal requirement: projects may preserve separate logical commits or use squash-and-merge. Follow the project’s timing for history cleanup, particularly during review. The branch names and fix/setup-error are illustrative. Do not claim most projects use staging. Read the contribution guide to determine both the starting branch and the PR target. Create a separate feature or fix branch from the required base, commit there and propose the change through the project's review process. Where a project uses an integration branch, its process determines when changes reach main. Approval and required checks depend on the repository. The diagram shows a contributor's route, not a universal release pipeline. Next, verify the change locally before preparing the PR. Explain issue links when introducing the PR description.
Sources: https://docs.github.com/en/get-started/using-github/github-flow and https://docs.github.com/en/pull-requests/reference/pull-request-merges
-->

---
class: h4f
---

<div class="eyebrow">07 / Check your work locally</div>

# Verify the change before opening your PR

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
<p>For a bug fix, show the failing behaviour and verify the correction.</p>
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
<div class="mock-bar"><carbon:pull-request /> Pull request </div>
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

<div class="eyebrow">08 / Connect the fix</div>

# Linking a PR to its issue

<div class="split">
<div>
<h2>In the PR description</h2>
<p><code>Closes #358</code><br>or <code>Fixes #358</code></p>
<p class="small">Closing keywords create the link when the PR targets the repository’s default branch.</p>
</div>
<div>
<h2>Through Development</h2>
<p>Someone with write access can select the PR in the issue’s <strong>Development</strong> section.</p>
<p class="small">A plain mention such as <code>#358</code> adds context without declaring that the PR resolves it.</p>
</div>
</div>
<div class="callout">Use a closing link when the PR resolves the issue. Merging into the default branch then closes the linked issue automatically.
<br>
<p class="small squash-reminder"><strong>Before your PR: check the commit policy.</strong> Squash into one commit if required.<br>Some projects keep separate commits or let maintainers squash at merge.</p>
</div>

<!--
1 minute. These are two ways to establish the issue–PR link. Put the closing keyword in the PR description, not just a discussion comment. For another repository, use the full reference, for example Fixes owner/repository#358. Keywords targeting a non-default branch do not create the link. A closing keyword in a commit message can close the issue without listing the containing PR as a linked PR. Manual linking through the issue's Development section requires write access. Use a normal reference for partial or related work that should not close the issue.
Source: https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue
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

<div class="eyebrow">Audience activity / 10 minutes</div>

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
<div class="callout small"><strong>No connection?</strong> Use the example issue from slide 10 and draft your question.</div>

<!--
10 minutes. The timer starts only when clicked and can be paused or reset. Participants need only browse and take notes, not post a comment or claim a task. Suggested pacing: two minutes for discovery, two for the guide, four for the issue and two for the question. If no beginner labels exist, identify a documentation gap or testing opportunity. With no connection, revisit the mock issue and ask what context is missing. Share back briefly during the summary.
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
