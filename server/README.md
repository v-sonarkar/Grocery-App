# Grocery App Server

Express + MongoDB backend for the Grocery App.

## Prerequisites

- Node.js 18+
- npm
- MongoDB connection string
- Cloudinary account
- Stripe account (for checkout/webhook features)

## Setup

1. Install dependencies:

```bash
npm install
```

2. Create a `.env` file in `server/` and add the following variables:

```env
PORT=4000
CLIENT_URL=http://localhost:5173
NODE_ENV=development

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

SELLER_EMAIL=your_seller_login_email
SELLER_PASSWORD=your_seller_login_password

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
```

## Run

Start in development mode (with auto-reload):

```bash
npm run server
```

Start in production mode:

```bash
npm start
```

Server runs at:

- `http://localhost:4000` (or `PORT` in `.env`)

## Health Check

- `GET /` returns `API is Working`

## Notes

- CORS allows `CLIENT_URL` plus local dev origins in `server.js`.
- Stripe webhook endpoint is `POST /stripe`.
