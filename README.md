# 🛒 MERN Ecommerce Website

This is a full-stack e-commerce web application built using the MERN stack (MongoDB, Express, React, Node.js). It also integrates **Cloudinary** for image uploads and **Razorpay** for payment processing.

---

## 🔗 Live Demo

🚀 *Coming soon* (Deploy on Vercel + Render or any of your choice)

---

## 🧩 Features

### 1️⃣ User Features
- ✅ Register/Login with JWT authentication
- 👕 Browse products by categories/subcategories
- 🛒 Add to cart
- 💳 Place orders with Razorpay
- 📦 View past orders

### 2️⃣ Admin Panel (`/admin`)
- 🔐 Admin Login with protected route (env configured credentials)
- 📦 Add new products with multiple image uploads via Cloudinary
- 📃 View all products
- 📬 View all orders
- 🔄 Auto token-based session management

---

## 🛠 Tech Stack

### Frontend
- React.js
- React Router
- Axios
- Tailwind CSS
- React Toastify

### Backend
- Node.js
- Express.js
- MongoDB (via Mongoose)
- Cloudinary (image hosting)
- Razorpay (payment integration)
- JWT (admin authentication)

---

## 🖼 Screenshots

> 📸 Add screenshots here after running locally.

---

## ⚙️ How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/safak/youtube.git
cd youtube
git checkout mern-ecommerce-app
```

### 2. Set up backend

```bash
cd backend
npm install
```

#### ➕ Create a `.env` file in `backend` with the following:

```env
PORT=4000
JWT_SECRET=greatstack
ADMIN_EMAIL=admin@example.com
ADMIN_PASSWORD=greatstack123
MONGODB_URI=your_mongodb_connection_string
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_SECRET_KEY=your_secret
```

```bash
npm start
```

### 3. Set up frontend

There are **two frontend apps**:

#### 🛍️ Customer frontend

```bash
cd frontend
npm install
```

Create `.env` in `frontend`:

```env
VITE_BACKEND_URL=http://localhost:4000
```

```bash
npm run dev
```

Visit `http://localhost:5173`

---

#### 🔐 Admin Panel

```bash
cd admin
npm install
```

Create `.env` in `admin`:

```env
VITE_BACKEND_URL=http://localhost:4000
```

```bash
npm run dev
```

Visit `http://localhost:5174` (or whatever port is shown)

---

## 💳 Payment Integration

- Razorpay is used for payment processing on the frontend (Checkout).
- No Firebase or Stripe is used in this project.

---

## ☁️ Image Uploads

- Admin panel uses **Cloudinary** to upload product images via API.
- Images are previewed before upload using `URL.createObjectURL`.

---

## 🧪 Extra Improvements

- [ ] Add validation and error boundaries
- [ ] Add filtering and search
- [ ] Add user profile page
- [ ] Add delivery address and shipping logic

---

## 🤝 Contributing

PRs welcome. Fork and raise a pull request 🚀


