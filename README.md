# AUREL storefront

A responsive static storefront for eyewear and watches, configured to deploy as Cloudflare Worker static assets.

## Preview locally

Open `public/index.html` in a browser, or run a local static server from the repository directory:

```sh
python3 -m http.server 8000 --directory public
```

Then visit `http://localhost:8000`.

## Connect the existing Cloudflare Worker to GitHub

The Worker is named `personal-repo`, matching `wrangler.jsonc`.

1. In Cloudflare, open **Workers & Pages → personal-repo → Settings → Builds**.
2. Connect the GitHub repository `syedtahirmehboob0-glitch/personal-repo`.
3. Select branch `main` and repository root `/`.
4. Leave the build command blank and use deploy command `npx wrangler deploy`.
5. Save and check the resulting build under the Worker’s Deployments page.

Cloudflare Workers Builds deploys from the connected Git repository on each push. The Worker name must match the `name` in Wrangler configuration. Official setup: [Connect an existing Worker](https://developers.cloudflare.com/workers/ci-cd/builds/) and [Workers Builds configuration](https://developers.cloudflare.com/workers/ci-cd/builds/configuration/).

## Before accepting real orders

- AUREL is a sample brand name and is already used by an eyewear seller. Check a replacement name before launch.
- Replace sample products, prices, product images, and business contact details with verified information.
- The cart is a browser-side demo. Checkout does not accept orders or payments until a commerce/payment provider is connected.
- Newsletter signup is a front-end demo and does not store email addresses.
- Confirm shipping, returns, privacy and terms content for your actual business.
- The page currently uses USD prices and hosted Google Fonts/Unsplash images.

