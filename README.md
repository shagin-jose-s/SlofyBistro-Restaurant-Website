# SlofyBistro — Restaurant Website Template

Responsive React + Vite + Tailwind CSS v4 restaurant website with Framer Motion animations and an optional Express backend.

## Colour palette
- Burgundy `#722F37`
- Cream `#F8F4E7`
- Dusty pink `#D7A7B1`

## Frontend
Requires Node.js 20.19+ or 22.12+.
```bash
npm install
cp .env.example .env
npm run dev
```
Visit http://localhost:5173. Production build: `npm run build`.

## Optional backend (not required to preview the website)
```bash
cd backend
npm install
cp .env.example .env
npm run dev
```
API health: http://localhost:5000/api/health

Endpoints:
- `GET /api/health`
- `GET /api/menu`
- `POST /api/reservations`
- `POST /api/newsletter`
- `POST /api/contact`

The backend stores demo records in JSON files under `backend/data`. It requires no database for local testing. For production, replace JSON storage with MySQL/PostgreSQL, add authentication for admin access, configure HTTPS, persistent storage, backups and a real email provider. Never expose private customer records through public API routes.

## Customize
- Menu names, categories, prices and gallery images: `src/data.js`
- Contact info, opening hours, reviews and content: `src/App.jsx`
- Palette and responsive styling: `src/style.css`
- API URL: `.env` (`VITE_API_URL`)
- Backend allowed frontend origin: `backend/.env` (`CLIENT_ORIGIN`)

Images are loaded from Unsplash; replace with your own licensed restaurant photography before selling or publishing. Contact details, menu prices and reviews are sample placeholders.
