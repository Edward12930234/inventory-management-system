# React Inventory Management System

A MERN-based inventory management application for tracking products, stores, purchases, and sales.

## Tech Stack

**Frontend:** React 18, React Router, Tailwind CSS, Headless UI, Heroicons, ApexCharts, Chart.js

**Backend:** Node.js, Express, MongoDB (Mongoose), Multer, CORS

## Features

- User registration & login
- Manage products (add / update / delete)
- Manage stores
- Record purchases and track purchase stock
- Record sales and track sold stock
- Dashboard with charts for sales/purchase analytics
- Image upload for products

## Project Structure

```
React-Inventory-Management-System/
├── Backend/
│   ├── controller/      # Route handlers (product, store, purchase, sales, stock)
│   ├── models/          # Mongoose schemas (product, store, purchase, sales, users)
│   ├── router/          # Express routers
│   └── server.js        # App entry, runs on port 4000
└── Frontend/
    ├── public/
    └── src/
        ├── components/  # AddProduct, AddStore, AddSale, Header, SideMenu, Layout, etc.
        ├── pages/       # Dashboard, Inventory, Sales, PurchaseDetails, Store, Login, Register
        ├── AuthContext.js
        └── App.js
```

## API Endpoints

- `POST /api/login` — user login
- `GET  /api/login` — current logged-in user
- `POST /api/register` — register new user
- `/api/store` — store CRUD
- `/api/product` — product CRUD
- `/api/purchase` — purchase records
- `/api/sales` — sales records

## Getting Started

### Backend

```bash
cd Backend
npm install
npm run serverStart
```

Server runs on `http://localhost:4000`. Configure the MongoDB connection in [Backend/models/index.js](Backend/models/index.js).

### Frontend

```bash
cd Frontend
npm install
npm start
```

App runs on `http://localhost:3000`.
