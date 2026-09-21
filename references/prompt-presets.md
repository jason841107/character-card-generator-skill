# Prompt Presets

Combine only the blocks needed for the requested page. Replace bracketed values with the approved character settings.

## `IDENTITY_LOCK`

```text
The exact same fictional adult character appears in every panel. Preserve [adult age], [ethnicity or regional appearance if requested], [face shape], [eye shape and color], [brows], [nose], [lips], [skin tone], [hair color, cut, part, bangs, and texture], and [persistent accessories]. Keep facial geometry, eye spacing, jawline, age impression, and hairstyle identical across all panels.
```

## `BODY_LOCK`

```text
Keep [height impression], [head-to-body ratio], [build], [collarbones and shoulders], [bust-waist-hip relationship], [waistline], and [leg proportion] identical across all full-body panels. Use realistic adult anatomy, natural joints, hands, and feet. Garment changes must not alter the underlying body.
```

When the supplied reference does not show enough of the body and the user provides no alternative, the preferred fictional baseline is an above-170-cm height impression, close to an eight-head fashion proportion, a slender balanced build, fuller bust, clear collarbones, and stable natural anatomy. The reference image and explicit user settings always override this baseline.

## `EXPRESSION_MATRIX`

Assign one distinct combination to each wardrobe scene and do not repeat adjacent combinations:

1. Front-facing slight smile, direct eye contact, relaxed shoulders.
2. Thoughtful three-quarter side gaze, lips relaxed, one hand near the face.
3. Calm confident chin lift, gaze past camera, upright stance.
4. Lowered gaze with a small smile while adjusting hair or a garment detail.
5. Restrained over-the-shoulder look, torso turned, eyes returning to camera.
6. Bright natural smile, face angled slightly upward, open stance.
7. Quiet neutral expression, profile view, hands loosely joined.
8. Focused gaze toward an object in the scene, three-quarter face.
9. Soft composed expression, head gently tilted, asymmetrical stance.

Expressions may change eyelids, brows, lips, and cheek tension. They must not change eye distance, nose shape, jawline, facial width, age impression, or identity.

## Wardrobe taste contract

Use this block when the user supplies no wardrobe reference:

```text
Build a complete young contemporary fashion editorial, not an inventory of isolated dresses. Every look must contain: one silhouette tension; one layer relationship; one deliberate reveal and at most one secondary focus; one visible material contrast; one styling friction item; and one believable social setting. Use fitted versus oversized, exposed versus wrapped, fluid versus rigid, or body-mapped versus low-slung construction. Keep the fictional adult fully clothed.

On a nine-look page, layer at least three looks. Use sheer over opaque, satin slip over lace or mesh, corset over jersey or knit, mini under a cropped oversized jacket, qipao top with a low-slung skirt, or scarf and pareo wrapping over a structured base. Include at least two relaxed or wide-bottom silhouettes, two outerwear-led looks, two motion devices such as scarf tails, fringe, feathers, or bubble hems, and three ordinary day or street contexts. Allow at most two long narrow column silhouettes and no more than three conventional high-heel looks. Create material friction through lace with washed denim, silk with technical nylon, sheer knit with leather, compact tailoring with liquid jersey, or satin with raw fringe. Preserve realistic hems, closures, seams, lining, fabric weight, and coverage.

Designed reveals may use curved negative space, an asymmetric waist, a keyhole, an open back, a high side slit, exposed collarbones, or structured bust shaping. Do not rely on generic deep-V bodycon, repeated bandage fabric, plastic-looking boning, random rhinestones, visible lingerie without tailoring, identical halter crop-and-mini sets, or the same dress with changed necklines.

Complete each look with one friction item such as a sculptural colored bag, mismatched metal jewelry, a wedge or hybrid mule, a directional boot, a wide leather cuff, an oversized cropped jacket, or a scarf tail. Use a roughly 70/20/10 dominant-support-accent balance within each look. Build coherent color stories rather than assigning unrelated bright colors.

Modern qipao may become an asymmetric wrap top with a low-slung skirt, a sleeveless mandarin-collar mini with a curved waist cutout, a translucent qipao coat over a compact knit base, a long bias qipao with a scarf tail and off-center slit, or a qipao-derived bodice with washed denim or technical nylon. Keep one or two controlled Chinese signals such as a mandarin collar, asymmetric closure, narrow piping, restrained frog buttons, abstract fringe movement, or a structured shoulder gesture. Abstract opera and heritage references into movement, proportion, color, closure, or collar construction. Do not reproduce full costume, headdress, stage makeup, stacked period symbols, full-surface brocade, tourist-costume styling, or photo-studio bridal styling.
```

