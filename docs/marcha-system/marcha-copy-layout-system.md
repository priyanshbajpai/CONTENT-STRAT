# Marcha Copy + Layout System

## Prime Rule

Every Marcha post must feel like a premium food brand, not a generic recipe page.

The copy should make people think:

> This should exist as a real food product.

Before writing final copy or generating visuals, use the Marcha research gate:

- check current trend and internet signals
- validate that the idea fits Indian Gen Z, healthy-ish food, quick-commerce, or FMCG behaviour
- define the real food texture, colour, and preparation logic
- reject concepts that would look fake, inedible, or visually impossible

## Production Output Rule

For Marcha carousels, generate two separate outputs:

1. **Clean visual slides**
   - all 7 slides as final food/image backgrounds
   - no text, no logos, no labels, no watermarks
   - realistic food, correct aspect ratio, complete visual composition

2. **Text placement layout**
   - one matching guide per slide
   - shows where the user should place headline, microcopy, callouts, page number, and CTA
   - includes exact copy separately

Do not bake final text into the main carousel visuals unless explicitly requested.

Before delivery, every exported asset must pass a pixel check:

- carousel clean visual: exactly `1080 x 1350`
- carousel text placement guide: exactly `1080 x 1350`
- reel clean visual/frame: exactly `1080 x 1920`
- reel text placement guide: exactly `1080 x 1920`
- single image clean visual: exactly `1080 x 1350`
- single image text placement guide: exactly `1080 x 1350`

If an image model returns the wrong canvas, crop and resize it to the locked format before delivery.

The final user workflow is:

1. Use the clean visual slide.
2. Add the provided copy manually.
3. Follow the matching text placement guide.
4. Keep the type integrated into negative space, not in separate blocks.

## Copywriting Voice

Marcha copy is:

- premium
- editorial
- concise
- sensory
- confident
- modern Indian
- product-minded
- never gimmicky
- never overly meme-heavy

Avoid:

- long captions on visuals
- generic food influencer phrases
- medical health claims
- fake urgency
- messy AI-sounding language

## Copy Formula

Use this structure across formats:

1. **Name the tension**
   - Ketchup is familiar, but boring.
   - Healthy food should not taste like punishment.
   - Chutney is powerful, but not portable.

2. **Reveal the concept**
   - Kashmiri Garlic Tomato Chilli.
   - Makhani Hummus.
   - Pani Puri Drizzle.

3. **Make it useful**
   - For momos, fries, dosa, rolls.
   - For wraps, bowls, toast, and snacks.

4. **Ask a product question**
   - Would you buy this?
   - Should this exist?
   - What would you eat this with?

## Aspect Ratios

These are locked. Do not change the canvas size per post unless the platform changes.

Final files must be exported at the exact pixel dimensions below, not merely “close to” the ratio.

### Instagram Carousel

- Ratio: `4:5`
- Size: `1080 x 1350`
- Use for: concepts, recipes, breakdowns, product ideas

### Single Image Feed Post

- Ratio: `4:5`
- Size: `1080 x 1350`
- Use for: hero food shots, product posters, quote/hot take posts

### Reel / Short Video

- Ratio: `9:16`
- Size: `1080 x 1920`
- Keep text inside safe zone:
  - top margin: 220 px
  - bottom margin: 320 px
  - side margin: 90 px

### Story

- Ratio: `9:16`
- Size: `1080 x 1920`
- Use sparingly for polls, concept voting, and behind-the-scenes.

## Image Style Language

Every Marcha image should feel like contemporary studio food photography with a 1970s hard-flash cookbook memory and a modern pop-art food lab finish.

Important direction:

- Text should be integrated into the image composition.
- Avoid obvious text blocks, floating cards, sticker labels, or button-like CTAs.
- Typography should sit directly on clean negative space, like an editorial food page or menu layout.
- Use fine callout lines, small ingredient labels, page numbers, menu-style boxes with only thin outlines, and calm body text.
- The image and text must feel designed together, not like text added after the fact.

Use these visual rules for generated images:

- medium: premium commercial food photography, not illustration
- lighting: hard direct flash or hard direct sunlight, one strong source
- shadows: crisp, dark, visible, and intentional
- focus: deep focus with sharp food, hands, props, and edges
- background: solid matte color fields, never busy kitchens or lifestyle rooms
- composition: minimalist, isolated, lots of negative space for text
- subject: close-up food action, ingredient layout, sauce pour, dip, hand gesture, plated hero
- texture: glossy sauces, crisp toppings, charred edges, fresh herbs, tactile ingredients
- camera: 50mm to 85mm equivalent, no wide-angle distortion
- finish: clean white balance, high local contrast, no haze, no grain, no soft blur
- brand fit: Indian pantry, global format, vegetarian-first, premium but edible
- scroll-stop power: one strong visual action or one unmistakable food object per slide
- copy relevance: the image must illustrate the exact slide message, not just the general concept
- platform behaviour: the cover should read instantly in a busy Instagram feed

