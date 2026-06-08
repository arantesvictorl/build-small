# Build Small Base Repo

This repository is a reusable base for Build Small Hackathon projects.

## Mission

Build small, polished Hugging Face Spaces for the Build Small Hackathon. Prefer concrete, shippable apps over broad demos. Every project should fit one of these shapes:

- Backyard AI: solves a real problem for a specific person or small group.
- Thousand Token Wood: a delightful AI-native toy, game, story, or creative interaction.

## Hackathon Constraints

- Use only models with total parameters at or below 32B. Count total parameters, not just active parameters.
- Ship as a Gradio app hosted as a Hugging Face Space under `build-small-hackathon`.
- Eligibility requires both joining the Hugging Face hackathon org and registering on the official app.
- For team projects, every teammate must register, join the org separately, and be listed by Hugging Face username in the Space README.
- Include a demo video and a social post link in the Space README.
- Keep the README current with the idea, how it was built, model choices, tech stack, demo link, social post, and requested track/badges.
- If using OpenAI/Codex for award eligibility, push to a public GitHub repo, keep Codex-attributed commits visible, and add the repo link to the Space README.
- If using Modal, note the Modal usage in the README.
- If targeting sponsor awards, explicitly document the required sponsor model/platform usage.

## Default Build Stack

Start with the simplest working stack unless the project needs more:

- Python + Gradio for the app surface.
- Hugging Face Spaces as the deployment target.
- `README.md` Space metadata frontmatter.
- `requirements.txt` or `pyproject.toml` for dependencies.
- Optional `Dockerfile` only when system packages, custom runtimes, or non-standard serving are required.

## Repo Layout

- `docs/build-small-hackathon.md`: distilled hackathon rules, timeline, awards, and submission checklist.
- `templates/space-readme.md`: README template for new Spaces.
- `skills/`: repo-local agent skills to copy or install into an agent skills directory when needed.

## Agent Workflow

For every new Space:

1. Pick the track and intended award badges before implementation.
2. Name the target user, use case, model, and deployment plan.
3. Build the smallest complete prototype first.
4. Verify locally with realistic inputs.
5. Confirm the model parameter count and document it.
6. Update the Space README before final submission.
7. Produce the demo video/script and social post draft.

## Quality Bar

- The app must be usable by a judge without private context.
- The first screen should be the actual experience, not a marketing page.
- Avoid generic chatbot wrappers unless the interaction is meaningfully adapted to the use case.
- Prefer visible product polish: good defaults, clear states, examples, loading feedback, and recoverable errors.
- Keep secrets out of the repo. Use Hugging Face Space secrets for tokens.
- Do not commit personal redemption codes, sponsor credit links, or private email links.

## Useful Links

- Hackathon org: https://huggingface.co/build-small-hackathon
- Field guide Space: https://huggingface.co/spaces/build-small-hackathon/field-guide
- Gradio docs: https://www.gradio.app/docs
- Spaces docs: https://huggingface.co/docs/hub/spaces
