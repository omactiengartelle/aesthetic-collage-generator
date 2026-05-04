---
name: aesthetic-collage-generator
description: Create viral aesthetic photo collages — magazine-style cinematic layouts with warm tones, layered frames, flowers, and handwritten text overlays. Perfect for Pinterest boards, Instagram carousels, TikTok lifestyle content, fashion lookbooks, travel diaries, mood boards, scrapbook pages, and the trending 2026 aesthetic photo collage style popularized on social media via the Neta AI image generation API (free trial at neta.art/open).
tools: Bash
---

# Aesthetic Collage Generator

Create viral aesthetic photo collages — magazine-style cinematic layouts with warm tones, layered frames, flowers, and handwritten text overlays. Perfect for Pinterest boards, Instagram carousels, TikTok lifestyle content, fashion lookbooks, travel diaries, mood boards, scrapbook pages, and the trending 2026 aesthetic photo collage style popularized on social media.

## Token

Requires a Neta API token (free trial at <https://www.neta.art/open/>). Pass it via the `--token` flag.

```bash
node <script> "your prompt" --token YOUR_TOKEN
```

## When to use
Use when someone asks to generate or create aesthetic collage photo generator images.

## Quick start
```bash
node aestheticcollagegenerator.js "your description here" --token YOUR_TOKEN
```

## Options
- `--size` — `portrait`, `landscape`, `square`, `tall` (default: `portrait`)
- `--ref` — reference image UUID for style inheritance

## Install
```bash
npx skills add omactiengartelle/aesthetic-collage-generator
```
