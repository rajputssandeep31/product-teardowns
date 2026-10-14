# Product teardown template

Maintained by Sandeep Singh Rajput. Edition 1.0. 14 October 2026.

An editable workbook with a connected YouTube example. Worked recommendations and tests are proposals, not executed research outcomes.

## 1 Scope and user job

Use this workbook to turn public feedback into one product decision worth testing. Complete a specific journey before recommending a feature. The output is a decision brief supported by an evidence record, a scoped intervention and an experiment. Replace the worked examples with your own research.

Choose a narrow job, a defined user group and a product state. A complaint about downloads could concern finding a saved video, playing it, renewing its availability or exporting a file. Those are different problems. Record what you know about plan, country, device and app version; leave missing information unknown.

Worked example: A YouTube Premium viewer has completed a manual download and wants to find it for offline playback. This case examines navigation on mobile. Desktop file export, failed downloads and Premium Lite are outside the first test. The public reports do not establish every reviewer's plan, country or app build.

### Product and journey

Name the product, release or observation date and the start and end of the journey.

[Write your response here]

### User job and stakes

Describe the situation, desired outcome and consequence of failure in the user's words.

[Write your response here]

### Included and excluded segments

Specify plan, country, device, app version and relevant state. Write unknown where evidence is missing.

[Write your response here]

### Decision to make

What single decision will this teardown inform? Name the assumption that could change it.

[Write your response here]

## 2 Evidence and counterexamples

Read multiple independent discussions and current official documentation. Store the link and date with each observation. Separate a reported experience from a verified product rule and from your own interpretation. Repeated complaints identify a research question; they do not establish prevalence, churn or a cause.

Include people who succeed, not only people who struggle. Look for differences in journey, active filters, connectivity, membership and device. Do not collect reviewer identities or personal details. When a comment supplies a workaround, treat it as something to reproduce rather than as proof of a universal solution.

Worked example: Two mobile discussions describe trouble locating Downloads. Replies describe finding it through a library filter or offline entry. A separate discussion includes a positive travel use case and a desktop expectation mismatch. Together these suggest distinct issues, not a single conclusion that offline playback is broken.

| Record | What to capture |
| --- | --- |
| Official behavior | Document link; checked date; displayed update date or not shown; exact scope. |
| Reported friction | Discussion link; date as displayed; journey; known segment; paraphrased observation. |
| Counterexample | Successful journey or contradictory report; conditions that differ. |
| Interpretation | Hypothesis; alternative explanation; what observation would disprove it. |

### Evidence record

Create one record per independent source. Record missing metadata and contradictory evidence.

[Write your response here]

### What is established and what remains open

List the supported facts, qualitative signals and unresolved claims separately.

[Write your response here]

## 3 Existing experience and controls

Verify what the product already offers before proposing a change. Trace the job from entry to completion. Distinguish a missing control from an existing control that is hidden, misunderstood or failing. A help article establishes documented behavior; it does not reproduce a particular app build.

Reproduce the reported journey on the relevant version and state where access is available. Use public documentation when direct testing is unavailable, and mark the gap. Do not label a proposed walkthrough as an observed test. Avoid advising destructive workarounds such as reinstalling an app unless their consequences are verified.

Worked example: YouTube's Android help describes a Downloaded filter and Downloads playlist. Smart Downloads already exists too. The case therefore investigates access to those controls; it does not recommend adding offline downloads or automatic downloading.

| Journey step | Evidence to inspect |
| --- | --- |
| Complete a manual download | Completion state and account eligibility. |
| Open the library | Entry route and currently selected filter. |
| Find the saved video | Visibility of existing Downloads controls and list. |
| Start playback offline | Successful start versus a separate availability or playback error. |

### Reproduction record

Record device, build, plan, country, connection and filter state; actions; observed result; expected result.

[Write your response here]

### Existing control check

Does the proposed capability already exist? Is the actual gap placement, wording, consistency or function?

[Write your response here]

## 4 Diagnosis and priority

Choose a root-cause hypothesis that explains the evidence and leads to a testable intervention. Do not turn every complaint into a feature request. Use competing explanations to identify what to investigate first.

Prioritize by consequence, how directly the hypothesis fits the evidence, and the work needed to test it. Do not invent numerical reach or confidence scores from a few reviews. State which segment has evidence and which segment does not. A serious functional failure may need repair before a discovery experiment.

Worked example: The initial hypothesis is that a library state makes an existing Downloads entry hard to find. A missing entry on an affected build could instead be a regression. Expired content or incorrect membership could explain a playback failure but would not explain every navigation report.

| Hypothesis | How to distinguish it |
| --- | --- |
| Navigation or filter state | Ask users to locate a confirmed download; inspect the visible controls and active filter. |
| UI regression | Compare the documented route with the same state on affected and unaffected builds. |
| Availability or playback failure | The saved video is found but fails to play; inspect the stated error separately. |

### Selected hypothesis

State the specific failure, evidence supporting it and the most credible alternative.

[Write your response here]

### Disconfirming observation