Suggested color stories: acidic mint with oxblood; silver with tobacco brown; ivory with lacquer red; ink with electric cobalt; butter yellow with black; plum with pale pink. A complete page should use at least four distinct dominant colors while keeping each look internally controlled. No more than two looks may use dusty or muted dominant colors.

Default outfit mix:

- Page 2, five looks: two modern qipao or qipao-derived looks, two dresses, and one layered fashion look; at least one mini and one ankle or floor-length look.
- Page 3, nine looks: three qipao or qipao-derived looks, three dresses, and three layered fashion looks; at least two mini looks and two ankle or floor-length looks; at least three layered looks; at least two texture clashes; at least two directional footwear choices; at least two relaxed or wide-bottom silhouettes; at least two outerwear-led looks; at least two visible motion devices; only one conventional evening gown; no more than three single-piece fitted dresses; no more than two long narrow column silhouettes; no more than three conventional high-heel looks.

Rotate among four fashion engines so later cards do not collapse into the same polished dress formula:

- Soft tailoring and translucent shadow: nip-waist jackets, statement cuffs, curved petal cutouts, translucent outer layers over complete opaque bases, sculptural vests, and ultra-wide trousers.
- Street fracture and sport-polish collision: cropped leather or technical bombers over dresses, mesh under qipao, low-slung skirts, coated denim, bright tights, sports-jersey details with silk or tailoring, hybrid boots, and wedge sneakers.
- Romantic armor and movement: lace against hard shoulders or metal details, bubble hems, scarf tails, restrained fringe or feathers, corsetry with relaxed denim, and one movement feature rather than literal stage costume.
- Sensual material and weather: wet-look drape, frayed denim, beaded mesh over a complete opaque base, double-layer sheers, rumpled skirts, and tactile homespun surfaces. Create sensuality through motion, texture, collarbones, and proportion rather than progressively deeper necklines.

Use this nine-look capsule as the default test matrix. Recompose colors, details, and settings for later cards so separate characters do not inherit the same wardrobe identity:

1. Ice-grey translucent qipao coat over an electric-cobalt compact-knit mini, with coated-denim boots.
2. Lacquer-red sculpted nip-waist blazer dress over an ivory liquid-satin underlayer, with cherry tights and hybrid loafers.
3. Jade mesh mandarin-collar qipao top over a complete black opaque base, with a low-slung relaxed denim maxi and directional boots.
4. Tomato-red bubble-hem qipao mini with a compact military shoulder capelet and ballet-combat flats.
5. Butter-yellow cropped knit with a silver petal-cutout column skirt and metallic hybrid mules.
6. Plum lace slip over a charcoal sports jersey, shaped by a wide stud belt and tailored ankle boots.
7. Black beaded-mesh dress over a complete ivory knit column, finished with sculptural wedge sneakers.
8. Pale-pink wet-drape jersey midi dress under a cropped frayed-denim coat, with a dark leather cuff and soft directional boots.
9. Cornflower-blue corset bodice over an opaque fine-knit base, with washed-indigo relaxed jeans, a long scarf tail, and square-toe boots.

Organize Page 3 as one coherent social story. Useful progressions include bus stop to creative studio to convenience-store forecourt; rehearsal studio to backstage corridor to taxi arrival; or daylight stairwell to neighborhood restaurant to rain-lit parking garage. Include at least three day or ordinary street contexts. Do not default to nine unrelated destinations, generic hotel lobbies, empty glamour rooftops, or nine luxury-editorial interiors.

## `PAGE_1_LAYOUT`

```text
Use case: infographic-diagram. Portrait character-reference sheet. Reserve the left 24% as a clean ivory information column without generated text. On the right, create five narrow full-body angles across the top, one large beauty portrait plus five head-angle studies in the middle, three hair or upper-body studies below, and five natural expression portraits along the bottom. No text, numbers, logos, or watermarks.
```

## `PAGE_2_LAYOUT`

