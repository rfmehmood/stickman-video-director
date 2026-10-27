# Style 6 — Urban Explainer / 城市科普风

Custom style (A6). City, geography, infrastructure, transport and scale-comparison explainers: flat-vector twilight scenes with simple black-headed characters, clean illustrated maps, short stylized 3D "scale" fly-overs, and navy-and-gold label pills added in post.

This style was derived from four reference frames supplied by the user (a bedroom scene, an illustrated map with an inset gauge, a low-poly 3D city fly-over, and a dusk bus-stop crowd). It captures the general look only: do not reproduce any channel's specific characters, logos, on-screen text or footage. It has not been generation-tested; treat anchors as a starting point and tune after 2–3 sample clips.

Style 6 is self-contained. Do not inherit Style 1's hollow-head/no-face bans, Style 2's beanie/shirt anchor, Style 3's cave/hide rules, Style 4's white-filled-head anchor, or Style 5's neck/palm/era-pack rules. Voice follows the shared `voice-continuity.md`.

## Style matrix entry

| Style Key | Style Name | Visual Theme | Best For | Character Design |
|---|---|---|---|---|
| **Style 6** | Urban Explainer (城市科普风) | Flat-vector illustrated rooms and streets in twilight palettes; illustrated maps; occasional stylized low-poly 3D scale shots | City planning, geography, transport, infrastructure, "X-sized" scale comparisons, economics and data explainers, "how cities work" stories | Solid flat-black round head, two small white dot eyes, solid-color sweater torso, thin black stick legs |

## Scene modes

Each clip has one dominant mode. Name the mode per clip in Phase A. Modes may cut within a clip, but do not blend them into one frame.

1. **Character scene** — characters in a detailed illustrated interior or street (bedroom, bus stop, platform, crossing, office).
2. **Map scene** — flat illustrated cartography with a highlighted subject region.
3. **Scale shot** — short stylized low-poly 3D fly-over to show size, density or distance. Characters never appear in 3D.
4. **Data inset** — a dark framed panel (gauge, dial, bar or icon) beside the main image, used for one comparison at a time.

## Fixed drawing grammar

Repeat the relevant anchors verbatim in every standalone prompt.

**Character anchor** (character scenes):

```text
CHARACTER: A minimalist 2D vector character with a solid flat-black round head, no hair strands, no nose and no mouth. Two small round white dot eyes; when sleeping or blinking, two short white dashes instead. The head sits directly above a simple softly shaded rounded sweater torso in one solid muted color with short matching sleeves. Two thin straight black stick legs with constant line weight and tiny dark feet. Exactly two arms and two legs. Balanced proportions: about three and a half head-heights tall, head slightly narrower than the shoulders. Expressions change only the eye marks (dots widen, dashes close, dots glance sideways); the head shape never changes. Hands, when needed, are small solid dark rounded shapes. A limb in motion replaces its previous pose; no duplicate limbs.
```

**Crowd rule:** describe a crowd as one uniform row or group using the same anchor, with varied torso colors (lavender, dusty pink, coral, teal, sage, peach, mustard) and at most one small accessory per person (hair bun, cap, beanie). Named foreground characters get their own full description. Do not spawn extra people that Phase A did not plan.

**Environment anchor** (character scenes):

```text
SETTING: Flat-vector 2D illustrated environment with soft gradient lighting, faint floating dust particles and a gentle vignette. Twilight palette: deep indigo and violet shadows, warm amber and peach glow from windows and street lamps, accents of teal, coral and mustard. Richly detailed props (books, plants, framed pictures, furniture, vehicles, skyline windows) drawn as clean simple shapes with thin soft shading. Mild shallow depth of field; a blurred foreground silhouette may frame the shot.
```

Vary the setting per story (bedroom at dawn, bus stop at dusk, platform, crossing, office). Keep character design, palette family and lighting logic fixed; change location and props.

**Map anchor** (map scenes):

```text
MAP: Flat illustrated map. Cream landmass, deep navy sea with subtle wave contour lines, thin gray country borders, soft vignette. The subject region is filled mint-teal with a soft glowing white outline. Small round city dots with tiny bold sans-serif style marks. Clean cartographic simplicity, no 3D terrain, no satellite texture.
```

**Scale-shot anchor** (3D fly-over):

```text
SCALE SHOT: Stylized low-poly 3D city fly-over at low altitude. Boxy pastel buildings in dusty pink, peach, slate blue, brick red and cream, with simple window grids and small orange rooftop boxes. A broad blue river with bridges, clustered round green trees, long straight avenues, hazy pale-blue sky with soft atmospheric perspective. Toy-model look, not photorealistic. No people, no characters.
```

