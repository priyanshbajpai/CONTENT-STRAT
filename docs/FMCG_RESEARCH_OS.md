# FMCG Research OS

Use this as the standard workflow for researching any FMCG brand, product category, ingredient, or launch idea in the Codex chat.

## Research Modes

### 1. Category Scan

Use when exploring a market/category.

Outputs:
- Category definition
- Consumer jobs-to-be-done
- Price and pack-size hypotheses
- Competitor buckets
- White-space opportunities
- Risks and constraints

Good prompts:
- `Research the Indian market for premium tomato sauces.`
- `Map white space for millet snacks in urban India.`
- `Compare Indian vs global fusion condiment opportunities.`

### 2. Product Concept Lab

Use when creating new FMCG product ideas.

Model roles:
- Epicure: ingredient pairings, substitutions, cuisine shifts
- RecipeBERT: plausibility and similarity scoring
- T5 recipe generation: rough prototype directions

Outputs:
- Concept names
- Ingredient stack
- Sensory profile
- Target consumer
- Use cases
- Positioning
- Watchouts
- Tasting panel hypotheses

### 3. Variant Architecture

Use when building a line, not just one product.

Outputs:
- Hero SKU
- Mass SKU
- Premium SKU
- Youth/fusion SKU
- Regional SKU
- Limited edition SKU
- Portfolio logic

Example:
- Tomato Tadka Sauce
- Tomato Pizza Masala Sauce
- Indo-Asian Tomato Chili Drizzle
- Tomato Mustard Seed Chutney Sauce
- Tomato Umami Mushroom Glaze

### 4. Formulation Direction

Use when moving from idea to prototype.

Outputs:
- Ingredient families
- Approximate functional roles
- Flavour balance
- Texture target
- Heat/acidity/sweetness/salt notes
- Stability and manufacturing questions

Guardrail:
This is R&D direction, not a final certified formula.

### 5. Brand Positioning

Use when turning concepts into a brand.

Outputs:
- Brand thesis
- Audience
- Positioning statement
- Naming territories
- Packaging cues
- Tone of voice
- Claim hierarchy
- Launch narrative

### 6. Content Strategy

Use when planning marketing.

Outputs:
- Content pillars
- Reel/TikTok ideas
- Product education hooks
- Founder POV
- Retail/shopper content
- Creator briefing notes
- Campaign calendar

### 7. Validation Plan

Use before committing to a product.

Outputs:
- Consumer test plan
- Tasting panel questions
- Concept test questions
- Price sensitivity hypotheses
- Retail feedback checklist
- QSR/HoReCa trial script

## Standard Output Template

For any FMCG research request, prefer this structure:

1. Category/brief interpretation
2. Model signals, if used
3. Top opportunities
4. Product concepts or variants
5. Positioning and use cases
6. Risks and validation questions
7. Next recommended experiment

## FMCG Lens For India

Always consider:
- Vegetarian acceptability
- Spice tolerance bands
- Regional food habits
- Price sensitivity
- Pack-size realism
- Modern trade vs quick commerce vs kirana
- QSR/HoReCa use cases
- Regulatory and claim risk
- Shelf stability
- Local ingredient supply
- Familiarity vs novelty balance

## How To Use The Chat

Ask naturally. Examples:

- `Use the models to create 10 sauce variants around tomato for Indian Gen Z.`
- `Find ingredient substitutes for a premium sauce that reduce cost but preserve flavour.`
- `Build a 3-SKU launch architecture for an Indian fusion condiment brand.`
- `Create a content strategy for this product line.`
- `Turn these 5 concepts into a retailer pitch.`
- `Make this idea more mass-market.`
- `Make this idea more premium/global.`
