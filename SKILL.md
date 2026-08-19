---
name: fashion-coordinate-poster
description: Create English 4:5 fashion-coordinate posters from uploaded outfit, flat-lay, garment, accessory, or styling reference images. Use for photorealistic or illustrated Japanese/Korean editorial outfit infographics, styling guides, item breakdowns, detail callouts, color palettes, or Chinese, Korean, and Malay Hijab models while strictly preserving real product color, cut, texture, construction, trouser shape, waist treatment, pockets, cords, and accessories.
---

# Fashion Coordinate Poster

Turn an outfit reference into a polished English fashion editorial poster. Treat the uploaded product image as authoritative and styling references as layout inspiration only.

## Workflow

1. Inspect every input image before generating.
2. Label each image as product authority, layout reference, or series reference. State that product authority has absolute priority and layout references may influence composition only.
3. Identify every garment, layer, accessory, color, texture, closure, waist treatment, pocket, hem, and special construction detail.
4. Select the requested model mode. If unspecified, infer the best fit from the outfit and target market.
5. Select a pattern from [references/layouts.md](references/layouts.md).
6. Draft concise English copy. Never retain Japanese, Chinese, or random reference-image text unless explicitly requested.
7. Select `Photorealistic` or `Japanese Editorial Illustration`. Use `Photorealistic` whenever the user asks for real people, real products, less AI look, or natural e-commerce photography. Use `Japanese Editorial Illustration` for 日系手绘, fashion magazine illustration, outfit breakdown, or hand-drawn styling infographic requests.
8. Use the built-in image-generation tool with only the necessary references. Put the product-authority image first and explicitly forbid layout references from redesigning products.
9. Inspect product fidelity, coverage, English text, anatomy, realism, and layout balance.
10. Correct material errors with one targeted edit while preserving everything else.

## Defaults

- Use portrait 4:5 for Shopee Malaysia and social content.
- Use English text.
- Use a warm off-white or pale neutral editorial-paper background.
- Use refined fashion illustration with fine ink lines and soft watercolor/marker shading only when the user requests or accepts illustration. Otherwise prefer photorealistic studio photography.
- Use one full-body hero model plus item cutouts, detail panels, styling notes, arrows, and a color palette.
- Use an elegant serif headline, clean sans-serif body, and restrained handwritten accent.
- Keep copy short enough to read inside the image.
- Prioritize product fidelity over decoration.

## Model Modes

### Chinese

Use a young adult Chinese woman. Keep the original outfit construction and exposure level. Choose refined natural hair and makeup appropriate to the outfit.

### Korean

Use a young adult Korean woman. Apply contemporary Korean hair, makeup, pose, and minimal styling without changing the product.

### Malay Hijab

Use a young adult Malay Muslim woman with natural Malaysian features and a coordinated hijab.

- Cover all hair and neck; show no stray hair.
- Keep arms, chest, midriff, and waist modestly covered.
- Add a simple fitted long-sleeve inner only when needed for coverage.
- Preserve the primary product. Never add sleeves to a sleeveless vest itself.
- Keep the hijab simple so it does not hide important garment construction.
- Draw the hijab color from the outfit palette, usually greige, ivory, black, taupe, or another muted neutral.

Read [references/model-modes.md](references/model-modes.md) for multiple ethnicity variants, fixed-character continuity, or difficult modest adaptations.

## Product Lock

Repeat the critical invariants in every generation prompt:

- Exact product colors and color placement.
- Exact neckline, sleeve length, garment length, silhouette, hem, layering, and fit.
- Exact fabric texture, pattern scale, sheen, seams, ribbing, pleats, gathers, and stitching.
- Exact pockets, zips, buttons, rings, straps, ties, cords, belts, and hardware.
- Exact accessory type and shape when accessories are part of the supplied look.

Never silently convert trousers into a skirt, change garment length, invent pockets, remove ties, add buttons, replace shoes, or hide a focus detail.

### Reference Priority

