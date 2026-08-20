# Dear X, Today — Letter Paper Generation Skill

[中文](README.md) · [한국어](README.ko.md) · [English](README.en.md)

**Current version: v1.0.0** · [Changelog](CHANGELOG.md)

> I lived this day, and made it into a letter for you.

`create-dear-x-letter-paper` is an image-generation workflow Skill for ChatGPT / Codex. It turns one or more reference photos into personalized stationery with photo-derived decorations around the edges and a large, calm writing area in the center.

It is designed for fan-letter stationery, anniversary letters, photo-themed journal pages, and personalized backgrounds for printing or digital handwriting.

## What it can do

- Preserve the recognizable characteristics of the main person or subject.
- Derive the palette, lighting, season, and emotional tone from the main photo.
- Identify decorative elements in additional photos, such as flowers, drinks, tickets, clothing patterns, buildings, toys, and meaningful everyday objects.
- Harmonize elements from different photos into one light, Instagram-inspired collage style.
- Reserve approximately 65%–75% of the page as a clean central writing area by default.
- Adjust blank-space ratio, subject placement, decoration density, orientation, aspect ratio, background color, and visual style.
- Produce a flat, front-facing stationery page rather than a photographed desk scene or product mockup.

## How it works

This repository does not contain an image-generation model and does not provide a standalone image-generation API.

The Skill gives an AI system with image-generation or image-editing capabilities a consistent, reusable design workflow:

1. Use the user-designated photo, or the first uploaded photo, as the main image.
2. Use the main image to establish identity, dominant colors, lighting, and mood.
3. Treat later photos as sources of decorative elements rather than large photo tiles.
4. Select one to three distinctive elements from each supporting photo.
5. Harmonize hue, saturation, grain, outlines, and shadows across all extracted elements.
6. Arrange the subject and decorations around the page edges while protecting the central writing field.
7. Check subject fidelity, blank space, unintended text, watermarks, repeated elements, and print usability before returning the result.

Actual image creation therefore depends on whether the host environment provides a compatible image-generation or image-editing tool.

## Repository structure

```text
create-dear-x-letter-paper/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── icon.svg
└── references/
    └── design-system.md
```

- `SKILL.md`: Core triggers, workflow, user controls, and quality guardrails.
- `references/design-system.md`: Page zones, multi-photo element extraction, styles, and visual hierarchy.
- `agents/openai.yaml`: Display name, description, default prompt, and icon configuration.
- `assets/icon.svg`: Skill icon.

## Installation

Add the complete `create-dear-x-letter-paper` folder to a ChatGPT / Codex environment that supports custom Skills. Once installed, invoke it by name in your message.

Installation entry points may vary by product version and environment. Refer to the Skills page or the official instructions available in the product you are using.

## Basic usage

Upload one photo and enter:

```text
Use @create-dear-x-letter-paper to turn this photo into personalized Dear X, Today stationery.
Preserve the subject's recognizable features, leave a large central writing area,
and decorate the edges with elements derived from the photo.
```

## Multi-photo example

```text
Use the first photo as the main image and preserve the person's face, hairstyle, and clothing details.
From the next three everyday photos, extract the bouquet, coffee cup, train ticket, and sky colors as decorations.
Create portrait A4 stationery in a light Instagram-inspired collage style.
Keep about 75% of the center clean for writing, place the subject in the lower-right corner,
and do not add text, watermarks, or a photographed desk mockup.
```

## Available adjustments

You can request revisions in natural language:

- “Increase the blank area to about 82%.”
- “Move the subject to the lower-left corner and keep everything else unchanged.”
- “Add a few more decorations, but keep them outside the writing field.”
- “Change it to a landscape 4:3 layout for tablet writing.”
- “Use a pale blue-gray background derived from the photo.”
- “Reduce the retro stickers and make the result feel more like clean editorial design.”

Any setting not mentioned in a revision request should remain unchanged.

## Default design rules

- Orientation: portrait.
- Central blank area: approximately 65%–75%.
- Subject placement: along one side or in a lower corner.
- Decoration placement: small asymmetrical clusters along the top, sides, and lower corners.
- Style: light, coherent, and uncluttered Instagram-inspired collage.
- Palette: three to six colors derived from the main photo.
- Output: no hands, desk, binding, folds, paper shadows, or prewritten body text.

## Limitations and responsible use

- Required reference photos must be provided; the Skill should not recreate a missing person from memory.
- The workflow aims to preserve recognizability, but image-generation tools may still introduce errors in faces, hands, or fine details.
- Accurate text inside generated images is not always reliable. For text-heavy designs, generate text-free stationery first and add typography in a design application.
- Check dimensions, resolution, color mode, and bleed settings before printing.
- Make sure you have permission to use uploaded photos and follow applicable portrait rights, copyright rules, and platform policies.

## Project vision

“X” can be anyone you miss—or anything worth remembering.

Dear X, Today turns moments from a day genuinely lived into a page where you can write your feelings, preserve the memory, and send it to someone meaningful.

## License

This project is released under the [MIT License](LICENSE). Photos, portraits, and example assets remain subject to their own copyright and permission requirements.
