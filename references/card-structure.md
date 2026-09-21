# Card Structure

Use this reference to choose the smallest page set that satisfies the request.

## Modes

| Mode | Pages | Default size |
| --- | --- | --- |
| `quick` | Page 1 | 2048×3072 |
| `complete` | Pages 1–3 | Page 1–2: 3072×4608; Page 3: 3072×6144 |
| `details` | Page 2 | selected tier |
| `wardrobe` | Page 3 | selected tier |

`complete` is the default when the user asks for a character card without choosing a page set.

## Page 1 — profile and expressions

Purpose: establish the canonical face, hair, body, base outfit, and fictional profile.

Required regions:

- Left information column with name, adult age, occupation, personality, face, eyes, brows, nose, lips, hair, skin, height, body proportions, and base outfit.
- Five narrow full-body angles: front, side, back, three-quarter front, and three-quarter back.
- One large beauty portrait.
- Five smaller head-angle studies.
- Three hairstyle or upper-body studies: front, side, and back.
- Five expression portraits.
- No numeric badges or panel numbers.

The five full-body angles must show the complete head and feet and use the same camera-height logic. Page 1 becomes the body baseline for all later pages.

## Page 2 — details and clothing scenes

Purpose: preserve defining details and show the character in five practical wardrobe contexts.

Required regions:

- Five facial macros: eye, eyebrow, nose, lips, and ear.
- Two skin details: cheek and shoulder/collarbone.
- Five body or garment details: collarbones, waist, hands, legs, and hair texture.
- Five large wardrobe scenes.
- No text, titles, page numbers, section labels, scene labels, outfit labels, numeric badges, or explanatory footer.

The detail grid and wardrobe row are separate regions divided only by hairline visual gutters. Detail panels show only the requested facial, skin, body, hair, or garment macro; they must not reuse portrait crops from the five wardrobe scenes. Each wardrobe scene appears once, contains exactly one visible person, keeps the same identity and body proportions, and receives a unique expression, gaze, face angle, hand action, and pose. Use the full canvas for a tight collage without reserving header, caption, footer, or broad empty areas.

## Page 3 — wardrobe expansion

Purpose: show nine clearly different outfits without turning the page into nine copies of one portrait.

Required regions:

- Three columns by three rows.
- Nine full-body or nearly full-body fashion scenes.
- No text, titles, page numbers, scene labels, outfit labels, numeric badges, or explanatory footer.

Use nine independent 1:2 portrait cells in a tight 3×3 grid that fills the full 1:2 canvas. Keep only hairline separators: at HD, use 12px horizontal outer and internal gutters plus 24px vertical outer and internal gutters on the 3072×6144 canvas. Each cell is 1008×2016. Generate source panels at 1:2 when possible, preserve their aspect ratio with uniform scaling, and never stretch them into mismatched cells. Do not create wide blank columns or bands around the images. Each cell contains exactly one visible person and one scene. Do not include mirrors, reflections, screens, posters, ghosted people, blurred person-shaped edge fill, or any subject bleeding across a cell boundary. Vary neckline, sleeve, hem, fabric, palette, environment, light, expression, head direction, hand action, and stance. Keep face geometry and body proportions locked.

## Multiple cards

For a batch of different characters:

1. Create a separate identity anchor for each main image.
2. Clear the preceding character's face, hair, palette, outfit, temperament, and scene notes before starting the next card.
3. Reuse the page system and quality criteria, not the prior character's visual identity.
4. Review cards side by side and reject accidental lookalikes.

## Naming

Use versioned filenames:

```text
<character-id>-page1-profile-v1.png
<character-id>-page2-details-scenes-v1.png
<character-id>-page3-wardrobe-v1.png
```

Increment the version rather than overwriting an accepted result.
