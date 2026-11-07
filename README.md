# Rue Lumière storefront

A responsive English-language storefront for eyewear and watches, configured to deploy as Cloudflare Worker static assets.

## Preview locally

Open `public/index.html` in a browser, or run a static server from this directory:

```sh
python3 -m http.server 8000 --directory public
```

Then visit `http://localhost:8000`.

## Deploy

The Worker is named `personal-repo`, matching `wrangler.jsonc`. In Cloudflare, connect the GitHub repository `syedtahirmehboob0-glitch/personal-repo` under **Workers & Pages → personal-repo → Settings → Builds**, select `main`, leave the build command blank, and use `npx wrangler deploy` as the deploy command. A push to `main` will deploy if the Cloudflare build connection is active.

## Brand

Rue Lumière is a Paris-inspired working name. It has not been cleared for trademark, company registration, domain or social-handle availability.

## Before accepting orders

- The customer WhatsApp number is configured in the `orderWhatsapp` constant in `public/index.html` (Pakistan format: 92 plus 10 digits). Update it if you change the business number.
- Confirm the Markaz reseller account, reseller cost and payout terms. Displayed shop prices are suggested retail prices and have not been margin-checked against account-specific reseller pricing.
- The order form prepares an order request in WhatsApp; it does not process payment or create a supplier order automatically. Confirm stock, final total, delivery charge, address and return terms with the customer, then place/track the order through the supplier.
- Supplier product availability, prices, shipping estimates and return eligibility can change. The site asks the customer to confirm these details before dispatch.
- The site does not store order details. Customers submit them directly to WhatsApp after choosing to send the prefilled message.
- Newsletter signup and online card payments are not offered.
