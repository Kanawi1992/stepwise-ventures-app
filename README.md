# Stepwise Ventures App

This package turns the supplied Stepwise Ventures order page into an installable Progressive Web App (PWA).

## Included
- Responsive storefront based on the supplied order page
- Dienqi RFID wallet listing at K50
- Quantity-based order total
- Delivery choices: Vision City and Waigani Central (free), other areas by confirmation, or arranged pickup
- Cash or bank-transfer selection
- WhatsApp order-message generation to +675 8297 2438
- Email and social links from the supplied page
- Installable Android home-screen experience
- Basic offline caching after the first successful visit

## Publish as a website
Upload the **contents** of this folder to a static HTTPS host. Examples include GitHub Pages, Netlify, or Cloudflare Pages. Keep `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons` folder together at the same site path.

Service workers and PWA installation require HTTPS (localhost is suitable for testing). After publishing:
1. Open the site in Chrome on Android.
2. Allow the page to finish loading once while online.
3. Use the browser menu → **Install app** or **Add to Home screen**.
4. Launch the Stepwise Ventures icon from the phone's home screen.

## Important operational notes
- WhatsApp orders are customer-submitted messages; this package does not automatically send messages.
- The supplied page intentionally does not expose bank account numbers. Bank details remain shared directly after the business confirms an order.
- This is a static storefront/PWA, not a cloud-backed order-management system. It does not yet store orders in a business dashboard, process card payments, or synchronize inventory.
- The product and business details were retained from the supplied page. Confirm stock, pricing, delivery policy, and contact details before public launch.

## Android native APK
This PWA can be installed directly on Android without an APK. A separately signed native APK/AAB requires an Android build environment and signing credentials; those are not included in this source package.
