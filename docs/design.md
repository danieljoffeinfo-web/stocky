# Stocky design direction

## Brief
A desktop-first operations workspace for a single wholesaler, spanning stock, purchasing, sales, relationships and full-accounting concepts. Static HTML/CSS/vanilla JS only. One initial warehouse, with future multi-location support treated as production scope.

## Reference lock
Primary foundation: Brex's precision-engineered toolkit, white/soft-gray surfaces, restrained borders, orange only for actions and selection. Borrow Beau's compact geometric sans-serif hierarchy. Ramp reviewed but rejected as the main direction: a dark full-page financial workspace would reduce clarity for dense inventory tables. Dark navigation provides a stable frame; content stays bright.

| Decision | Source | Role | Reason |
|---|---|---|---|
| White canvas, thin gray rules, 12px panels | Brex style 7471a4ea-ab61-4281-8f19-2d65352efc44 | Content hierarchy | Dense business data remains readable |
| Orange primary buttons, no decorative gradient | Brex | Actions only | Make the next action obvious |
| Compact sans-serif typography | Beau style 522a3200-2712-4008-9d2f-02b584c2eaea | UI text | Quiet, precise numeric tables |
| Grouped sidebar, status tabs and search | Shopify screen dc0a9649-d270-4617-b686-6ebc5db4bf50 | Navigation / product management | Familiar operational workflows |
| Product details alongside focused forms | Mangomint screen 329c26c8-3a76-4f47-b6f9-5b06a0be92d1 | Progressive detail | Keep tables manageable |
| Supplier → product → quantities → review | Programa flow 13438 | Document creation | Clear sequence and visible totals |
| Stock on hand / reserved / available | User scope + inventory workflow | Stock integrity | Avoid double deductions |
| Carton → inner → individual | User requirement | Packaging hierarchy | Normalise stock to base units |

Typography uses system sans-serif for offline portability. Color adaptations ensure readable small text. Muted semantic status colors and chart marks are for data only. No external fonts, assets, APIs or network dependencies. Product icons deliberately serve as catalogue placeholders; five photo slots accept real product images.

## Verification target
Desktop 1440×1000; mobile 390×844. Check dashboard/table hierarchy, modal focus, scroll containment, navigation, readable figures, and responsive table overflow. Preserve white content, charcoal navigation, orange actions, compact type and purposeful data density.
