# Build Small Hackathon Notes

Snapshot date: 2026-06-08.

Sources:

- https://huggingface.co/build-small-hackathon
- https://huggingface.co/spaces/build-small-hackathon/field-guide
- https://huggingface.co/spaces/build-small-hackathon/field-guide/blob/main/details.md
- Emails from Yuvi at Hugging Face sent 2026-06-03 through 2026-06-06.

## Core Idea

Build Small is a Hugging Face / Gradio hackathon focused on useful or delightful apps built with small, open or locally tinkerable models rather than giant API-only systems.

The guiding constraint is simple: build with models at or below 32B total parameters and make the result feel personal, polished, and demoable.

## Timeline

- Registration closed: 2026-06-03.
- Build window starts: 2026-06-05.
- Submissions close: 2026-06-15.
- Winners: date TBD.

## Required Constraints

- Models: each model must be at or below 32B total parameters.
- App: must be a Gradio app.
- Hosting: must be a Hugging Face Space in the `build-small-hackathon` organization.
- Eligibility: participant must both join the Hugging Face org and register on the official app.
- Teams: solo or team entries are allowed; every teammate must register, join the org, and be listed by Hugging Face username in the README.
- Submission: must include Space link, demo video, and social post.
- README: must include demo/social links, short idea description, build notes, tech used, and requested track/badges.

## Tracks

### Backyard AI

Build for a real person and a specific practical problem.

Judging signals:

- Specific real-world problem.
- The intended person actually used it.
- Honest fit between problem and small-model constraint.
- Polished Gradio app.

### Thousand Token Wood

Build something delightful, playful, weird, or AI-native.

Judging signals:

- Genuinely delightful.
- AI is central to the experience.
- Original concept.
- Polished Gradio app.

## Bonus Quests / Badges

- Off the Grid: no cloud APIs; runs locally on the model in front of the user.
- Well-Tuned: uses a fine-tuned model published on Hugging Face.
- Off-Brand: custom frontend beyond default Gradio look.
- Llama Champion: model runs through `llama.cpp`.
- Sharing is Caring: shared agent trace on the Hub.
- Field Notes: wrote a blog post or report about the build and learnings.

## Award Targets

- Main track awards: Backyard AI and Thousand Token Wood each have 1st through 4th prizes.
- Community Choice: community-voted app.
- OpenBMB: requires MiniCPM models.
- OpenAI Codex: requires building with Codex, pushing code to a public GitHub repo with Codex-attributed commits, and adding the repo link to the Space README. The track was described as $10,000 cash plus ChatGPT Pro subscriptions for the top 3.
- NVIDIA: requires Nemotron models.
- Modal: requires Modal for development or runtime and README disclosure.
- Special awards: Bonus Quest Champion, Off-Brand, Tiny Titan, Best Demo, Best Agent, Judges' Wildcard.

## Credits and Runtime Notes

- Registered builders were offered $250 in Modal credits and $20 in Hugging Face credits.
- Early registrants received a personal $100 OpenAI Codex credit code.
- Personal redemption codes and tracked claim links must not be committed to this repo or copied into public READMEs.
- Hugging Face credits were described as usable for ZeroGPU beyond the free quota, upgraded Spaces hardware, and Inference.
- Hackathon org members were described as receiving 40 minutes per day of ZeroGPU free, with additional ZeroGPU usage billed at $1 per 10 minutes against HF credits.
- HF credits from the email expire on 2026-07-31.
- Codex credit codes from the email must be redeemed by 2026-06-30.
- Gradio Discord for questions, teammates, credits, and AMAs: https://discord.gg/YHECTft87Z

## Submission Checklist

- [ ] Space exists under `build-small-hackathon`.
- [ ] Builder joined the org and registered on the official app.
- [ ] If team entry, every teammate joined/registered and all HF usernames are listed in the README.
- [ ] App launches from a clean Space build.
- [ ] App is Gradio-based.
- [ ] Every model used is documented with parameter count.
- [ ] Public GitHub repo link is present if targeting the OpenAI Codex track.
- [ ] Codex-attributed commits are visible if targeting the OpenAI Codex track.
- [ ] README frontmatter has relevant tags/tracks/badges.
- [ ] README explains idea, user, model, tech stack, and build process.
- [ ] README includes demo video link.
- [ ] README includes social post link.
- [ ] Sponsor award criteria are explicitly documented if targeted.
- [ ] No private redemption codes or tracked claim links are committed.
- [ ] Demo video shows the core workflow, not only setup.
- [ ] Social post has a clear hook, Space link, and demo link.

## Base Project Recommendation

For fast iteration across multiple Spaces, keep each idea in a separate repo or branch copied from this base, with:

- `app.py`
- `README.md`
- `requirements.txt`
- `examples/`
- `docs/decision-log.md`
- `demo/` for script, screenshots, and video notes