Avoid:

- generated text, labels, logos, watermarks, fake typography, or misspelled packaging
- smoky restaurant lighting, dark moody backgrounds, rustic wood tables, cluttered kitchens
- blurry motion, shallow-focus food, messy sauce splatter unless intentionally graphic
- unrealistic neon food colors or inedible styling
- solid text cards placed over the food
- oversized CTA buttons
- heavy boxes that separate copy from the photograph

## Image Generation Prompt Base

Use this base for Marcha visual generation, then change only the subject and format:

```text
Premium contemporary studio food photography for Marcha, a modern Indian food lab. Hard direct flash lighting, crisp dark shadows, extremely sharp edges, deep focus, high-saturation color blocking, one solid matte background in a Marcha brand colour, minimalist composition with generous negative space reserved for typography. Do not use dual-colour, split, half-and-half, curved-block, or multi-panel backgrounds. Close-up edible vegetarian food action, realistic tactile food texture, fresh Indian pantry ingredients, modern global-fusion presentation using ingredients available in India. The food must look exactly as if it was made in reality: believable colour, shape, structure, portion, viscosity, gloss, spice flecks, oil sheen, herb texture, toasted or crisp edges where relevant. Name the food's texture and viscosity precisely: spoonable, pourable ribbon, slow drip, spreadable, set, airy, crumbly, crunchy, or crisp. 50mm to 85mm lens feel, clean white balance, high local contrast, no haze, no grain, no blur. No text, no logo, no watermark, no packaging words.
```

### Format Prompt Add-Ons

Carousel cover, `1080 x 1350`:

```text
Vertical 4:5 Instagram carousel cover. Leave clean negative space in the upper-left or center-left for a large editorial headline. Food action should sit in the lower half or right side. No text in the image.
```

Carousel ingredient slide, `1080 x 1350`:

```text
Vertical 4:5 ingredient still life. Ingredients arranged with premium spacing on a matte background, crisp shadows, clean negative space for labels. No text in the image.
```

Carousel process slide, `1080 x 1350`:

```text
Vertical 4:5 faceless hand-action food shot. A hand is pouring, dipping, spreading, tearing, sprinkling, blending, or plating. Keep the action sharp and centered with negative space for a short headline. No text in the image.
```

Reel frame, `1080 x 1920`:

```text
Vertical 9:16 reel frame. Keep the main food action between the center and lower third. Leave safe empty space in the top third and lower third for text overlays, away from social app UI. No text in the image.
```

Single image post, `1080 x 1350`:

```text
Vertical 4:5 premium food hero poster. One strong food subject, graphic matte background, crisp hard shadow, clean headline space. No text in the image.
```

## Text Placement Rules

Every text placement guide must include:

- exact copy for that slide
- font family
- font size in px
- font colour and hex code
- font style: regular, bold, italic, underline
- font effects: none, subtle shadow, opacity, outline, line height, letter spacing
- placement zone for each text element

Default typography specs:

- Display headline: Paquito Bold, 64-92 px, no underline, no shadow unless contrast requires it, letter spacing 0
- Editorial subhead: Paquito Regular, 28-38 px, no underline, line height 1.05-1.15
- Body / points: clean sans-serif, 22-30 px, regular or semibold, line height 1.15-1.25
- Microcopy / labels: clean sans-serif, 14-20 px, regular, line height 1.1
- Page number: clean sans-serif, 16-20 px, regular
- Callout labels: clean sans-serif, 14-18 px, regular, connected with 1 px thin lines

Default effects:

- No underline.
- No italics unless a food word needs editorial emphasis.
- No heavy drop shadows.
- Use subtle shadow only when text sits on a photo and needs contrast.
- Prefer direct text on negative space over boxes.
- Use thin outline boxes only for menu-ticket details.

### Carousel Cover

Default layout:

- Small editorial line: top left
- Marcha wordmark: top right
- Big Paquito headline: placed directly in clean negative space
- Food/action visual: centered, lower half, or lower-right depending on crop
- Fine callout labels: optional, connected to ingredients with thin lines
- Subtitle: small, close to the headline or near the food
- Page number: small, bottom right

Best for:

- concept covers
- sauce covers
- food hero shots

Maximum cover copy:

- headline: 2-5 words
- subtitle: 8-14 words

Example:

```text
AI FOOD CONCEPT

NOT
KETCHUP.

Kashmiri garlic tomato chilli
for momos, fries and everything.
```

### Carousel Interior Slide

Use one of three layouts:

1. **Editorial page**
   - best for ingredient logic and product explanation

