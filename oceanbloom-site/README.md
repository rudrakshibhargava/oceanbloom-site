# oceanbloom

A single-page storefront for beach accessories — bags, crochet bags, jewelry, dresses, hair accessories, and charms.

## What's included

- Product catalog with category filters
- Shopping cart (add, adjust quantity, remove)
- Checkout with shipping details and payment method selection (Cash on Delivery, Net Banking, UPI)
- Order confirmation flow
- Fully responsive layout

## Running locally

This is a single static HTML file with no build step or dependencies. Just open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying

### GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under "Build and deployment," set **Source** to "Deploy from a branch," pick the `main` branch and `/ (root)` folder.
4. Save — your site will be live at `https://<username>.github.io/<repo-name>/`.

### Any static host
Upload `index.html` to Netlify, Vercel, Cloudflare Pages, or any static file host — no build configuration needed.

## Notes

- Cart and order data are held in memory for the current browser session only (no backend or database yet).
- To accept real online payments (net banking, UPI, cards), connect a payment gateway such as Razorpay or PayU on a backend — the current checkout flow is UI-only and does not process real transactions.
