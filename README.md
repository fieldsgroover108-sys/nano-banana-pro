# Nano Banana Pro

Image generation & editing skill powered by Google Gemini 3 Pro Image API.

## What it does

Generate or edit images using text prompts. Supports:
- Text-to-image generation
- Image-to-image editing
- Multiple resolutions: 1K / 2K / 4K

## Quick start

```bash
# Generate a new image
uv run ~/.codex/skills/nano-banana-pro/scripts/generate_image.py \
  --prompt "your image description" \
  --filename "output.png" \
  --resolution 1K

# Edit an existing image
uv run ~/.codex/skills/nano-banana-pro/scripts/generate_image.py \
  --prompt "edit instructions" \
  --filename "output.png" \
  --input-image "input.png" \
  --resolution 2K
```

## Workflow

1. **Draft** (1K) → fast iteration
2. **Iterate** → adjust prompt
3. **Final** (4K) → only when prompt is locked

## Files

```
├── SKILL.md       # Skill definition & usage guide
├── _meta.json     # Skill metadata
└── scripts/
    └── generate_image.py   # Core generation script
```

## Requirements

- `uv` package manager
- Gemini 3 Pro Image API key