2. **Plated diagram**
   - best for ingredients, callouts, and flavour logic

3. **Image top, text bottom**
   - best for recipe steps

4. **Magazine page**
   - best for a hero food image with a short body paragraph

Rules:

- one headline
- max 3 body points
- no paragraph blocks longer than 2 lines
- keep generous margins
- no filled cards unless the concept specifically needs a menu-ticket detail
- if a box is used, use a thin outline only

### Carousel CTA Slide

Use minimal layout:

- large question in Paquito
- one supporting line
- one CTA line, not a button

Examples:

- Would you dip momos in this?
- Should this become real?
- What would you eat this with?

### Reel Text Placement

Use text overlays in fixed safe areas:

- Hook: top third
- Ingredient flashes: center
- Use-case text: lower third
- CTA: center or lower third, above app UI

Never place important text:

- very bottom
- extreme top
- near right-side Instagram buttons
- over hands, sauce streams, or hero food texture
- inside a separate box unless the whole reel uses a menu-ticket system

Reel copy length:

- hook: 3-7 words
- mid text: 2-5 words
- CTA: 3-8 words

Example reel sequence:

```text
0-2s: Not ketchup.
2-5s: Tomato + Kashmiri chilli + garlic.
5-8s: Built for momos.
8-12s: And fries. And dosa.
12-15s: Should this exist?
```

### Single Image Post

Use one of three layouts:

1. **Hero food + small title**
   - text top-left
   - food centered or lower frame

2. **Big quote / hot take**
   - text centered
   - solid brand background

3. **Mock packaging poster**
   - product centered
   - product name above
   - short line below

4. **Editorial menu page**
   - food centered
   - small text labels around the dish
   - thin callout lines
   - one small menu-style note

Single image copy:

- 1 big line
- optional 1 subtitle
- no body copy
- exception: editorial food-page posts may use one short paragraph under 45 words

Examples:

- Not Ketchup.
- Better-for-you should still taste like something.
- Indian pantry. Global format.
- Makhani Hummus.

## Font Rules

### Paquito

Use for:

- big hooks
- product names
- recipe names
- emotional editorial lines

Do not use Paquito for dense body copy.

### Sans Serif

Use Inter, DM Sans, or a clean Helvetica-style sans-serif for:

- body text
- ingredient labels
- page numbers
- tiny UI labels

## Color Rules

Use no more than 3 active colors per post.

Use one solid matte background colour per slide. Do not use dual-colour, split, half-and-half, curved-block, gradient, or multi-panel backgrounds. Different slides in the same carousel may use different brand colours.

Pillar cover background colours:

- Not Ketchup: Chilli Red `#D7382F`
- India-Available Fusion: Turmeric Yellow `#F2B544`
- Pantry To Product: Deep Teal `#0F6F78`
- Healthy But Not Sad: Cream `#FFF4D8`
- The Chutney Matrix: Ink Black `#17120F`
- One Sauce, Five Foods: Deep Teal `#0F6F78`
- Food Hero Shots: rotate one solid brand colour based on the hero food, never dual-colour.

Main combinations:

### Premium Editorial

- Background: Deep Teal `#0F6F78`
- Text: Cream `#FFF4D8`
- Accent: Chilli Red `#D7382F`

### Educational / Recipe

- Background: Cream `#FFF4D8`
- Text: Ink Black `#17120F`
- Accent: Chilli Red `#D7382F`

### Spicy / Bold

- Background: Chilli Red `#D7382F`
- Text: Cream `#FFF4D8`
- Accent: Turmeric Yellow `#F2B544`

## Copy Banks

### Strong Hooks

- Not ketchup.
- This should exist.
- Indian food does not need to stay still.
- Better-for-you should still taste like something.
- Built from the Indian pantry.
- A sauce for modern snacking.
- Would this survive the momo test?
- Chutney, but built for now.
- Familiar flavour. New format.
- Global format. Indian pantry.

### CTA Lines

- Would you try this?
- Should this become real?
- What would you eat this with?
- Momo test or dosa test?
- Would you buy this as a sauce?
- Save this food concept.
- Comment the food you would test this with.

## Image Generation Rules

Always request:

- correct aspect ratio for the target format
- no text in generated food image
- no logo
- no watermark
- faceless hands only when people appear
- hard direct flash
- crisp shadows
- matte solid background
- deep depth of field
- clean high-contrast commercial food photography

Then add Marcha typography afterward.

## Final QA Checklist

Before any asset is final:

- Is the aspect ratio correct?
- Is the first line scroll-stopping?
- Is Paquito used only where it adds premium character?
- Is body text readable?
- Are there only 3 active colors?
- Is text placed in a consistent Marcha layout?
- Is there enough negative space?
- Does it feel like a food brand, not a recipe dump?
- Is the CTA clear?