```text
Use case: infographic-diagram. Portrait detail-and-wardrobe sheet. Leave a clean ivory header strip. Arrange five facial macros, two wide skin-detail panels, five body or garment details, and five equal large wardrobe scenes along the bottom. Each wardrobe scene uses the same person with a different expression, gaze, face angle, hand action, and pose. No text, numbers, logos, or watermarks.
```

## `PAGE_3_LAYOUT`

```text
Use case: infographic-diagram. Portrait wardrobe expansion sheet. Leave a clean ivory header strip. Arrange a precise three-column by three-row grid of nine full-body or nearly full-body fashion scenes. Keep identity and body proportions stable while varying outfit cut, color, fabric, environment, expression, gaze, face angle, hand action, and stance. No text, numbers, logos, or watermarks.
```

## Style packs

### `STYLE_DAILY`

Design café, fitting-room mirror, sunlit apartment, gallery stairs, neighborhood convenience store, and rehearsal-studio settings. Use compact knits layered over opaque bases, shaped sundresses with directional footwear, short modern qipao, low-slung bias skirts, and one oversized cropped layer. Include one relaxed look without turning the set into conservative casualwear.

### `STYLE_URBAN`

Gallery opening, city street, elevator mirror, taxi back seat, parking garage, and after-hours lounge settings. Use technical corsetry, liquid jersey, low-slung skirts, sculptural knit, asymmetric dresses, strong cropped jackets, hybrid footwear, and controlled city lighting. Avoid generic office uniforms, hotel-lobby catalog poses, and repeated polished eveningwear.

### `STYLE_QIPAO`

Contemporary tea bar, modern Chinese residence, gallery stairs, elevator, backstage corridor, and rain-lit city settings. Vary curved-cutout mini qipao, sheer high-neck qipao over opaque corset lining, asymmetric wrap qipao tops with low-slung skirts, long bias qipao with scarf tails, and qipao-derived bodices with washed denim or technical nylon. Use one or two controlled Chinese signals per look and keep the remaining construction sharply modern. Pair with sculptural mules, wedges, hybrid shoes, or directional boots instead of repeated court shoes.

### `STYLE_TRAVEL`

Coast, pool bar, transit lounge, night market edge, ferry deck, and compact hotel-bathroom settings. Use wrapped technical layers, lined bias slips, sculpted halter maxis, asymmetric draped dresses, scarf-tail qipao, and wind-responsive fabrics with wedges, hybrid mules, soft pouches, and one strong accent bag.

### `STYLE_EVENING`

Gallery opening, backstage corridor, taxi ride, cocktail bar, theater stair, and after-hours street settings. Use a maximum of one conventional gown, plus layered slips, corset minis under oversized jackets, fringe open-side dresses, asymmetric jersey, technical satin, lace over opaque structure, and controlled metallic surfaces.

Across all style packs, use the wardrobe taste contract by default. Keep the visual result youthful, fashion-forward, sensual, and fully clothed. Qipao and dresses outweigh trousers and conservative suits. Color, hem length, neckline, shoe shape, bag shape, and scene lighting must visibly rotate across the page.

## Quality tiers

- `standard`: whole-page generation, final 2048×3072.
- `hd`: grouped generation, final 3072×4608, default.
- `ultra`: individual major panels, final 4096×6144.

For `hd`:

- Page 1 groups: full-body angles; portrait angles; hairstyle views; expressions.
- Page 2 groups: facial details; skin details; body details; wardrobe scenes.
- Page 3 groups: three wardrobe rows. Repair an individual outfit when one panel drifts.

For `ultra`, generate each major full-body or wardrobe panel separately and downsample into the final grid.

## `NO_TEXT_NEGATIVE`

```text
Do not add text, letters, numbers, captions, labels, logos, signatures, watermarks, interface elements, or decorative borders. Avoid duplicated faces, repeated expressions, identity drift, changing hair length, changing age, altered body proportions, extra fingers, fused hands, malformed feet, inconsistent garments, plastic skin, excessive smoothing, and false high-frequency sharpening.
```

## Prompt assembly order

Use this order:

```text
Use case and asset type
Input-image roles
Scene and page layout
IDENTITY_LOCK
BODY_LOCK
WARDROBE_TASTE_CONTRACT
Requested outfits and settings
EXPRESSION_MATRIX assignments
Lighting, camera, texture, and quality
NO_TEXT_NEGATIVE
```