**Data inset anchor:**

```text
INSET: A dark navy rounded-square panel with a thin gold border placed in a screen corner. It holds one simple icon only: a round dial gauge with tick marks and a red needle, or a plain bar. No numerals, no letters.
```

## Labels and text

Video models render text badly, so keep the generated footage free of readable text. Add labels in post-production (CapCut or similar):

- Label pill: dark navy rounded pill, thin gold border, white spaced uppercase sans-serif text (for example "ITALY-SIZED", "TALL TOWERS", "SHARED ROADS").
- Inset caption: small gold pill under the inset icon.
- Map city labels: small bold uppercase text beside city dots.
- Place pills at the lower-left or upper-center, away from faces and key action. Keep wording to one to three words.

Phase A lists each label and the clip/second where it appears. Prompts say only where empty space should be left for a label, never the label text itself.

## Facts and map accuracy

- Do not invent quotations, statistics, areas, populations or distances. Every "X-sized" comparison and number in the narration must come from a source the user confirms.
- Generated maps will not reliably draw real coastlines or borders. For factual shapes, either generate a stylized background and overlay a real outline asset in the editor, or accept an obviously illustrative map and say so in Phase A. Never present a generated shape as measured geography.
- Label placement and numbers are post-production work, so they stay editable and correct.

## Phase A: planning

Use the existing proposal and approval workflow. Include:

- **Mode plan:** the dominant mode for each clip (character, map, scale, inset) and what connects each cut.
- **Cast cards:** for each named character, torso color, accessory and role. Crowds as uniform groups.
- **Settings:** one recognizable location per character segment, with time of day and light source.
- **Palette:** four to six ordinary color names and their roles.
- **Labels:** exact label text, position and timing (post-production only).
- **Facts:** each claim and its source; mark anything illustrative.
- **Music:** one coherent score direction.

## Phase B: standalone clips

Each prompt contains:

1. Approved duration, ratio and technical targets; call it a `stickman animated video`.
2. The relevant anchor(s) for the clip's mode, plus the palette.
3. Full cast descriptions for every visible named character; uniform crowd description if used.
4. Opening layout, screen direction and held props.
5. `[0–3s]`, `[3–7s]`, `[7–10s]` beats with camera work and an ending state.
6. Exact approved audio-only VO and the complete frozen voice block from `voice-continuity.md`.
7. Score, timed SFX and voice-first mix; same score identity across clips.
8. Compatible negatives.

**Motion:** prefer slow, readable camera moves: push-in, lateral tracking along a street, parallax pan, top-down to horizon, fly-over along an avenue. For maps: the highlighted region fills in, the glow outline pulses once, the camera drifts across the sea, the gauge needle sweeps. For characters: a few concrete actions (waking, stretching, walking to a stop, boarding, looking up). Avoid liquid morphing and many simultaneous effects.

**Audio:** documentary-explainer score (light pulsing ambient electronic with soft piano or plucked synth). Subtle location SFX (city hum, bus air brakes, footsteps, alarm tick) and soft UI whooshes timed to label entrances. No mandatory piano; no change to the narrator between modes.

**Negatives:**

```text
NO VISIBLE TEXT, LETTERS, NUMBERS, SUBTITLES, LOGOS OR WATERMARKS, NO SPEECH BUBBLES, NO PHOTOREALISTIC PEOPLE, NO 3D CHARACTERS, NO EXTRA LIMBS, NO FUSED OR DUPLICATE HEADS, NO FACIAL FEATURES BEYOND TWO DOT EYES, NO COSTUME CHANGES, NO EXTRA CHARACTERS, NO REALISTIC MAP TERRAIN OR SATELLITE TEXTURE, NO BLOOD OR GORE.
```

Keep negatives compatible with the approved scene mode: do not ban the 3D look in a Scale shot, or the glow outline in a Map scene.

## Review

When generation is authorized, inspect actual footage for:

- Black round head, two white dot eyes and no extra facial marks; torso color and accessory unchanged across clips.
- Exactly two arms and two legs; no duplicate limbs during walking or turns.
- Crowd members distinguished only by torso color and one accessory, with no cloned foreground characters.
- Palette and lighting consistent within a story; settings vary by segment.
- No unwanted text, numerals or logos in the footage; labels added in post.
- Scale shots read as stylized toy models, with no people and no photorealism.
- Map shapes are clearly illustrative or replaced by a real outline overlay.
- Narrator voice listened to across all clips; repeated voice text is not audio certification.

Record prompt compliance separately from observed output and state sampling coverage; do not claim frame-by-frame certification.
