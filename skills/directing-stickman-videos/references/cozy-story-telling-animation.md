# Style 7 — Cozy Story Telling Animation / 治愈故事动画风

Custom style (A7). Style 4's cozy character look, upgraded for explainers whose narration contains numbers, comparisons, places and key claims. Those moments are highlighted with animated graphs, map animations, callouts and spotlight effects, while the character and the story world stay consistent from the first clip to the last.

A7 is built on `cozy-storytelling.md` (Style 4). Read both. Where they differ, A7 takes precedence for A7 videos only: A7 keeps one consistent story world instead of Style 4's default "new setting every segment", and it adds a highlight layer. Never apply A7 to Styles 1–6 or any B style. Voice follows the shared `voice-continuity.md`.

This style has not been generation-tested. Treat anchors as a starting point and tune after 2–3 sample clips.

## Style matrix entry

| Style Key | Style Name | Visual Theme | Best For | Character Design |
|---|---|---|---|---|
| **Style 7** | Cozy Story Telling Animation (治愈故事动画风) | Style 4's warm full-color 2D cartoon world plus animated graph, map and callout plates with one consistent highlight accent color | Explainers with statistics, comparisons, timelines, geography, money, science and "how it works" stories | White filled round head, slim white torso, dark stick limbs (Style 4 anchor, unchanged) |

## Two layers

Highlights are built from two layers so that numbers are always correct:

1. **Footage layer (generated):** the cozy character scenes, plus wordless animated graphic plates (bars grow, lines draw, regions fill, needles sweep, pins drop). No readable text, letters or numerals appear in generated footage, because video models misspell and misdraw them.
2. **Overlay layer (post-production):** exact numbers, short labels and key-phrase captions added in CapCut or similar, timed to the narration. The generated plates leave clear space for them.

A graph shape from the model is illustrative. If the exact bar heights, line values or map shapes matter, generate the plate wordless and replace or overlay it with a real chart or outline asset in the editor, and say so in Phase A.

## Character and world

**Character anchor:** repeat Style 4's default anchor verbatim from `cozy-storytelling.md` in every standalone prompt. Keep action, camera scale and props outside it.

**Story world bible (new, required):** the visuals stay consistent because the world is defined once in Phase A and repeated verbatim in every prompt:

- **Home location:** one main setting (for example a cozy study, kitchen table or window desk) with fixed furniture, wall color, window position, light direction and time of day.
- **Extra locations:** at most two approved secondary settings, each frozen the same way, used only for planned story purposes. Return to the home location as the callback.
- **Palette lock:** four to six ordinary color names with roles, plus one **highlight accent color** (warm amber/gold by default) used only for highlights. Viewers then learn that the accent color means "look here."
- **Light and lens:** one consistent light direction, soft warm light and a medium cinematic framing for the whole video.
- **Graphic kit:** the same plate frame, line weight and colors for every chart and map (see below).

Scene changes inside the same location use camera position, props and graphics, not a redesigned room. Describe each new clip's opening as the same recognizable place from a stated camera angle.

## Highlight engine

In Phase A, read the narration and build a **Highlight Sheet** before writing any clip prompt. A highlight cue is any narration phrase that carries one of:

- a number, percentage, amount of money, date, rank, count or measurement
- a comparison or ratio ("twice as big", "half of")
- a change over time (growth, decline, timeline)
- a place or route
- a part of a whole
- the single key claim the viewer must remember

Each cue gets a row:

| Clip | Time | Narration phrase | Type | Exact value and source | Footage treatment | Overlay text and timing |
|---|---|---|---|---|---|---|
| 2 | 3–6s | `[phrase]` | bar / line / map / ring / callout / spotlight | `[value]` and confirmed source | wordless plate or glow | `[text]` appears at the spoken word, holds 1.5–2.5s |

Rules:

- Sync the highlight to the moment the number or place is spoken, not before.
- One idea per highlight, one highlight at a time. At most two or three highlights per ten-second clip; skip minor numbers rather than crowding the frame.
- Hold each highlight long enough to read (at least 1.5 seconds), then release it so the character scene returns.
- Never invent or round numbers silently. Every value comes from the user's script or a source the user confirms.
- Not every clip needs a graph. Pure story moments stay plain character scenes.

## Highlight types and treatments

Use the type that matches the cue. All use the story palette and the accent color.

1. **Number callout:** the camera pushes in slightly, the background softens, a clear quiet space opens near the subject (a blank wall, tabletop or window area). In post, a rounded sticker card with the number counts up in that space.
2. **Bar or column chart plate:** rounded bars grow from a baseline with a soft ease; the key bar turns the accent color and pulses once. Used for comparisons and rankings.
3. **Line chart plate:** a smooth line draws left to right; a dot at the key point blooms in the accent color. Used for trends.
4. **Ring or part-of-whole plate:** a ring fills to the share, with the filled segment in the accent color.
5. **Gauge or size comparison:** a needle sweeps, or two simple icons scale against each other to show "X times bigger".
6. **Map animation:** flat cartoon map; the camera zooms from a wider region to the subject; the region fills and glows in the accent color; a route line draws; a pin drops with a small bounce. City dots have no labels in footage; names go in post.
7. **Timeline plate:** a horizontal line with dots that light up in order as dates are spoken.
8. **Spotlight:** the object being discussed gets a soft warm halo while the rest of the scene dims slightly; used for qualitative key points.
9. **Key-phrase caption (post):** the most important two to five words appear as a highlighted caption with the accent color behind the key word.

