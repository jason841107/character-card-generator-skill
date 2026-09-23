---
name: character-card-generator
description: Use when the user asks for a 角色卡、人物设定卡 or character cards based on portrait references, especially when they need a fictional character introduction and consistent appearance across scenes.
---

# Character Card Generator

Create reusable character cards from portrait references while keeping identity stable and making clothing scenes visibly different.

## Inputs

Require at least one main portrait image. Label every image as one of:

- identity reference
- page baseline
- style or wardrobe reference
- edit target

Treat inferred name, age, occupation, personality, and life story as fictional creative settings. Never present them as facts about a real person.

If sensual, low-neck, fitted, slip, or qipao styling is requested, require an explicitly adult character and keep the result fully clothed. Ask for another image only when the face is too small, heavily occluded, or absent.

## Preferred defaults

The main image always has priority over defaults. When a creative attribute is absent from both the image and the user's instructions, use these preferences:

- adult Asian woman, with distinct facial identity for every separate card
- height impression above 170 cm, close to an eight-head fashion proportion
- slender balanced build, fuller bust, clear collarbones, stable shoulder-waist-hip proportions
- contemporary editorial qipao, fitted dresses, slip dresses, halter dresses, and modern daily fashion, always fully clothed
- refined luminous colors such as celadon, butter yellow, tomato red, cornflower blue, smoky rose, and pale lavender, balanced with ivory, ink, or another quiet neutral

Treat these as fictional design settings. Do not claim that they are measurements or facts about a real person in a supplied image.

## Wardrobe taste contract

When the user supplies no wardrobe reference, build every look from this recipe:

- Treat the page as a complete contemporary editorial story, not an inventory of isolated dresses. Every look combines a silhouette tension, a layer relationship, a designed reveal, a material contrast, a styling friction item, and a believable social setting.
- Build silhouette tension through fitted versus oversized, exposed versus wrapped, fluid versus rigid, or body-mapped versus low-slung construction. Rotate mini, midi, and ankle or floor lengths.
- Give each look one deliberate reveal and at most one secondary focus: curved negative space, asymmetric waist, keyhole, open back, high side slit, collarbones, or structured bust shaping. Keep the adult character fully clothed.
- Layer at least two looks on the five-look page. Useful formulas include sheer over opaque, satin slip over lace or mesh, corset over jersey or knit, mini under a cropped oversized jacket, qipao top with a low-slung column skirt, and scarf or pareo wrapping over a structured base.
- Create material friction with pairings such as lace and washed denim, silk and technical nylon, sheer knit and leather, compact tailoring and liquid jersey, or satin and raw fringe. A page must not read as five smooth bodycon garments.
- Give every look one styling friction item: a sculptural colored bag, mismatched metal jewelry, a wedge or hybrid mule, a directional boot, a leather cuff, an oversized cropped jacket, or a scarf tail. Accessories complete the silhouette instead of decorating it afterward.
- Use coherent color stories rather than random variety. Favor acidic mint with oxblood, silver with tobacco brown, ivory with lacquer red, ink with electric cobalt, butter yellow with black, or plum with pale pink. Use a roughly 70/20/10 dominant-support-accent balance within each look.
- Use lived-in fashion settings such as a fitting room with a curtain wall, backstage corridor, taxi or parking garage, night convenience store, gallery stairs, elevator corridor, rooftop lounge, compact hotel dressing area, or rehearsal studio. Keep mirrors and reflective screens out of frame. Avoid repeating generic hotel lobbies and empty glamour rooftops.
- Balance polish with visible youth culture. On the five-look page, include at least one relaxed or wide-bottom silhouette, one outerwear-led look, one motion device such as a scarf tail, fringe, feathers, or bubble hem, and two ordinary day or street contexts. Allow at most one long narrow column silhouette and no more than two conventional high-heel looks.
- Rotate hair finish and beauty styling without redesigning the character. Wet texture, an ear tuck, a loose tie or braid, a beret or cap, and a slicked-back finish are allowed when the recognizable cut, length, color, hairline, and face framing remain stable.

