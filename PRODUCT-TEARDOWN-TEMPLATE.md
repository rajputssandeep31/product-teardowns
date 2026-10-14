# Product teardown template

Maintained by Sandeep Singh Rajput. Edition 2.0. 14 October 2026.

An editable workbook with a connected Apple Music example. Worked recommendations and tests are proposals, not executed research outcomes.

## 1 Product context and decision

Use this workbook to explain how a product creates value, where one important journey becomes difficult, and what you would do next as its PM. Complete the prompts in order. The Apple Music example connects the sections; replace it with evidence about your chosen product.

Start with the product purpose and a decision worth making. Explain what works before recommending a change. Separate documented facts, reported experiences and your proposed reasoning. Keep unsupported business outcomes and company motives out of the conclusion.

Worked example: Apple Music helps listeners play known music and find something new. I would examine whether a listener can redirect an ongoing discovery session when the music fits their general taste but misses the current moment. The proposed control has not been built or tested.

### Product and value

Name the product, user value, surface, plan and observation date.

[Write your response here]

### What deserves preservation

Describe a supported strength or successful journey. What could your proposal disrupt?

[Write your response here]

### Decision to make

What choice should a PM make after reading this teardown? What evidence could change it?

[Write your response here]

## 2 Users and jobs

Define users through the situation and outcome that matter to this decision. A persona is useful when it changes the design choice. Do not invent age, occupation or purchasing power from an anonymous review.

Keep the first research group specific. Record device, app version, country, plan and current product state. Unknown metadata stays unknown. Describe the trigger, desired outcome and consequence of failure.

Worked example: A listener enjoys several genres but wants one direction during the current session. Their job is to change what plays next without confusing a temporary intention with general dislike.

| Situation | Job | Success |
| --- | --- | --- |
| Background listening | Start suitable music with little effort | Listening continues with little intervention |
| Active discovery | Find unfamiliar music worth exploring | Finds something worth saving |
| Change of session intention | Redirect the current listening session | Music fits the moment and the choice duration is understood |

### Priority group and reason

Which situation informs the first test, and why?

[Write your response here]

### Inclusions and exclusions

Record known plan, country, device, version and state; name separate cases.

[Write your response here]

## 3 Journey and existing features

Map the journey from the original trigger to completed value. Mark each step as documented, directly observed, reported or hypothetical. Do not present a proposed walkthrough as a test you performed.

Check current equivalents before proposing a feature. Include working paths and relevant eligibility. The opportunity may be how existing controls fit together, rather than a missing capability.

Worked example: Discovery Station, genre and mood playlists, preference feedback and Playlist Playground already provide different routes. Compare them before adding another way to direct music.

| Stage | Question to investigate |
| --- | --- |
| Choose a listening route | Does the listener understand the station or playlist they selected? |
| Listen and respond | Does the music fit the situation? What caused a skip? |
| Recover | Can existing routes express the current intention? |
| Continue and return | Did recovery help, and does the user understand what carries forward? |

### Journey record

For each stage write the user action, current control, evidence type and success condition.

[Write your response here]

### Existing control and eligibility

List current equivalents and how device, region or plan changes their availability.

[Write your response here]

## 4 Evidence and counterexamples

Read independent discussions and current primary documentation. Record what the evidence supports and what it cannot establish. Review complaints alongside successful experiences; their differences can reveal the actual problem.

A review is a research signal, not a representative sample or proof of internal behavior. Preserve the source, displayed date and checked date. Avoid reviewer identities and personal details. Store conflicting date metadata in research notes rather than inventing precise chronology.

Worked example: Some listeners describe valuable discoveries, while others report unsuitable direction or poor relevance. These signals require different explanations. They do not establish that Apple Music recommendations fail generally.

| Evidence type | Record |
| --- | --- |
| Official behavior | URL; checked date; revision date if shown; platform and feature scope |
| Reported experience | Independent discussion; date as displayed; journey; known segment; paraphrase |
| Counterexample | Working path or contradictory experience; differing conditions |
| Interpretation | Hypothesis, alternative and evidence that would disprove it |

### Evidence ledger

Create one record per independent source. Keep missing information visible.

[Write your response here]

### Supported conclusion

State the narrow finding supported by the records and the strongest counterexample.

[Write your response here]

## 5 Tension and prioritization

Choose a consequential tension within the user journey. Explain why this decision matters more than the other candidates. A product can work well overall and still require improvement in a specific situation.

Separate misunderstanding of controls, temporary intent mismatch and persistent poor relevance. Each needs different research and intervention. Use consequence, evidence fit and investigation effort to prioritize; do not manufacture numerical reach from reviews.

Worked example: A listener may enjoy electronic music but want rock now. Before adding a session control, check whether the person understands existing routes and can complete that task with them.

| Candidate | First decision |
| --- | --- |
| Control misunderstanding | Test existing-route understanding and visibility |
| Temporary intent mismatch | Compare recovery in the current session with existing alternatives |
| Persistent poor relevance | Investigate recommendation quality separately |

### Selected tension and priority

Name the conflict, affected situation and reason to investigate first.

[Write your response here]

### Alternative explanation

What else explains the evidence? Which observation would rule out your preferred diagnosis?

[Write your response here]

### Evidence gate

What must be true before moving to a prototype?

[Write your response here]

