---
name: create-dear-x-letter-paper
description: Use when the user asks for idol letter paper, fan letter stationery, photo-derived stationery, a printable writing background, multi-photo element extraction, or revisions to a sheet's blank-space ratio, subject placement, palette, collage style, decoration density, orientation, or print size.
---

# Create Dear X, Today Letter Paper

Create one finished stationery image from the user's reference photos. Preserve the main subject's recognizability, use the main photo to establish one coherent palette and mood, and turn selected details from every supplied photo into a light Instagram-inspired collage around a large, calm writing area.

## Required tool

Use the available image-generation or image-editing tool for every requested creation or revision. Include every target reference image in the tool call. Do not imitate the subject from memory when a required image is missing; ask the user to attach it again.

## Workflow

1. Assign photo roles. Use the user-designated main photo; otherwise use the first uploaded photo as the main photo and every later photo as an element-source photo.
2. Inspect all photos internally. Identify the main person or object, clothing colors, lighting, season, setting, gestures, and the most distinctive reusable objects, motifs, textures, and color cues.
3. Infer sensible defaults from the images and the user's request. Generate directly without asking questions unless the user requests an exact print size, requires text whose wording is missing, or refers to an unavailable image.
4. Read [references/design-system.md](references/design-system.md) before composing the image.
5. Build a full-page stationery composition with the writing area as the primary functional region, the main subject as the visual anchor, and extracted elements as a unified border collage.
6. Verify before returning: the writing area is visibly usable; the subject is recognizable; every added element comes from an uploaded photo; the collage reads as one style; decorations do not invade the writing area; no unintended words, logos, watermarks, or mockup backgrounds appear.
7. Return the completed image. Keep accompanying text brief unless the user asks for an explanation.

## Composition defaults

- Default to portrait stationery with a clean central writing area occupying about 65%–75% of the page.
- Place the recognizable subject near one lower corner or along one side; keep the face and defining clothing details coherent.
- Concentrate decorative elements along the top edge, side edges, and lower corners. Maintain an irregular, scrapbook-like rhythm without forming a heavy closed frame.
- Default to a light Instagram-inspired collage treatment: small cutouts, restrained torn-paper shapes, translucent tape, instant-photo edges, postage or ticket fragments, thin hand-drawn marks, and subtle grain. Keep it airy rather than materially heavy.
- Normalize every extracted element to the main photo through shared color grading, reduced saturation, consistent edge treatment, and one shadow or outline language.
- Let decorations overlap the outer margins slightly but never cover the central writing field.
- Use a light, low-contrast background suitable for handwriting or overlaid text.
- Keep the result as a flat, front-facing page. Do not show hands holding it, desks, paper shadows, binders, folds, or product mockups unless explicitly requested.
- Do not add the project name, slogan, date, ruled lines, signature, or decorative typography unless explicitly requested.

## Subject and source fidelity

- Treat the main photo as the sole authority for identity, hairstyle, pose cues, clothing, dominant lighting, and palette. Treat later photos only as sources of supporting elements unless the user assigns different roles.
- Preserve recognizable facial structure and key styling without beautifying the person into a different identity.
- Extract or reinterpret the person as a clean cutout integrated into the border; do not place a large rectangular photo block in the center.
- Add only supportive motifs that are visually or emotionally consistent with the source, such as flowers, stars, ribbons, clouds, tickets, postage marks, doodles, fabric motifs, or setting-derived objects.
- Avoid unrelated fandom symbols, invented logos, trademarks, album names, and false signatures.

## User controls

Translate natural-language requests into these controls:

- `blank_area`: standard 65%–75%; large 75%–82%; extra-large 82%–88%.
- `orientation`: portrait, landscape, square, or an exact aspect ratio.
- `subject_position`: lower-left, lower-right, side, top corner, or balanced corners.
- `subject_scale`: accent, medium, or prominent; never let it destroy writing usability.
- `decoration_density`: sparse, balanced, or rich.
- `background`: warm ivory, cool white, pale photo-derived tint, or user-specified color.
- `style`: light Instagram collage by default for multiple photos; optional photo collage, soft scrapbook, clean editorial, hand-drawn accents, retro print, dreamy, seasonal, or source-led.

For revision requests, preserve every unspecified choice and change only the requested control.

## Multi-photo requests

- Use the designated main photo—or the first photo when none is designated—as the identity, palette, lighting, and mood anchor.
- Treat every additional photo as an element source rather than a second composition.
- Select one to three distinctive decorative elements per source photo. Good candidates include flowers, food, drinks, clouds, buildings, tickets, toys, accessories, clothing motifs, handwritten marks, packaging shapes, and characteristic colors or textures.
- Extract, simplify, crop, or stickerize selected elements before arranging them around the page. Harmonize their hue, saturation, contrast, grain, outline, and shadow with the main photo.
- Use only the strongest elements needed for a balanced result; do not represent every object from every photo.
- Never paste an additional source photo as a large rectangle. Use a small instant-photo crop only when it functions as a minor collage accent and the user has not requested element-only extraction.
- Do not extract faces or introduce additional people from source photos unless the user explicitly asks for multiple people.
- Do not create duplicate faces or merge identities unless the user explicitly asks for multiple people.
- Keep the main subject dominant and the source-derived decorations subordinate.
- Keep all decoration clusters outside the safe writing field, even when the user uploads many photos.

## Output quality guardrails

- Keep the central field genuinely empty: no faint characters, faces, objects, noisy textures, or high-contrast marks.
- Prevent cropped heads, extra fingers, duplicated limbs, distorted faces, malformed props, and repeated decorative objects.
- Prefer a restrained palette of three to six source-derived colors.
- Maintain sufficient resolution and crisp edges for digital writing and ordinary printing.
- Produce one strong result per request unless the user asks for variants.
