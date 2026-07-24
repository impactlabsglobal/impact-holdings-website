# Stripe Setup For Impact Holdings LLC

The website is prepared for Stripe but does not accept card payments yet. Do not add a Stripe secret key to `index.html` or to GitHub Pages.

## Create these Stripe products and one-time prices

| Website key | Product | Price |
| --- | --- | --- |
| `w2` | W-2 Tax Return | $100.00 |
| `mileage` | W-2 + 1099 with mileage | $250.00 |
| `expenses` | W-2 + 1099 with expenses | $400.00 |
| `llc` | Complete LLC package | $300.00 |
| `extra` | Extra SSN or W-2 filing | $30.00 |

After creating them, replace each `prod_REPLACE_*` and `price_REPLACE_*` value in `index.html` with the actual Stripe Product ID and Price ID.

## Checkout implementation

Use a secure server-side endpoint to create Stripe Checkout Sessions. Send the selected service Price ID and, when applicable, the extra filing Price ID with quantity 0 to 4. The website already stores both values in the submitted request.

The endpoint must use the Stripe secret key stored as a server environment variable. GitHub Pages is static hosting, so it cannot securely create Checkout Sessions by itself. A small serverless endpoint on Cloudflare Workers, Netlify Functions, Vercel, or a similar service is required before enabling the Card checkout option.

Configure Stripe Checkout to accept card payments and enable Apple Pay and Google Pay in the Stripe Dashboard when your account is ready. Cash App Business and Zelle Business remain manual payment methods confirmed after the client request.
