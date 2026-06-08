---
name: gradio-space-builder
description: Builds deployable Gradio apps for Hugging Face Spaces with simple dependency, README, and runtime conventions. Use when creating or modifying a Space app, app.py, requirements.txt, Dockerfile, or Space README.
---

# Gradio Space Builder

## Default Shape

Use this layout for simple Spaces:

```text
app.py
requirements.txt
README.md
examples/
```

Use Docker only when the app needs system packages, custom serving, `llama.cpp` builds, or other non-standard runtime setup.

## Implementation Checklist

- Keep `app.py` as the clear entry point.
- Provide examples that judges can run immediately.
- Handle missing secrets or model downloads with visible errors.
- Keep startup work minimal; lazy-load heavy models where possible.
- Include `queue()` for slow inference flows.
- Avoid private local paths and hard-coded tokens.

## README Requirements

Include:

- Space metadata frontmatter.
- What the app does.
- Track and target awards.
- Model IDs and parameter counts.
- Runtime and dependencies.
- Demo video link.
- Social post link.

## Verification

Run locally before shipping:

```bash
python app.py
```

Then test:

- first load
- example inputs
- empty/error inputs
- one full successful workflow

## Hugging Face Notes

- Use Space secrets for API keys and tokens.
- Keep model downloads compatible with Space storage/runtime limits.
- Document any hardware assumptions in the README.