- Treat the product-authority image as the sole source of product truth.
- Treat layout references as composition, typography, and information-density inspiration only.
- Never copy garment construction, fit, pockets, hems, hardware, or styling changes from a layout reference.
- When a generated poster is reused as a layout reference, repeat that it cannot override the original uploaded product.

### Trouser Lock

Trousers are a high-risk item. Record and repeat:

- Waistband type, height, gathers, ruching, drawcord count, color, length, tips, and exit point.
- Leg shape: straight, wide straight, palazzo, tapered, bootcut, or flare. Do not substitute one for another.
- Exact rise, drape, length, hem width, pattern scale, fleck density, seams, pleats, and confirmed pockets.
- Whether pockets are present, functional, absent, or unconfirmed. If absent or unconfirmed, keep both hands outside and show no pocket opening.

Compare the worn trousers, item cutout, and macro panel separately against the product authority.

## Visual Medium

### Photorealistic

Use when the user asks for `真人`, `实物`, `去除AI味`, realistic, natural, catalog, or photography.

- Create a real photographed model with natural facial asymmetry, fine pores, skin variation, lip lines, individual lashes, realistic hands, nails, hair strands, and flyaways.
- Preserve normal eye size and body proportions. Avoid porcelain skin, plastic smoothing, doll faces, CGI edges, artificial glow, illustration lines, and excessive beauty filtering.
- Render genuine cloth gravity, seam tension, wrinkles, compression, contact shadows, slub, weave, sheen, and translucency.
- Make item cutouts look like real e-commerce product photography and detail panels like real macro photography.
- Use soft studio daylight and believable shadows. Do not mix photographic models with illustrated product cards.

### Illustrated

Use fine ink and soft watercolor or marker shading only when requested or clearly preferred. Keep the same product locks.

### Japanese Editorial Illustration

Use for Japanese fashion-magazine, hand-drawn coordinate, outfit-analysis, or styling-infographic references.

- Use elegant fine ink outlines, restrained watercolor or marker shading, subtle paper grain, and clean editorial whitespace.
- Use one large full-body illustrated model plus isolated product cards, accessory cards, detail crops, handwritten arrows, notes, and four to six palette swatches.
- Keep the model mature and fashion-editorial rather than anime, chibi, doll-like, or exaggerated.
- Convert all visible Japanese, Chinese, or source-image copy to concise English unless the user explicitly requests another language.
- Treat supplied style images as medium and layout references only. Never copy their garments, accessories, labels, logos, or product construction.
- Preserve realistic garment gravity, proportions, seams, hardware, and texture even though the output is illustrated.

Read [references/illustration-styles.md](references/illustration-styles.md) when the user provides hand-drawn fashion posters or requests this style.

## Poster Copy

Use only sections that improve the poster:

- `STYLE 01` or `COORDINATE 01`
- Main look title and one-sentence summary
- `STYLING POINT`
- `ITEM CHECK` or `ITEMS IN THIS LOOK`
- Two or three product-detail labels
- Three or four short checklist points
- `COLOR PALETTE` with four to six labeled swatches

Spell in-image text exactly. Keep labels concrete, such as `TEXTURED LONG VEST`, `SIDE-TIE WRAP DETAIL`, or `RELAXED WIDE-LEG PANTS`.

## Quality Check

Compare the output against the product authority image:

- Match garment lengths and layers.
- Keep trousers visibly trousers.
- Preserve special ties, rings, straps, pockets, and hems in the correct place.
- Match source color and texture.
- Check the neckline, placket, button count, pintucks, gathered seams, sleeve cuffs, side seams, and hem. Do not introduce unconfirmed slits.
- Check waistband gathers, trouser-leg width, length, fleck or print density, cords, cord tips, and pocket status.
- Ensure the model does not touch or insert a hand into an absent or unconfirmed pocket.
- In Malay Hijab mode, cover hair, neck, arms, chest, and waist.
- Make every visible word English, readable, and correctly spelled.
- Show the full body and keep key items unobstructed.
- In Photorealistic mode, reject painterly skin, plastic texture, doll-like anatomy, illustrated cutouts, or overlong and exaggerated garment proportions.

Correct only meaningful errors. Do not regenerate for minor stylistic variation.
