---
name: hackathon-submission-check
description: Reviews Build Small Hackathon projects for submission readiness, award eligibility, README completeness, and demo/social asset gaps. Use before publishing or submitting a Build Small Space.
---

# Hackathon Submission Check

## Review Order

1. Confirm app and deployment.
2. Confirm model parameter compliance.
3. Confirm README completeness.
4. Confirm track and badge eligibility.
5. Confirm demo video and social post.
6. Identify high-impact polish gaps.

## Required Checks

- Space is under `build-small-hackathon`.
- Builder joined the org and registered on the official app.
- For team entries, every teammate joined/registered and all HF usernames are listed.
- App is Gradio-based.
- Every model is at or below 32B total parameters.
- README names the track and requested badges.
- README includes demo video and social post links.
- README explains idea, build process, tech stack, and models.
- README does not expose private redemption codes, credit links, or tracked email links.

## Award-Specific Checks

- OpenBMB: MiniCPM model usage is real and documented.
- OpenAI Codex: public GitHub repo is linked in the README and Codex-attributed commits are present and visible.
- NVIDIA: Nemotron model usage is real and documented.
- Modal: Modal usage is real and documented.
- Tiny Titan: model is at or below 4B.
- Best Agent: agent loop, tools, memory, planning, or traces are visible enough to evaluate.
- Off-Brand: app clearly goes beyond default Gradio appearance.

## Output Format

Return:

- Blockers: issues that could disqualify or prevent judging.
- Eligibility gaps: missing evidence for prizes/badges.
- Polish gaps: changes likely to improve judging.
- Submission-ready checklist: final items to complete.
