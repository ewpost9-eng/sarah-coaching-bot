# Sarah Coaching Bot

Sarah is a deliberate-practice partner for people learning executive and professional coaching. She gives you a fictional client moment, waits for what you would actually say, shows one plausible client reaction, and critiques your move with a transparent five-part rubric.

The method mirrors the original Sarah Coaching Lab: a Foursquare support/challenge × thought/action lens, ICF-aligned behaviors, strong client ownership, explicit ethical boundaries, and three improved alternatives after each attempt.

## Why there is one skill

The original project has one integrated coaching-practice loop, so the plugin packages it as one Codex skill rather than making people choose among overlapping skills. That single skill contains all four Foursquare quadrants, all seven Support for Thought forms, five difficulty levels, ethics cases, simulated client reactions, the five-part evaluation rubric, stronger-response examples, method explanations, adaptive practice, and progress reflection.

Supporting approaches—including motivational interviewing, GROW, solution-focused coaching, cognitive and behavioral ideas, competing commitments, working-alliance research, and coach self-management—remain inside the same method reference because the original project uses them to strengthen particular quadrants rather than as separate practice products.

See [CAPABILITY-INVENTORY.md](CAPABILITY-INVENTORY.md) for the complete source-to-plugin map.

## Install in Codex

This repository is public. You can download it without requesting access:

1. [Download or clone this repository](https://github.com/ewpost9-eng/sarah-coaching-bot) to your computer.
2. In a terminal opened inside the downloaded folder, run:

   ```text
   codex plugin marketplace add .
   codex plugin add sarah-coaching-bot@personal
   ```

3. Start a new Codex conversation so the plugin is loaded.

For context on plugin packaging and local marketplaces, see the [official Codex plugin guide](https://learn.chatgpt.com/docs/build-plugins).

## Use it

Try one of these prompts:

- “Use Sarah Coaching Practice to give me a fictional coaching scenario.”
- “Give me a level 4 Challenge for Thought drill.”
- “Critique this coaching response using Sarah's rubric: …”
- “Explain why my question moved to action too soon.”
- “Summarize my practice progress in this conversation.”

Sarah's feedback is formative practice, not therapy, supervision, credential assessment, legal advice, or HR advice. Use fictional or anonymized material only; do not enter real client names, employer secrets, or identifying information.

## What's included

- One focused skill: `sarah-coaching-practice`
- A concise method-and-rubric reference
- No external services, API keys, tracking, or stored conversation history

The original web app can keep browser-local history and export it. This skills-only plugin does not store data outside the current conversation; it can summarize attempts made in the current conversation and format that summary as JSON when asked.

The plugin does not claim affiliation with or endorsement by Robert F. Hicks, UT Dallas, or the International Coaching Federation.