## 6 Scoped proposal and behavior

Define one intervention that addresses the selected tension. Explain the mechanism, trigger, user action, resulting behavior and recovery path. A feature name alone is not a product requirement.

Write acceptance conditions that can be observed. Include existing equivalents, queue or state rules, cancellation, unavailable results and accessibility. Validate feasibility before estimating engineering effort.

Worked proposal: For this session lets a listener choose a temporary direction while Discovery Station is playing. A visible label and Clear action show its duration. It must not record the action as Suggest Less or remove a Favorite. Ordinary listening-history settings still apply.

### Trigger and user action

Who can use it, where, and when? What deliberate action begins the change?

[Write your response here]

### State and acceptance conditions

What changes immediately, what ends the state, and what proves correct behavior?

[Write your response here]

### Failure and recovery

What happens when the desired result cannot be provided? Describe a truthful fallback.

[Write your response here]

### Scope and exclusions

Which existing features remain the baseline? Which adjacent problems will this change not solve?

[Write your response here]

## 7 Alternatives and business constraints

Compare realistic ways to solve the same user job. Account for the business and the people who operate the product. Documented constraints and your assumptions should remain distinguishable.

Discuss user effort, product complexity, eligibility, ongoing operations and the journeys that could be harmed. Do not infer revenue effects, recommendation architecture or company motives from public complaints.

Worked example: A session control could reduce recovery effort but adds interface and recommendation work. The existing playlist route may solve the task without building anything new. Both need evaluation.

| Option | Reason to consider | Tradeoff |
| --- | --- | --- |
| Improve existing-route guidance | Small intervention if misunderstanding is the cause | May require switching away mid-session |
| Use Playlist Playground where eligible | Existing route for a stated intention | Playlist creation and regional eligibility |
| Temporary station direction | Recovers inside the current session | Extra controls, queue state and feasibility work |

### Chosen and deferred alternatives

Compare the options on the same task and state why one earns a test.

[Write your response here]

### Stakeholders and constraints

Name the affected user journey, owner and evidence or assumption for each constraint.

[Write your response here]

## 8 Metrics and experiment

Measure completion of the user job, not adoption of your new button. Define the primary outcome, diagnostics and guardrails before inspecting results. Proposed measures are not observed company outcomes.

Compare against useful existing controls, not an artificially weak baseline. Set the observation window and minimum useful effect from baseline work. Separate usability evidence from production outcomes. Record eligibility and counterbalance order where participants see both versions.

Worked proposal: Compare current recovery routes with a session-control prototype. The primary outcome is reaching music the participant confirms fits the stated task, unaided, within a fixed window. Include failed attempts.

| Measure | Definition or purpose |
| --- | --- |
| Primary outcome | Successful eligible assigned participants / all eligible assigned participants |
| Diagnostics | Time, recovery actions, skips and selected route; inspect reasons rather than infer dislike |
| Guardrails | Duration understanding; accidental persistent feedback; playback or queue disruption; satisfaction of non-users |

### Assignment and measurement

Define eligibility, comparator, observation window, unit and treatment of failures.

[Write your response here]

### Decision rule and test status

Record baseline, justified targets and rollback criteria. State planned or completed; report inconclusive results honestly.

[Write your response here]

## 9 Execution and validation

Turn the selected proposal into work a team can evaluate. Plan the next evidence-producing step, dependencies and release gates. Do not disguise unknown feasibility as a delivery date.

Separate concept validation, engineering feasibility and a limited production experiment. Identify owners by role. Preserve a rollback path and make unintended effects observable before exposure grows.

Worked plan: First compare existing routes and the prototype. Then validate temporary queue behavior and event separation with recommendation and client owners. Proceed to a limited experiment only if duration is understood and playback remains reliable.

| Gate | Evidence required | Owner role |
| --- | --- | --- |
| Concept | Useful recovery and correct duration understanding | PM, design and research |
| Feasibility | Supported queue behavior; no persistent negative-feedback event | Client and recommendation engineering |
| Limited test | Instrumentation, assignment, guardrails and rollback ready | PM, analytics and engineering |

### Next deliverable and owner

Specify the artifact, responsible role, dependency and completion condition.

[Write your response here]

### Acceptance and rollback

Which checks must pass? What result stops or reverses the change?

[Write your response here]

### Unresolved dependencies

Record unknowns, how they will be resolved and who owns each investigation.

[Write your response here]

## 10 Overall take and public post

State what you would preserve, what you would investigate and the decision you would make next. The conclusion should follow from the product context, evidence and tradeoffs, rather than a list of PM frameworks.

For a post, introduce the product and a supported strength, explain one tension, connect it to a proposal, show the alternative and test, then link the substantive asset. Use original wording. Do not invent firsthand experience, employer endorsement or completed results.

Worked conclusion: Compare existing listening routes before building. If they solve the job with similar effort, improve their visibility or leave the journey alone. Test temporary station direction only if the in-session recovery need remains and users understand its scope.

### One page decision

Product value, user job, strength, tension, evidence, choice, tradeoff, proposed outcome and next gate.

[Write your response here]

### Exact LinkedIn draft

Write the final wording in a natural voice and link the published analysis and verified download.

[Write your response here]

### Review before publication

Record factual verification, confidentiality check, artifact download test and individual approval of the exact final post.

[Write your response here]
