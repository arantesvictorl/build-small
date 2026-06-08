---
name: build-small-hackathon
description: Keeps agents aligned with Build Small Hackathon rules, tracks, awards, and submission requirements. Use when planning, reviewing, or building any Hugging Face Build Small Hackathon project or Space.
---

# Build Small Hackathon

## Quick Start

Before implementation, identify:

- Track: Backyard AI or Thousand Token Wood.
- User or experience: who benefits or what delight is created.
- Model plan: every model must be at or below 32B total parameters.
- Deployment: Gradio app hosted as a Hugging Face Space under `build-small-hackathon`.
- Eligibility: builder joined the org and registered on the official app.
- Submission assets: README, demo video, and social post.

## Constraints

- Do not use a model above 32B total parameters.
- Prefer small-model-native ideas over generic chatbot wrappers.
- The app must be Gradio-based, even if custom UI is layered on top.
- For teams, every teammate must register, join the org, and appear by Hugging Face username in the README.
- Never commit personal redemption codes, credit links, or tracked email links.
- Keep sponsor criteria explicit in the README when targeting sponsor awards.

## Track Guidance

Backyard AI:

- Pick a real person or group.
- Solve a narrow problem.
- Show evidence of real use or realistic test cases.

Thousand Token Wood:

- Make the AI central to the fun.
- Favor originality, surprise, and polish.
- Ship a complete toy/game/art/story interaction over a vague framework.

## Award Notes

- OpenBMB: use MiniCPM models.
- OpenAI Codex: build with Codex, push to a public GitHub repo, keep Codex-attributed commits visible, and link the repo from the Space README.
- NVIDIA: use Nemotron models.
- Modal: use Modal for development or runtime and say so in the README.
- Tiny Titan: prefer models at or below 4B.
- Off-Brand: create a custom UI beyond default Gradio styling.

## Done Criteria

- Space builds cleanly.
- README includes track, badges, builder HF usernames, model parameter counts, build notes, repo link when needed, demo video, and social post.
- Demo covers the main interaction in under a few minutes.
- The app is understandable without private context.