What finding would make you abandon this diagnosis? What evidence must be collected next?

[Write your response here]

### Priority and reason

Explain why this problem deserves attention before the other candidates.

[Write your response here]

## 5 Constraints and alternatives

A useful teardown accounts for the customer, the business and the people who operate the product. Separate documented constraints from assumed company priorities. Compare realistic alternatives across the same criteria.

Record access or content rules, screen space, development effort, service reliability and affected journeys where relevant. Do not attribute motives to a company from user complaints. For each option, explain the mechanism, benefit to test, downside and condition that would make you reject it.

Worked example: Download eligibility and availability rules remain in place. Library space also serves playlists and other saved content. Whether more visibility displaces a valuable action is a design tradeoff to test, not a claim about YouTube's internal strategy.

| Option | Reason to consider | Tradeoff |
| --- | --- | --- |
| Preserve existing Downloads access across filters | Addresses a reproduced state problem. | Uses space or changes filter behavior. |
| Add contextual guidance | May help when controls exist but users miss them. | Adds interruption; cannot fix a missing control. |
| Redesign the entire library | Could simplify several journeys. | Broad effort and regression risk before the cause is known. |

### Stakeholders and constraints

Name the user job, business requirement, operating owner and evidence for each constraint.

[Write your response here]

### Alternative chosen and alternative deferred

Explain the tradeoff using the observed problem rather than a generic feature ranking.

[Write your response here]

## 6 One scoped intervention

Describe the smallest change that tests your diagnosis without adding unrelated features. Write the trigger, user action, expected product behavior and failure or recovery path. Specify what remains unchanged so reviewers can assess the scope.

Reproduce the failure before deciding implementation. If a documented control is missing, repair that state before experimenting with explanatory copy. If the control is present but missed, test visibility or guidance against the current experience, including any guidance already present.

Worked proposal: If an active Playlists filter makes Downloads inaccessible on an affected build, preserve a visible route to the existing Downloads view. Keep the existing download and content-availability rules. This is a conditional proposal; the reported state has not been reproduced in this analysis.

### Eligibility and trigger

Which users and product state receive the change? Which users remain excluded?

[Write your response here]

### Behavior and scope

What can the user do, where, and what happens next? State one acceptance condition.

[Write your response here]

### Existing feature and failure check

Describe the current equivalent or nearest control. What happens if no eligible download exists?

[Write your response here]

### Dependencies and owner

Name the responsible roles and prerequisites. What evidence permits a prototype or repair to begin?

[Write your response here]

## 7 Experiment and measures

Make success observable at the end of the user job. Choose a primary outcome, diagnostic measures and guardrails before inspecting results. Every target needs a rationale. Leave targets unset when there is no baseline or agreed acceptable effect.

Start with a task-based comparison of the current experience and a prototype. For a later production test, define eligibility, random assignment, duration and the sample needed with the analytics owner. Do not claim that a small usability exercise estimates population conversion or retention.

Worked proposal: Ask eligible mobile Premium users with a verified manual download to locate it and start playback under controlled offline conditions. Compare the current navigation with the scoped prototype. Separate inability to find the video from a failure after pressing play.

| Measure | Definition |
| --- | --- |
| Primary task success | Eligible assigned participants who find the video and start playback without help / all eligible assigned participants. |
| Diagnostic | Time from task instruction to playback; navigation backtracks; help requests. |
| Guardrails | Playlist task success; playback errors after the video is found; accidental changes to saved content. |

### Assignment and observation window

Define comparison, eligibility, device and country segments, task order and timing. Include failed attempts in the denominator.

[Write your response here]

### Targets and decision rule

Set the minimum useful effect and acceptable guardrail change with a rationale. Record inconclusive results without calling them success.

[Write your response here]

### Test status

Planned or completed? If completed, record sample, exclusions, uncertainty and actual results. Never fill example results as observed data.

[Write your response here]

## 8 Decision brief and reusable post

Bring the reasoning together in one decision brief. A reviewer should be able to understand the problem, follow the evidence and see why the proposed change addresses it. Update the brief when new evidence changes the diagnosis.

For a public post, explain the user situation before naming the fix. Include an existing product control, a specific proposal, an alternative and its tradeoff, then the proposed test. Link to the substantive analysis and template. Do not imply employment at the company, internal access or completed experiments.

Worked conclusion: Investigate mobile download findability first. Verify the reported library and filter state, then test consistent access to the existing Downloads view if the issue is reproduced. Positive offline-use reports keep us from calling the entire feature broken. The evidence does not establish how many users are affected.

### One page decision

User job; narrow friction; evidence and limits; chosen intervention; alternative; constraints; primary outcome and guardrails.

[Write your response here]

### Proceed change or stop

Who decides, on what evidence, by when? What would lead to a repair, a usability test, more research or no change?

[Write your response here]

### Public post draft

Write the exact text. Identify hypothetical reasoning and include a working public artifact link.

[Write your response here]

### Release check

Record current control verification, source dates, privacy check, artifact download test and individual approval of the final post.

[Write your response here]
