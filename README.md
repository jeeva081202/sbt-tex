# S.Bakkiyalaxmi Tex – Online Saree Shop

E-commerce website for **S.Bakkiyalaxmi Tex**, handloom cotton sarees from Kasi Nagar, T.Subbulapuram, Aundipatti, Theni District, Tamil Nadu.

> **Status:** frontend preview. Payment, orders and tracking run in demo mode in the browser. A backend (database, admin panel, Razorpay) is the next step.

## Features
- Green and gold design based on the shop's banner, mobile friendly
- Tamil / English language switch
- Product grid with border, colour, price and sort filters
- Search, quick view, wishlist, recently viewed
- Product page with image gallery, zoom, PIN code delivery check, WhatsApp order
- Cart, coupon codes (`DEEPAVALI10`, `FIRST100`), gift wrap, checkout (UPI / card / net banking preview)
- Order confirmation and order tracking timeline
- Deepavali offer bar with live countdown

## Tech
Plain **HTML, CSS and JavaScript** in one `index.html`. No build step, no framework. Fonts from Google Fonts. Product photos cleaned with Python (OpenCV + Pillow).

## Run locally
Open `index.html` in a browser, or run:
```bash
python3 -m http.server 8000
```
then visit http://localhost:8000

## Edit shop settings
At the top of the `<script>` in `index.html`:
- `WHATSAPP` – shop WhatsApp number with country code, e.g. `"919876543210"`
- `OFFER_END` – Deepavali offer end date
- `COUPONS` – coupon codes
- `P` – product list (name, Tamil name, prices, photos, description)

## Deploy on GitHub Pages
Settings → Pages → Source: *Deploy from a branch* → Branch: `main` / root → Save.

## Next steps
- Backend for orders and stock (Firebase / Supabase or Node.js)
- Admin page to add sarees and see orders
- Live Razorpay payment
- Custom domain
