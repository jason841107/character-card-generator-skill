# Quality Checks

Run every applicable check before delivery. A large canvas with soft or repeated source detail does not pass the clarity gate.

## File checks

```bash
file outputs/<final>.png
sips -g format -g pixelWidth -g pixelHeight outputs/<final>.png
shasum -a 256 outputs/<final>.png
```

Required results:

- Decodable PNG.
- Exact selected dimensions for Page 1 and Page 2: 2048×3072, 3072×4608, or 4096×6144.
- Exact selected dimensions for Page 3: 2048×4096, 3072×6144, or 4096×8192.
- A recorded SHA-256 digest.
- No accidental overwrite of an accepted earlier version.

## Original-size visual check

Inspect the final PNG at original detail. Check:

- eyes, lashes, brows, nose edges, lips, pores, and hair strands
- hands, fingers, feet, joints, and limb continuity
- collarbones, shoulders, waistline, and stable body proportions
- garment seams, closures, fabric texture, slit construction, and accessories
- hard compositing seams, inconsistent light direction, duplicated objects, and false sharpening halos

If one panel fails, regenerate or replace that panel or group. Keep valid panels.

## Identity check

Compare every page with the main reference and accepted Page 1 baseline:

- face shape and facial width
- eye spacing and eye shape
- nose bridge and tip
- lips and jawline
- skin tone and age impression
- hair length, part, bangs, and texture
- height impression, head-to-body ratio, shoulder width, waistline, and bust-waist-hip relationship

Reject a panel when an expression or camera angle produces a different-looking person.

## Expression and angle diversity

For every clothing scene, record:

- expression
- gaze direction
- face angle
- head tilt
- hand action
- body stance

Adjacent scenes must differ in at least four of the six fields. Do not accept a wardrobe row that repeats one front-facing neutral face.

## Wardrobe taste check

When the user supplies no explicit wardrobe reference, confirm:

- every outfit has one silhouette tension, one layer relationship, one designed reveal, one material relationship, one styling friction item, and one believable social setting
- no look has more than two reveal or sensual-focus areas; all styling remains fully clothed and clearly adult
- Page 2 uses two modern qipao or qipao-derived looks, two dresses, and one layered fashion look by default
- Page 3 uses three qipao or qipao-derived looks, three dresses, and three layered fashion looks by default
- Page 3 contains at least two mini looks, at least two ankle or floor-length looks, at least three layered looks, at least two visible texture clashes, and at least two directional footwear choices
- Page 3 contains at least two relaxed or wide-bottom silhouettes, two outerwear-led looks, two visible motion devices, and three ordinary day or street contexts
- Page 3 contains only one conventional evening gown, no more than three single-piece fitted dresses, no more than two long narrow column silhouettes, and no more than three conventional high-heel looks
- the page uses at least four dominant colors while each look follows a controlled dominant-support-accent balance; no more than two looks use dusty or muted dominant colors
- fabrics visibly rotate between sheer and opaque, rigid and fluid, polished and raw, or traditional and technical while retaining plausible weight, lining, seams, closures, hems, and coverage
- qipao use one or two controlled Chinese signals and a clearly modern construction; useful forms include curved-cutout mini, translucent qipao coat over a compact opaque base, asymmetric wrap top with a low-slung skirt, scarf-tail bias construction, and qipao-derived bodice with denim or technical fabric
- opera or heritage influence is abstracted into movement, proportion, color, closure, collar, or structured shoulder gesture; full costume, headdress, stage makeup, and stacked period symbols are absent
- dresses and separates visibly rotate among curved negative space, asymmetric waist, layered slip, framed corsetry, sculptural drape, fringe, wrapped construction, and low-slung proportions
- accessories create intentional friction through sculptural color, directional footwear, mismatched metal, leather cuffs, cropped oversized layers, or scarf tails
- scenes form one coherent social progression and include at least three lived-in fashion contexts; generic hotel lobbies and empty glamour rooftops do not dominate
- temporary hair styling may vary, but the cut, length, color, hairline, and face-framing identity remain recognizable

Reject the whole page when more than three looks are single-piece fitted dresses, fewer than three looks are layered, more than two looks use long narrow column silhouettes, relaxed bottoms or outerwear are absent, conventional high heels dominate, the same dress appears with changed necklines, or the page reads as a department-store occasionwear catalog. Reject an individual look when it uses generic deep-V bodycon, repeated bandage fabric, plastic-looking boning, random rhinestones, exposed lingerie without tailoring, a generic halter crop-and-mini set, tourist-costume qipao, literal opera costume, photo-studio bridal styling, nude pumps with a beige clutch, or an implausible transparent garment. Keep the strongest design idea and improve construction, proportion, layering, footwear, material tension, or scene styling instead of adding decoration.

When delivering multiple cards, reject a later card that repeats more than two exact outfit formulas, the same color-story sequence, or the same social-scene progression as the preceding card.

## Text and layout check

Check:

- Page 1 uses exact Chinese characters and punctuation
- Page 1 has no numeric badges or panel numbers
- Page 2 and Page 3 contain no title, page number, section name, scene name, outfit name, caption, label band, footer, generated fake text, or other explanation
- no clipping, overlap, overflow, or mojibake
- Page 1 keeps a consistent title hierarchy and label placement
- Page 2 and Page 3 use tight image grids with hairline separators; reject broad empty columns, oversized gutters, pillarboxing, or unused header and footer space
- no source panel is stretched or compressed; faces, bodies, circles, and architectural lines retain natural proportions

## Panel isolation and source-use check

For Page 2 and Page 3, record which source asset occupies each destination cell and confirm:

- every wardrobe source is used exactly once
- Page 2 contains true macro details above and five wardrobe scenes below; no crop from those five scenes reappears as a portrait strip or detail tile
- Page 3 contains nine independent cells with exactly one visible person in each cell
- Page 3 cells follow the 1:2 target ratio and retain complete heads, feet, outfits, and poses without wide side padding
- source and destination aspect ratios match; every panel uses uniform scaling with no forced non-uniform resize
- mirrors, reflections, screens, posters, ghosted layers, blurred person-shaped fills, and offset copies are absent
- replacement assets fully cover their destination cells; no head, torso, garment, background, or seam from the previous asset remains visible
- hard clipping and gutters prevent all image content from crossing into adjacent cells

Reject and recompose the page when any source appears twice, any cell contains a second visible instance of the character, or a replacement reveals part of the image underneath it.

## Thumbnail check

Create or inspect a 360px-wide preview. Confirm:

- Page 1 title and profile text remain readable
- Page 2 and Page 3 remain clean text-free collages at thumbnail size
- panel boundaries stay clear and no face or outfit is clipped by a gutter

Adjust Page 1 text or Page 2 and Page 3 crop geometry when thumbnail readability fails.

## Cross-card check

When delivering multiple character cards, compare their Page 1 front portraits side by side. Confirm that each card has a different face, hair, outfit system, temperament, and life-scene vocabulary. Shared templates and page coordinates are allowed; shared identity is not.

## Final response

Report:

- built-in imagegen generation or edit mode
- page mode, style pack, and quality tier
- final prompt-set summary
- absolute output paths
- format and dimensions
- identity and expression-diversity result
- any unresolved limitation
