# Capability inventory

This inventory audits the original Sarah Coaching Bot project and maps every distinct coaching capability into the distributable Codex plugin.

| Source capability | Original behavior | Plugin mapping |
|---|---|---|
| Practice loop | Present a fictional executive moment, collect exactly what the learner would say, show a client reaction, then critique | `sarah-coaching-practice` scenario and evaluation workflow |
| Four-quadrant method | Support for Thought, Challenge for Thought, Support for Action, Challenge for Action | Full map in the skill reference; quadrant-specific scenario creation and critique |
| Seven forms of understanding | Contributing Conditions, Self-Understanding, Recurring Pattern, Cross-Situational Meaning, Personal Contribution, Consequences and Significance, Emerging Direction | Definitions, sample invitations, filters, and primary learning targets for Support for Thought |
| Scenario variety | 160 generated cases from eight executive contexts, quadrant-specific arcs, varied fictional clients, and five difficulty levels | Generative fictional scenarios across the same contexts, arcs, quadrants, and difficulty range; no real identities copied |
| Adaptive selection | Filter by quadrant, difficulty, or Support for Thought form; prefer unseen cases and avoid immediate repeats | Conversation-level adaptive selection toward unseen and underpracticed areas |
| Ethical layers | Sponsor confidentiality, mental-health referral, third-party confidentiality/privacy, consulting boundary, conflicts of interest | Ethical layer generation plus ethics-first critique and referral/boundary rules |
| Client simulation | One plausible in-character reaction classified as receptive, considering, guarded, or withdrawn | Client reaction appears before critique and is explicitly framed as uncertain |
| Five-part rubric | Presence, Listening, Inquiry, Quadrant fit, Client ownership; 0–20 each, total 100 | Same five dimensions and formative scoring contract |
| Behavioral calibration | Detect advice, leading/closed/stacked questions, reflection, emotion, partnership, ownership, target fit, premature movement, length, and ethics awareness | Same signals guide qualitative judgment; they are evidence rather than brittle keyword rules |
| Feedback contract | Title, what worked, improvements, three alternatives, principle, confidence, caution | Same output, including exactly three stronger alternatives and ethics priority |
| Evaluation modes | Deterministic local rubric with optional AI-enhanced critique calibrated by the local result | Codex provides the nuanced critique directly while retaining the transparent rubric as its calibration guide; no external API or fallback service is required |
| Method teaching | Explain the Foursquare map, its uses, misuse risks, evidence cautions, and seven forms | “Explain the method” route in the same skill |
| Supporting approaches | ICF-aligned behavior and ethics, motivational interviewing, GROW, solution-focused coaching, cognitive/behavioral ideas, competing commitments, working alliance, coaching psychology, coach self-management | Explicitly mapped inside the reference as quadrant-supporting resources, not separate branded workflows |
| Progress reflection | Attempts, average, strongest quadrant, growth edge, quadrant balance, seven-form coverage, question discipline, reflection, advice reflex | Current-conversation progress summary and optional JSON export |
| Local history/export | Browser-local persistence, reset, and downloadable JSON | Intentionally not reproduced: a skills-only plugin has no background storage. It summarizes only the current conversation and stores nothing independently |
| Controlled improvement loop | Gold examples, human calibration, reviewed releases, rollback; no autonomous self-rewrite | Skill prohibits autonomous rubric changes and requires explicit, human-reviewed improvement |
| Safety boundary | Not therapy, crisis care, mentor coaching, supervision, credential assessment, legal advice, or HR investigation; no real client data | Preserved in skill instructions, README, and privacy review |
| Attribution boundary | No claim to speak for or be endorsed by Hicks, UT Dallas, or ICF | Preserved in skill instructions and README |
| Starter actions | The web app uses filters and buttons rather than reusable text prompts | Plugin metadata adds three equivalent starters: draw a scenario, critique a response, and practice Support for Thought |

## Packaging decision

One skill is intentional because these capabilities are phases and lenses of one coherent deliberate-practice workflow. Splitting scenarios, evaluation, method teaching, ethics, and progress into separate skills would create overlapping invocation rules and make users choose implementation details before practicing. The single skill routes among those modes while keeping installation and invocation simple.
