# WattSwap Store Mock-up

A static, responsive concept storefront for the WattSwap home-energy system. It presents WattSwap as a premium OffGrid Pro product and demonstrates a purchase flow combining a one-time hardware charge with a recurring subscription.

## What is included

- Apple-inspired product-launch landing page
- OffGrid Pro-inspired colour palette and visual treatment
- Two selectable subscription tiers
- Monthly and annual billing options
- One-time WattSwap hardware charge
- Interactive basket drawer
- Responsive desktop and mobile layouts
- Concept render of the 10-inch WattSwap touchscreen

## Run locally

No build tools or dependencies are required. Download the files and open `index.html` in a browser.

For a local web server, run this command from the project folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `wattswap-hub.png`, and this `README.md` to the repository root.
3. Open the repository's **Settings**.
4. Select **Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Choose the `main` branch and `/ (root)` folder, then save.

GitHub will provide the public Pages URL after deployment completes.

## Editing plans and prices

Each plan is an `<article class="plan">` in `index.html`. Its recurring and hardware prices are stored in these attributes:

```html
data-monthly="19.99" data-hardware="499"
```

Update the visible price text in the same plan card when changing these values.

## Shopify integration note

This package is an interactive front-end mock-up, not a completed Shopify theme or payment integration. The basket and checkout button demonstrate the intended customer journey but do not take payment.

For production, the design can be rebuilt as Shopify Liquid sections and connected to Shopify products, a subscription app, Shopify Payments, delivery rules, taxes, customer accounts, and the final WattSwap terms.

## Concept disclaimer

Plan names, prices, product details, and the hardware render are illustrative and should be replaced with the final approved WattSwap information before launch.