For five wardrobe scenes, default to two modern qipao or qipao-derived looks, two dresses, and one layered fashion look. Include at least one mini look and one ankle or floor-length look, at least two layered constructions, one visible texture clash, one directional footwear choice, one relaxed or wide-bottom silhouette, one outerwear-led look, and one visible motion device. Allow at most one conventional evening gown, no more than two single-piece fitted dresses, one long narrow column silhouette, and two conventional high-heel looks.

Modern qipao may become an asymmetric wrap top with a low-slung skirt, a sleeveless mandarin-collar mini with a curved waist cutout, a translucent qipao coat over a compact knit base, a long bias qipao with a scarf tail and off-center slit, or a qipao-derived bodice with washed denim or technical nylon. Preserve Chinese identity through one or two controlled signals such as a mandarin collar, asymmetric closure, narrow piping, restrained frog buttons, abstract fringe movement, or a structured shoulder gesture. Abstract opera and heritage references into movement, proportion, color, closure, or collar construction; never reproduce full costume, headdress, stage makeup, or stacked period symbols. Avoid full-surface brocade, tourist-costume styling, and photo-studio bridal styling.

Reject generic deep-V bodycon, identical halter crop-and-mini sets, plastic-looking boning, random rhinestones, visible lingerie without tailoring, repeated bandage fabric, and the same dress with changed necklines. If the user explicitly requests maximalist, retro, glossy, ornate, or costume styling, follow that brief as an intentional override.

## Identity contract

One main image defines one character identity. Keep these stable across every page:

- face geometry, eye spacing, nose shape, lips, skin tone, and age impression
- hair color, length, part, bangs, and texture
- height impression, head-to-body ratio, shoulder width, waistline, and bust-waist-hip relationship
- persistent jewelry or other user-approved identity marks

Temporary styling may change the finish or arrangement of the same haircut, such as wet-look texture, a side sweep, an ear tuck, or a loose tie. Keep the recognizable cut, length, color, hairline, and face-framing identity stable.

Every clothing scene must use that same identity while varying expression, gaze, face angle, hand action, and pose. Separate character cards must start from separate identity anchors. Do not reuse the prior card's face, outfit, palette, temperament, or life scene unless the user explicitly requests continuity.

## Route the task

Read only the resources required by the requested output:

- Read [references/card-structure.md](references/card-structure.md) to select pages and panel inventory.
- Read [references/prompt-presets.md](references/prompt-presets.md) before generating raster assets.
- Read [references/quality-checks.md](references/quality-checks.md) before final delivery.
- Use the templates in `assets/layouts/` only for requested pages.

Default to `complete + hd` when the user gives a main image and asks for a role card without specifying page count or quality.

## Workflow

1. Inspect every reference image and record its role.
2. Build a concise identity anchor and editable fictional character settings.
3. Select page mode, style pack, and quality tier. Apply the preferred defaults only where the input leaves an attribute unspecified. Use `complete + hd` by default.
4. Use built-in `imagegen` to generate text-free raster assets.
5. Establish Page 1 as the accepted face and body baseline. Use the main image plus that baseline for later wardrobe pages.
6. Assign each wardrobe scene a different expression, gaze, head direction, hand action, and pose from the expression matrix.
7. Before generation, reject a five-look wardrobe plan that repeats more than two single-piece fitted dresses, lacks two layered constructions, uses more than one long narrow column silhouette, lacks a relaxed bottom, outerwear, or a motion detail, overuses conventional high heels, or reuses the same color story and scene vocabulary from the preceding card.
8. If identity, anatomy, outfit, or expression diversity drifts, regenerate only the affected panel or group.
9. Before composition, make a panel-use map. Assign every generated raster to exactly one destination cell. Page 2 macro details must be independent detail assets, not crops copied from its five wardrobe scenes.
10. Copy selected assets into the current project's `work/` directory.
11. Compose Page 2 as a tight editorial mosaic with hard-clipped rectangular cells and narrow dividers. Preserve every source panel's aspect ratio with uniform scaling; never force a panel into a mismatched cell. Derive the canvas from the completed layout and source aspect ratios instead of fixing page dimensions. Do not leave broad blank columns or bands. Never paste a replacement over a partially visible earlier image. Never use a blurred, mirrored, enlarged, or offset copy of the person as edge fill.
12. Render real Chinese text through the Page 1 MVG template only after its raster grid is complete. Keep Page 2 as a text-free image collage.
13. Save versioned PNG files into the current project's `outputs/` directory.
14. Run file, dimension, text, identity, expression-diversity, wardrobe-taste, panel-isolation, and thumbnail checks.
15. Report the imagegen mode, prompt set, output paths, dimensions, and any remaining limitation.

