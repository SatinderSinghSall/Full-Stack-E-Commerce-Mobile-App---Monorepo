# 📱 Full-Stack E-Commerce Mobile Application

## 📌 Overview

This project is a **Full-Stack E-Commerce Mobile Application** built using **React Native (Expo)** for the client and **Node.js + Express + MongoDB** for the backend. The application enables users to browse products, manage carts, place orders, and securely complete payments, while administrators can manage products and orders.

The system follows a **modern mobile-first architecture**, incorporating scalable backend design, secure authentication, and modular UI components.

This project demonstrates real-world implementation of:

- Mobile application development
- RESTful API design
- Authentication & authorization
- Cloud media storage
- Payment integration
- State management
- Admin dashboard functionality

---

## 🎯 Objectives

The main objectives of this project include:

- Designing a scalable mobile commerce platform
- Implementing secure user authentication & authorization
- Developing an intuitive mobile shopping experience
- Creating an admin interface for store management
- Integrating payment processing and order tracking
- Applying modern development best practices

---

## 🏗️ System Architecture

The application follows a **client–server architecture**:

```
Mobile App (React Native + Expo)
            │
            │ REST API
            ▼
Backend Server (Node.js + Express)
            │
            ▼
MongoDB Database + Cloudinary Storage
```

### Architecture Highlights

- **Client:** Mobile UI & state management
- **Server:** API, business logic & security
- **Database:** Persistent data storage
- **Cloudinary:** Image storage & delivery

---

## 🧰 Technology Stack

### 📱 Frontend (Mobile App)

- React Native (Expo)
- TypeScript
- Expo Router (File-based navigation)
- NativeWind (Tailwind CSS for RN)
- Context API (State Management)
- Clerk Authentication
- Axios / Fetch API

### 🌐 Backend (Server)

- Node.js
- Express.js
- TypeScript
- MongoDB & Mongoose
- JWT Authentication
- Multer (File Upload)
- Cloudinary (Image Hosting)
- Payment Integration (Stripe/Razorpay ready)
- Webhooks support

### 🛠 Development Tools

- Expo CLI
- ESLint & TypeScript
- Vercel Deployment (Server)
- Android Studio (Emulator)

---

## 📂 Project Structure

### Root Directory

```
client/     → React Native mobile application
server/     → Express backend API
doc/        → Documentation
```

---

## 📱 Mobile Application Structure (`client/`)

### Key Directories

#### `app/`

Contains screen routes using Expo Router.

- `(auth)/` → Authentication screens
- `(tabs)/` → Main tab navigation screens
- `product/` → Product details
- `orders/` → Order history & details
- `checkout.tsx` → Checkout flow
- `admin/` → Admin management screens

#### `components/`

Reusable UI components:

- ProductCard
- CartItem
- Header
- ConfirmModal
- CategoryItem

#### `context/`

Global state management:

- CartContext
- WishlistContext

#### `constants/`

API URLs, types, shared constants.

#### `assets/`

Images, icons, and static resources.

---

## 🖥️ Backend Structure (`server/`)

### `config/`

- Database connection
- Cloudinary configuration

### `controllers/`

Handles application logic:

- Products
- Orders
- Cart
- Wishlist
- Admin operations
- Payments & webhooks

### `models/`

MongoDB schemas:

- User
- Product
- Order
- Cart
- Wishlist
- Address

### `routes/`

REST API endpoints for all modules.

### `middleware/`

- Authentication & authorization
- File upload handling

### `scripts/`

- Seed products
- Create admin user

---

## 🔐 Authentication & Security

The application implements secure authentication:

- Clerk-based user authentication
- JWT token validation on server
- Protected admin routes
- Secure payment verification
- Middleware-based authorization

---

## 🛒 Features

### 👤 User Features

✔ User registration & login
✔ Browse products & categories
✔ Product search & details
✔ Add/remove cart items
✔ Wishlist management
✔ Address management
✔ Secure checkout
✔ Order tracking & history

### 🛍️ Shopping Experience

✔ Smooth mobile UI/UX
✔ Product images & descriptions
✔ Quantity management
✔ Real-time cart updates

### 💳 Payment & Orders

✔ Secure payment processing
✔ Order confirmation & storage
✔ Payment webhooks support

### 🛠️ Admin Features

✔ Add/edit/delete products
✔ Manage orders
✔ Admin dashboard access
✔ Inventory management

---

## 🌐 API Endpoints Overview

