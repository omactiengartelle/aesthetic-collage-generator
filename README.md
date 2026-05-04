# Aesthetic Collage Generator

Generate viral aesthetic photo collages from text descriptions — magazine-style cinematic layouts with warm golden tones, layered polaroid frames, dried flowers, torn paper edges, and handwritten typography overlays. Ideal for Pinterest boards, Instagram carousels, TikTok lifestyle content, fashion lookbooks, travel diaries, mood boards, and scrapbook pages.

Powered by the Neta AI image generation API (api.talesofai.com) — the same service as neta.art/open.

## Install

```bash
npx skills add omactiengartelle/aesthetic-collage-generator
```

Or via ClawHub:

```bash
clawhub install aesthetic-collage-generator
```

## Usage

```bash
node aestheticcollagegenerator.js "your description here" --token YOUR_TOKEN
```

### Examples

Generate the default Pinterest-core aesthetic collage:

```bash
node aestheticcollagegenerator.js "aesthetic magazine-style photo collage, layered cinematic composition, warm golden tones, vintage film grain, dried flowers and pressed petals, polaroid frames and torn paper edges, handwritten typography overlays, soft sun flare, scrapbook layout, Pinterest-core, dreamy lifestyle aesthetic, high detail" --token YOUR_TOKEN
```

A travel diary style spread:

```bash
node aestheticcollagegenerator.js "summer travel diary collage, sun-bleached photos, ticket stubs and postcards, ocean horizon, golden hour" --token YOUR_TOKEN --size landscape
```

A fashion lookbook page:

```bash
node aestheticcollagegenerator.js "fashion editorial mood board, neutral tones, layered fabric swatches, vintage magazine clippings" --token YOUR_TOKEN --size tall
```

Inherit style from a reference image:

```bash
node aestheticcollagegenerator.js "autumn coffee shop scrapbook page" --token YOUR_TOKEN --ref <picture_uuid>
```

## Options

| Flag | Description | Default |
| --- | --- | --- |
| (positional) | Prompt describing the collage | built-in default |
| `--token` | Neta API token (required) | — |
| `--size` | `portrait`, `landscape`, `square`, `tall` | `portrait` |
| `--ref` | Reference image UUID for style inheritance | — |

### Sizes

| Name | Dimensions |
| --- | --- |
| `square` | 1024 × 1024 |
| `portrait` | 832 × 1216 |
| `landscape` | 1216 × 832 |
| `tall` | 704 × 1408 |

## Output

Returns a direct image URL.

## Token setup

You need a Neta API token. Sign up for a free trial at <https://www.neta.art/open/>.

Pass your token via the `--token` flag on every invocation:

```bash
node aestheticcollagegenerator.js "your prompt" --token YOUR_TOKEN
```

For convenience, you can store the token in a shell variable and expand it at call time:

```bash
node aestheticcollagegenerator.js "your prompt" --token "$NETA_TOKEN"
```

The `--token` flag is the only way the script accepts your credentials.

---

This skill requires a Neta API token (free trial available at https://www.neta.art/open/).