## Graphic kit anchors

Repeat the relevant anchor verbatim in each prompt that uses it.

**Graphic plate anchor:**

```text
GRAPHIC PLATE: A clean flat rounded-rectangle panel in warm off-white with a thin dark outline matching the character's outline weight and a soft shadow, floating in the scene beside the character or filling the frame during a cut-in. Inside, simple flat shapes in the story palette on a plain background; no paper texture, no sketchbook border, no gradients beyond soft shading. Axis lines and tick marks are plain strokes with no numerals or letters. The key element uses the highlight accent color; all other elements stay in muted palette colors.
```

**Map anchor:**

```text
MAP: Flat cartoon map in the story palette: soft cream land, muted blue-green water with faint wave lines, thin soft borders, rounded friendly shapes, gentle vignette. The subject region fills with the highlight accent color and a soft glowing outline. Small round city dots with no labels. No satellite texture, no 3D terrain, no realistic map text.
```

**Highlight accent definition (in every prompt using highlights):**

```text
ACCENT: Warm amber-gold is reserved for highlighted elements only. It appears briefly at the highlight beat and then fades back; it is never used on the character, furniture or background.
```

## Post-production overlay spec

Give the user this spec with the Highlight Sheet:

- Font: a rounded bold sans-serif (for example Nunito, Poppins or Quicksand); numerals large and bold.
- Number card: warm off-white rounded card, thin dark outline, soft shadow, accent-colored underline; count-up animation over about 0.8 seconds, then hold.
- Captions: lower third safe area, one or two lines, accent color behind the key word only.
- Entrances: soft pop or slide with ease-out; exits fade over 0.3 seconds. No spinning or glitch effects.
- Keep overlays out of the character's face and the main action; use the clear space the footage leaves.

## Facts and data integrity

- Do not invent quotations, statistics, dates or sources. Mark any illustrative figure as illustrative in Phase A.
- Generated charts and maps are stylized. For factual precision, replace them with real data-driven charts or outline assets in post and keep the generated plate only as a background.
- Phase A lists each value with its source for the user to confirm before generation.

## Phase A: planning

Use the existing proposal and approval workflow. Include:

- Story world bible (home location, extra locations, palette with accent, light and lens).
- Cast cards in the Style 4 manner (one protagonist unless more are planned).
- The Highlight Sheet and the overlay spec.
- For each clip: the main setting, the character action, the highlight beats and what connects the cut (same location from a new angle, graphic wipe, or approved time jump).

## Phase B: standalone clips

Each prompt contains, in order:

1. Approved duration, ratio and technical targets; call it a `stickman animated video`.
2. Style 4 character anchor, the story world bible and palette lock, light and lens.
3. The four Style 4 scopes: static design (character and fixed location), movable prop identity, first frame and timed transfers, final state.
4. Beats at `[0–3s]`, `[3–7s]`, `[7–10s]`: character action, camera move and each highlight beat with its graphic anchor, accent and exact timing. Name the clear space left for the overlay.
5. Exact approved audio-only VO and the complete frozen voice block from `voice-continuity.md`.
6. Score, timed SFX and mix.
7. Compatible negatives.

**Audio:** warm story score with the same motif and tempo across clips. Add soft highlight SFX at low volume (a gentle pop for a number card, a light tick-up for counters, a soft whoosh for a map zoom). Narration stays first in the mix and never changes character between scenes.

**Negatives:**

```text
NO VISIBLE TEXT, LETTERS, NUMBERS, NUMERALS, SUBTITLES, LOGOS OR WATERMARKS, NO SPEECH BUBBLES, NO PHOTOREALISTIC OR 3D HUMAN CHARACTERS, NO EXTRA LIMBS, NO FUSED OR DUPLICATE HEADS, NO COSTUME OR CHARACTER REDESIGN, NO EXTRA CHARACTERS, NO PAPER TEXTURE OR SKETCHBOOK BORDER, NO SATELLITE OR REALISTIC TERRAIN, NO ACCENT COLOR ON THE CHARACTER OR BACKGROUND.
```

Keep negatives compatible with the clip: a Map clip may show the accent glow, and a Graphic plate may contain shapes, but never characters in 3D or readable chart text.

## Review

When generation is authorized, inspect actual footage for:

- Same character design, head and torso fill and proportions in every clip; two arms and two legs.
- Same home location layout, palette, light direction and lens across clips; changed angles are fine, redesigned rooms are not.
- Every highlight cue in the sheet has a matching beat, in the right place, at the spoken word.
- Plates are wordless; accent color appears only on highlighted elements; space for overlays is clear.
- Graph and map shapes are clearly illustrative or replaced with real assets.
- No unwanted text, numerals, logos, borders or paper textures.
- Wipes land on usable frames; give a candidate trim point rather than claiming seamless assembly.
- Narration compared by listening across clips; repeated voice text is not audio certification.

Record prompt compliance separately from observed output and state sampling coverage; do not claim frame-by-frame certification.