## Quality tiers

- `standard`: whole-page generation at standard detail; derive both page canvases from their completed layouts.
- `hd`: grouped generation at high detail; derive both page canvases from their completed layouts; default.
- `ultra`: individual major panels at the highest detail; derive both page canvases from their completed layouts.

Increasing canvas dimensions alone does not qualify as a clarity improvement. Inspect real facial, hair, skin, anatomy, and fabric detail at original size.

## Generation invariants

- Generate images without letters, numbers, labels, logos, signatures, or watermarks.
- Keep camera rendering and skin treatment coherent across pages.
- Use the main portrait as the strongest face reference and the accepted Page 1 image as the strongest body reference.
- Keep expressions distinct without changing eye distance, nose shape, jawline, or age impression.
- Keep body proportions stable across outfits; fitted garments must not silently alter bust, waist, hips, shoulder width, or leg ratio.
- Preserve natural hands, feet, joints, and garment construction.
- Every Page 2 wardrobe cell contains exactly one visible instance of the character. Mirrors, reflections, screens, posters, ghosted layers, blurred edge copies, and repeated background figures count as extra instances and are forbidden.
- Use every wardrobe scene exactly once. Do not reuse a crop of the same scene in another row, and do not leave any part of an old scene visible beneath a replacement.
- Keep every raster inside its assigned cell. No subject, background, label, or compositing layer may bleed into a neighboring cell.
- Page 2 is a pure image collage. Do not add titles, page numbers, section names, scene names, outfit names, captions, label gutters, footer bars, or explanatory text.
- Page 2 uses a content-fit image collage. Preserve each source image's aspect ratio and avoid fixed page dimensions, empty footer bands, duplicate scenes, or stretched panels.

## Typesetting

Render Chinese titles and necessary labels locally on Page 1 only. Do not add numeric badges or panel numbers. Page 2 must remain text-free and does not receive an MVG text overlay. For the bundled HD Page 1 template:

- reference width: 3072px; derive page height from the completed collage
- serif: `/System/Library/Fonts/Supplemental/Songti.ttc`
- sans: `/System/Library/Fonts/Hiragino Sans GB.ttc`
- output: lossless PNG

Copy the Page 1 `.mvg.template` into the project's `work/` directory, replace every `{{FIELD_NAME}}`, and draw it over the composed base image. Keep replacement text free of unmatched single quotes because MVG text values are single-quoted.

## Authorization and stopping rules

- Do not invoke paid APIs, third-party generators, publishing, or cloud uploads without explicit authorization.
- Do not overwrite an existing final asset unless the user requested replacement.
- If ImageMagick is unavailable, report the missing dependency and stop before typesetting; do not install it automatically.
- After three failures caused by the same panel-level issue, preserve valid pages, identify the failed group, and ask the user how to continue.

## Delivery

Deliver only files that pass [references/quality-checks.md](references/quality-checks.md). Include:

- the local final paths
- page dimensions and PNG format
- the prompt mode and quality tier
- a concise note about identity and expression-diversity checks
- any unresolved limitation