### Products

```
GET    /api/products
GET    /api/products/:id
POST   /api/admin/products
PUT    /api/admin/products/:id
DELETE /api/admin/products/:id
```

### Cart & Wishlist

```
GET    /api/cart
POST   /api/cart
DELETE /api/cart/:id
```

### Orders

```
POST   /api/orders
GET    /api/orders
GET    /api/orders/:id
```

### Addresses

```
GET    /api/address
POST   /api/address
```

---

## ⚙️ Installation & Setup

### 🔹 1. Clone Repository

```bash
git clone https://github.com/yourusername/ecommerce-app.git
cd ecommerce-app
```

---

### 🔹 2. Setup Backend

```bash
cd server
npm install
```

Create `.env` file:

```
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret
CLOUDINARY_NAME=your_cloud_name
CLOUDINARY_KEY=your_key
CLOUDINARY_SECRET=your_secret
PAYMENT_SECRET=your_payment_secret
```

Run server:

```bash
npm run dev
```

---

### 🔹 3. Setup Mobile App

```bash
cd client
npm install
```

Start Expo:

```bash
npx expo start
```

Run on device/emulator:

- Press **a** → Android
- Scan QR → Physical device

---

## 🧪 Seeding & Admin Setup

Create admin user:

```bash
npm run makeAdmin
```

Seed sample products:

```bash
npm run seedProducts
```

---

## 📊 Database Design

### Collections

- Users
- Products
- Orders
- Cart
- Wishlist
- Addresses

The schema design ensures:

- data normalization
- scalability
- efficient queries
- relational referencing

---

## 🚀 Deployment

### Backend

Deploy using:

- Vercel
- Render
- Railway
- DigitalOcean

### Mobile App

Build APK:

```bash
npx expo run:android
```

Production build:

```bash
npx expo build:android
```

---

## 🧩 Future Enhancements

- Push notifications
- Product reviews & ratings
- Coupon & discount system
- Multi-vendor support
- AI-based product recommendations
- Offline support & caching
- Advanced analytics dashboard

---

## 📚 Academic Relevance

This project demonstrates concepts in:

- Mobile computing
- RESTful service architecture
- Secure authentication systems
- Cloud-based media storage
- Payment system integration
- UI/UX engineering
- Scalable backend design

---

## 🤝 Contribution Guidelines

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Submit a pull request

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

**Satinder Singh Sall**

Full-Stack Developer | Mobile App Developer | Software Engineer | Web Developer

---

## ⭐ Acknowledgements

- React Native & Expo Team
- MongoDB & Mongoose
- Cloudinary
- Clerk Authentication
- Open Source Community

---

## 📬 Contact

For questions, collaboration, or academic discussions:

