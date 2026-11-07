# AUREL storefront

A modern, responsive storefront for eyewear and watches. It is a lightweight static site: no build step or package installation is required.

## Preview locally

Open `index.html` in a browser, or run a local static server from the repository directory:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. GitHub will show the published site URL in the Pages settings when deployment finishes.

The homepage is `index.html` at the repository root, ready for this setup.

## Customize before launch

- Replace the sample AUREL name, product descriptions, prices and contact details in `index.html`.
- Replace the Unsplash image URLs with your own product photography.
- The cart is a front-end demo and persists in the visitor's browser. The checkout button currently shows a setup message; connect a payment and order system (such as Shopify or Stripe Checkout) before accepting orders.
- The newsletter form is a front-end interaction only. Connect it to an email marketing provider to collect subscriptions.
- Update shipping, returns, privacy and terms content to match your business.

The site uses Google Fonts and hosted Unsplash images, so those resources need an internet connection.
