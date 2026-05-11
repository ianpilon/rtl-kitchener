# Asset slots

Save real images at the paths below. Until a file exists, the page falls back
to a `placehold.co` placeholder automatically.

| File path                     | Used for                       | Target size (px) | Notes                              |
| ----------------------------- | ------------------------------ | ---------------- | ---------------------------------- |
| `assets/logo.png`             | Header logo (navy nav)         | 200 × 40         | Transparent PNG, light-on-dark OK  |
| `assets/logo-dark.png`        | Footer logo (dark navy bg)     | 200 × 40         | Light/white version of the logo    |
| `assets/hero.jpg`             | Hero background                | 1600 × 500       | Wide truck/trailer hero shot       |
| `assets/owner.png`            | Jeff Carson cutout (hero)      | 280 × 380        | Transparent PNG works best         |
| `assets/shop-exterior.jpg`    | Gallery main photo             | 600 × 300        | Shop exterior or signage           |
| `assets/gallery-1.jpg`        | Gallery thumbnail 1            | 150 × 60         |                                    |
| `assets/gallery-2.jpg`        | Gallery thumbnail 2            | 150 × 60         |                                    |
| `assets/gallery-3.jpg`        | Gallery thumbnail 3            | 150 × 60         |                                    |
| `assets/gallery-4.jpg`        | Gallery thumbnail 4            | 150 × 60         |                                    |
| `assets/parts-promo.jpg`      | Parts & accessories promo card | 600 × 420        | Tall card on the testimonials row  |
| `assets/parts/belts.jpg`      | Parts page: Drive Belts        | 500 × 300        | 5:3 ratio, object-fit cover         |
| `assets/parts/door-seals.jpg` | Parts page: Door Seals         | 500 × 300        | 5:3 ratio                          |
| `assets/parts/filters.jpg`    | Parts page: Filters            | 500 × 300        | 5:3 ratio                          |
| `assets/parts/refrigerant.jpg`| Parts page: Refrigerant        | 500 × 300        | 5:3 ratio                          |
| `assets/parts/sensors.jpg`    | Parts page: Sensors            | 500 × 300        | 5:3 ratio                          |
| `assets/parts/brakes.jpg`     | Parts page: Brakes             | 500 × 300        | 5:3 ratio                          |

Sizes are targets — anything in roughly the same aspect ratio will look fine
because each `<img>` is constrained by CSS.

When a parts image file is missing, the gray block stays as a placeholder
(`onerror` hides the broken `<img>` so only the slot's gray bg shows).
