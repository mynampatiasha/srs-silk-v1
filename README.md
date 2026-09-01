# 🥻 SRS Silks — Ecommerce Platform (v1)

`React (Vite)` `Node.js` `Express` `MongoDB` `Cloudinary` `Flutter`

> An earlier snapshot — see [srs-silks](https://github.com/mynampatiasha/srs-silks) for the current version.

## What is this?

A full-stack ecommerce site for SRS Silks (a saree and ethnic-wear store) —
product catalog, orders, reviews, and admin management. Same structure as
the current [srs-silks](https://github.com/mynampatiasha/srs-silks) repo.

| Folder | What it is |
|---|---|
| `Real_time_Application/` | Full-stack app — React (Vite) + Express/MongoDB + Cloudinary |
| `demo/` | Earlier static HTML/CSS/JS prototype |
| `srs-backend/` | Earlier/parallel backend copy |

## 🛠️ Tech Stack

- **Frontend**: React (Vite)
- **Backend**: Node.js, Express 5, MongoDB (Mongoose), JWT auth, bcrypt, Cloudinary

## ⚠️ Stray file

`billing_main_shell.dart` at the repo root is **not part of this project** —
its imports match the [abra-finance-app](https://github.com/mynampatiasha/abra-finance-app)
codebase (ERP/invoicing/finance features), and its relative import paths
point to a folder structure that doesn't exist here. Looks accidentally
committed, not wired into or runnable as part of SRS Silks.

## 🚀 Running Locally

```bash
cd Real_time_Application/srs-backend
npm install
npm start
```

```bash
cd Real_time_Application/srs-frontend
npm install
npm run dev
```

## 🔒 Security

Requires a `.env` with `MONGO_URI`, a JWT secret, and Cloudinary credentials.