📧 Email: [satindersinghsall111@gmail.com](mailto:satindersinghsall111@gmail.com)
🌐 Portfolio: [satinder-portfolio](https://satinder-portfolio.vercel.app/)

---

**If you found this project helpful, please ⭐ the repository.**

---

# 🛍️ Full-Stack E-Commerce Mobile App

A **modern full-stack e-commerce mobile application** built with **React Native (Expo)** and **Node.js / Express / MongoDB**.
The app provides a complete shopping experience including **authentication, product browsing, cart management, checkout, orders, admin management, and payment integration**.

This project demonstrates **mobile development, backend APIs, authentication, cloud services, and full-stack architecture**.

---

# 📱 Screenshots (Coming Soon...)

- Home Screen
- Product Page
- Cart
- Checkout
- Orders
- Admin Dashboard

---

# 🚀 Features

## 👤 User Features

- User authentication using **Clerk**
- Browse products
- Product detail page
- Add / remove products from cart
- Wishlist (favorites)
- Address management
- Checkout flow
- Cash on delivery support
- Order placement
- Order history
- Order tracking timeline
- Order details page
- Lottie success animations

---

## 🛒 Shopping Features

- Product catalog
- Categories
- Product images
- Cart management
- Quantity updates
- Size selection
- Price calculations
- Shipping and tax support

---

## 📦 Order System

- Create order from cart
- Order status tracking
- Order lifecycle:

```
Placed → Processing → Shipped → Delivered
```

- Payment status tracking

---

## 🛠️ Admin Features

Admin dashboard includes:

- Product management
- Add products
- Edit products
- Delete products
- Order management
- View all orders
- Update order status

---

## 📍 Address Management

Users can:

- Add addresses
- Edit addresses
- Delete addresses
- Set default address

---

## 💳 Payment System

Supports:

- Cash on Delivery
- Stripe integration (backend ready)

---

# 🏗️ Tech Stack

## Frontend (Mobile App)

| Technology                   | Purpose                       |
| ---------------------------- | ----------------------------- |
| React Native                 | Mobile framework              |
| Expo                         | Development environment       |
| Expo Router                  | Navigation system             |
| NativeWind                   | Tailwind CSS for React Native |
| Axios                        | API requests                  |
| Clerk                        | Authentication                |
| Lottie                       | Animations                    |
| React Navigation             | Navigation system             |
| React Native Gesture Handler | Gesture support               |
| React Native Toast Message   | Notifications                 |

---

## Backend

| Technology | Purpose           |
| ---------- | ----------------- |
| Node.js    | Runtime           |
| Express.js | Backend framework |
| MongoDB    | Database          |
| Mongoose   | ODM               |
| Clerk      | Authentication    |
| Stripe     | Payments          |
| Cloudinary | Image uploads     |
| Multer     | File uploads      |
| CORS       | API security      |

---

# 📂 Project Structure

```
E-Commerce Mobile App
│
├── client (React Native Expo App)
│
│   ├── app
│   │   ├── (auth)
│   │   ├── (tabs)
│   │   ├── admin
│   │   ├── addresses
│   │   ├── orders
│   │   ├── product
│   │   └── checkout.tsx
│   │
│   ├── assets
│   │   ├── images
│   │   ├── animations
│   │   ├── constants
│   │   └── screenshots
│   │
│   └── context
│       ├── CartContext
│       └── WishlistContext
│
└── server (Node.js Backend)
    │
    ├── config
    │   ├── db
    │   ├── cloudinary
    │   └── env
    │
    ├── controllers
    ├── models
    ├── routes
    ├── middleware
    └── scripts
```

---

# ⚙️ Installation

## 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/ecommerce-mobile-app.git
cd ecommerce-mobile-app
```

---

## 2️⃣ Install dependencies

### Client

```bash
cd client
npm install
```

### Server

```bash
cd server
npm install
```

---

# ▶️ Running the Project

## Start Backend

```bash
cd server
npm run server
```

Backend runs on:

```
http://localhost:3000
```

---

## Start Mobile App

```bash
cd client
npm start
```

Run on:

```
Android Emulator
iOS Simulator
Expo Go
Web Browser
```

---

# 🌐 API Routes

## Products

```
GET /api/products
GET /api/products/:id
POST /api/products
PUT /api/products/:id
DELETE /api/products/:id
```

---

## Cart

```
GET /api/cart
POST /api/cart/add
PUT /api/cart/item/:productId
DELETE /api/cart/item/:productId
DELETE /api/cart
```

---

## Orders

```
GET /api/orders
GET /api/orders/:id
POST /api/orders
PUT /api/orders/:id/status
```

---

## Addresses

```
GET /api/addresses
POST /api/addresses
PUT /api/addresses/:id
DELETE /api/addresses/:id
```

---

## Wishlist

```
GET /api/wishlist
POST /api/wishlist
DELETE /api/wishlist/:productId
```

---

# 🔐 Authentication

Authentication is handled using **Clerk**.

Features:

- Secure authentication
- Token-based API access
- User session management
- Admin role support

---

# 📦 Database Models

Main models:

```
User
Product
Cart
Order
Address
Wishlist
```

---

# 📊 Order Flow

```
User adds product to cart
        ↓
User selects address
        ↓
Checkout
        ↓
Order created
        ↓
Cart cleared
        ↓
Order status tracking
```

---

# 🎨 UI / UX Highlights

- Modern mobile UI
- Tailwind styling with NativeWind
- Smooth animations
- Loading states
- Toast notifications
- Responsive layout
- Safe area support

---

# 📈 Future Improvements

Planned improvements:

- Stripe payment gateway
- Push notifications
- Order tracking map
- Product reviews
- Search functionality
- Pagination
- Admin analytics dashboard
- Image optimization
- Performance improvements

---

# 👨‍💻 Author

**Satinder Singh Sall**

Full-Stack Developer

Technologies:

```
React Native
Node.js
MongoDB
TypeScript
Expo
```

---

# 📜 License

This project is licensed under the **ISC License**.

---

# ⭐ Support

If you like this project:

⭐ Star the repository
🍴 Fork the project
📢 Share it with others

---
