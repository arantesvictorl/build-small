---
title: <Project Name>
emoji: 🧭
colorFrom: green
colorTo: gray
sdk: gradio
sdk_version: <optional>
app_file: app.py
pinned: false
tags:
  - build-small-hackathon
  - gradio
  - <track-or-badge>
---

# <Project Name>

<One paragraph: what this Space does, who it is for, and why a small model is a good fit.>

## Track

- Target track: Backyard AI / Thousand Token Wood
- Target awards or badges:
  - <badge or sponsor award>

## Builders

| Name | Hugging Face username |
| --- | --- |
| <name> | <hf-username> |

## Demo

- Space: <Space URL>
- Public GitHub repo: <Repo URL>
- Demo video: <Video URL>
- Social post: <Post URL>

## How It Works

<Short explanation of the user flow.>

## Models

| Model | Parameters | Runtime | Why this model |
| --- | ---: | --- | --- |
| `<model-id>` | `<size>` | `<Transformers/llama.cpp/etc>` | `<reason>` |

## Tech Stack

- Gradio
- Hugging Face Spaces
- <Other dependencies>

## Build Notes

<Explain how the app was built, including Codex, fine-tuning, Modal, llama.cpp, or other sponsor-relevant tooling if applicable.>

For OpenAI Codex track eligibility, link the public GitHub repository and keep Codex-attributed commits visible.

## Local Development

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

## Submission Checklist

- [ ] App runs on the Space.
- [ ] Demo video link is public.
- [ ] Social post link is public.
- [ ] Model parameter counts are documented.
- [ ] Builder/team HF usernames are listed.
- [ ] Public GitHub repo is linked if targeting the Codex track.
- [ ] Track and badges are listed in README tags/frontmatter.
