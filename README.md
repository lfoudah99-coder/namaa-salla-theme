# NAMAA Salla theme (نَماء)

Salla Twilight theme for the NAMAA store. Built on Salla's official Raed theme, so the product pages, cart, checkout and payment are Salla's own. NAMAA's look (colours, fonts, illustrations and homepage sections) is added on top.

## What was added
| File | Purpose |
| --- | --- |
| `public/namaa.css` | NAMAA colours, fonts and section styles. Plain CSS, loaded after the theme's own styles. Copy kept in `src/assets/styles/namaa.css`. |
| `src/views/layouts/master.twig` | Loads Google Fonts (El Messiri, Readex Pro, Lexend) and `namaa.css`. |
| `src/views/components/home/namaa-*.twig` | Six homepage sections: hero, products with add to cart, statement, collections, learn through play, why NAMAA. |
| `src/views/pages/partials/namaa-symbol.twig` | The seed and leaf symbol. |
| `public/images/namaa/` | Watercolour illustrations, box photos and the logo SVG. |
| `twilight.json` | Theme name and the six NAMAA sections with their editable fields. |

The original Raed readme is kept as `README-raed.md`. Raed is MIT licensed by Salla.

## Connect to Salla
1. Create a Salla Partners account at https://salla.partners and connect your GitHub account.
2. Push this folder to a new GitHub repository (for example `namaa-salla-theme`) and put its link in `twilight.json` under `repository`.
3. In the Partners Portal: My Themes > Create theme > import from GitHub, then choose this repository.
4. Preview it on a demo store, then send an installation request to your live store (private theme).
5. In your store dashboard: Store design > choose the NAMAA theme > Customise. Arrange the NAMAA sections and pick the products for "نماء: المنتجات مع زر السلة".

## If you rebuild the theme assets
`public/` already contains the built files, so no build is needed. If you later run `pnpm install` and `pnpm run production`, `namaa.css` and the images are untouched by the build because they live directly in `public/`.
