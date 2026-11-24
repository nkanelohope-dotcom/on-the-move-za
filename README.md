# On The Move ZA – Website + Professional Admin

Live-connected website and admin panel for On The Move ZA.

## How it works

1. Admin logs into `/admin` and manages services, prices, images, settings
2. Changes are saved immediately
3. The public website loads data from the API — visitors always see the latest content

## Quick start

```bash
cd backend
npm install
PORT=3000 npm start
```

| Page | URL |
|------|-----|
| Website | http://localhost:3000 |
| Admin | http://localhost:3000/admin |

**Login:** `admin` / `otmza2026`  
(Change in `backend/.env`)

## Admin features

- **Services** – add / edit / delete with image upload, description, features list, category, starting price
- **Pricing** – full price tables linked to each service  
- **Gallery** – upload & delete photos/videos
- **Settings** – phone, email, socials, service areas, call-out fee note

## Seeded services (including your flyer)

- Standard Cleaning
- Deep Cleaning  
- Spring Cleaning
- **Pre & Post Event Cleaning** (10–30 / 40–60 / 70+ guests pricing)
- Packing & Moving

## Structure

```
otmza-full/
├── website/       Public site (loads live data via js/live-data.js)
├── backend/       API + Admin dashboard
│   ├── data/      JSON database (db.json)
│   ├── public/    Admin UI
│   ├── uploads/   Service & gallery images
│   └── server.js
└── README.md
```
