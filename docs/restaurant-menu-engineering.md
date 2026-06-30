# restaurant-menu-engineering
> Engineer a more profitable, more appealing menu — analysis, psychology, pricing, copy, and layout.

## Description
A menu consultant in a skill: it runs the classic menu-engineering matrix (popularity × profitability → Stars / Plowhorses / Puzzles / Dogs), then applies evidence-based psychology, pricing strategy, item-description copywriting, layout, and accurate dietary/allergen labeling to lift your average check and margin. Works from your menu and (ideally) item cost + sales data. Honest by design — no fake scarcity, no misleading sourcing claims, no fabricated numbers.

## Compatibility
Advisory skill — no tooling or runtime required. Works from your menu and (ideally) item cost + sales data. Dietary/allergen guidance is a framework, **not legal compliance** — verify labels against your actual recipes and local law.

## Keywords
menu engineering, restaurant menu design, menu psychology, menu pricing strategy, food cost, contribution margin, menu item descriptions, menu copywriting, restaurant profitability, Stars Plowhorses Puzzles Dogs, price anchoring, menu layout, dietary labeling, allergen menu, average check, F&B, hospitality

## Sample input
> "Here are 6 dishes with their food cost, menu price, and last month's sales counts. Tell me which to feature, reprice, or cut — and rewrite the two weakest descriptions."

## Sample output
*(Illustrative shape.)*
- **Engineering matrix:** each item placed by contribution margin (price − food cost) × menu-mix % → e.g. the short rib is a **Star** (feature it), the pasta is a **Plowhorse** (popular but thin margin → trim cost or nudge price, don't cut it), the branzino is a **Puzzle** (high margin, low sales → promote/reposition/rename), the side salad is a **Dog** (rework or remove).
- **Description rewrite:** "Chicken Salad" → a sensory, honest rewrite (no invented "wild" or "organic" claims).
- **Pricing/layout:** food-cost-% and margin reasoning + where to place the high-margin items, with honest framing (no fake "only 2 left").
- **Dietary flag:** which items need verified allergen/dietary labels — with the reminder to confirm against your recipes and local law.

## Known limitations
- **Advisory only** — it doesn't connect to your POS; you supply the menu + (ideally) item cost and sales counts. If you don't have the numbers, it asks rather than inventing them.
- **No deception** — it refuses fake scarcity, misleading sourcing ("wild-caught" on farmed fish), and unsupported health claims.
- **Dietary/allergen guidance is not legal compliance or certification** — labels must reflect your actual recipe/prep and your local law; mislabeling can seriously harm guests. Verify with your local food-safety regulator.
- Psychology effects (charm pricing, etc.) are real but modest and context-dependent — it frames them as tendencies, not guarantees, and treats the "golden triangle" eye-zone claim as the myth it is.
