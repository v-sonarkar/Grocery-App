
# Grocery_APP

A full-stack grocery shopping application with separate frontend (React) and backend (Node.js/Express) codebases. This app allows users to browse products, manage their cart, place orders, and sellers to manage their inventory.

## Folder Structure

```
Grocery_APP/
│
├── client/   # React frontend
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       │   └── seller/           # Seller-specific components
│       ├── context/
│       ├── pages/
│       │   └── seller/           # Seller-specific pages
│       ├── App.jsx
│       ├── main.jsx
│       └── ...
│   ├── package.json
│   └── ...
│
├── server/   # Node.js/Express backend
│   ├── configs/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   ├── package.json
│   └── ...
│
└── RESUME.md # Project summary
```

## Features

## Notes on Folder Structure

- The `components/` folder contains reusable UI components, including a `seller/` subfolder for seller-specific components.
- The `pages/` folder contains main application pages, with a `seller/` subfolder for seller dashboard pages.

Example:

```
client/
   src/
      components/
         Navbar.jsx
         Footer.jsx
         ProductCard.jsx
         BestSeller.jsx
         BottomBanner.jsx
         Categories.jsx
         Loading.jsx
         Login.jsx
         MainBanner.jsx
         NewsLetter.jsx
         seller/
            SellerLogin.jsx
      pages/
         Home.jsx
         Cart.jsx
         AllProducts.jsx
         MyOrders.jsx
         AddAddress.jsx
         ProductCategory.jsx
         ProductDetails.jsx
         seller/
            AddProduct.jsx
            Orders.jsx
            ProductList.jsx
            SellerLayout.jsx
```
- User authentication (users & sellers)
- Product browsing, categories, and details
- Shopping cart and order management
- Address management
- Seller dashboard (add products, view orders)
- Image upload (Cloudinary)

## Technologies
- **Frontend:** React, Vite, CSS
- **Backend:** Node.js, Express, MongoDB (Mongoose)
- **Other:** Cloudinary, Multer, Vercel

## Getting Started

### Prerequisites
- Node.js and npm installed
- MongoDB instance (local or cloud)

### Setup
1. Clone the repository
2. Install dependencies in both `client` and `server` folders:
   - `npm install` (in each folder)
3. Configure environment variables (e.g., MongoDB URI, Cloudinary keys) in the server
4. Start the backend server:
   - `node server.js` (from `server` folder)
5. Start the frontend:
   - `npm run dev` (from `client` folder)

## Deployment
- The app is ready for deployment on Vercel (frontend) and can be adapted for other platforms.

## License
MIT

---
For more details, see the RESUME.md and the README files in each subfolder.
