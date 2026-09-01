# SRS Silks — Ecommerce Platform (v1)

An earlier snapshot of the SRS Silks ecommerce platform — see
[srs-silks](https://github.com/mynampatiasha/srs-silks) for the current,
actively-developed version with the same structure.

A full-stack ecommerce site for SRS Silks (a saree and ethnic-wear store) —
product catalog, orders, reviews, and admin management, plus a separate
Flutter billing/POS shell.

This repo contains a few stages of the same project side by side:

- **`Real_time_Application/`** — the full-stack app: React (Vite) frontend
  + Express/MongoDB backend with Cloudinary image storage
- **`demo/`** — an earlier static HTML/CSS/JS prototype (storefront +
  admin panel)
- **`srs-backend/`** — an earlier/parallel copy of the backend
- **`billing_main_shell.dart`** — a Flutter shell for a POS/billing app

## Tech stack

- **Frontend**: React (Vite)
- **Backend**: Node.js, Express 5, MongoDB (Mongoose), JWT auth, bcrypt,
  Cloudinary (via `multer-storage-cloudinary`) for product images

## Running locally

```bash
cd Real_time_Application/srs-backend
npm install
npm start
```
Requires a `.env` with `MONGO_URI`, a JWT secret, and Cloudinary credentials.

```bash
cd Real_time_Application/srs-frontend
npm install
npm run dev
```
