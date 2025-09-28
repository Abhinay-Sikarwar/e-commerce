# 🛒 Full-Stack E-Commerce Platform

![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat-square)
![React](https://img.shields.io/badge/React-18-blue?style=flat-square&logo=react)
![Node.js](https://img.shields.io/badge/Node.js-18-green?style=flat-square&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-8.6-brightgreen?style=flat-square&logo=mongodb)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4-38B2AC?style=flat-square&logo=tailwindcss)
![Razorpay](https://img.shields.io/badge/Razorpay-Payments-blue?style=flat-square&logo=razorpay) 

---

## 📖 About The Project

The **E-Commerce Platform** is a feature-rich, full-stack web application built to deliver a **modern online shopping experience**.  
It enables users to **browse products, add them to a cart, complete secure checkout with payments, and track orders**, while administrators have tools to **manage inventory, customers, and sales**.

Built with the **MERN stack (MongoDB, Express, React, Node.js)** and styled with **TailwindCSS**, the platform ensures **speed, scalability, and responsive design**.

---

## ✨ Features

- 🔐 **Authentication & Authorization** – Secure JWT-based login/signup with role management.  
- 🛍 **Product Catalog** – Browse, search, filter, and view product details.  
- 🛒 **Cart & Checkout** – Add/remove/update products, calculate totals, and checkout.  
- 💳 **Payments Integration** – Razorpay for smooth and secure transactions.  
- 📦 **Order Tracking** – Real-time order history and tracking.  
- 🛠 **Admin Dashboard** – Manage products, categories, users, and orders.  
- 📱 **Responsive Design** – Fully optimized for desktop, tablet, and mobile.  
- 📧 **Email Notifications** (planned) – Order confirmations, password resets, and more.  

---

## 📁 Directory Structure

```

Directory structure:
└──  e-commerce/
    ├── LICENSE
    ├── client/
    │   ├── package.json
    │   ├── tailwind.config.js
    │   ├── public/
    │   │   ├── index.html
    │   │   ├── manifest.json
    │   │   └── robots.txt
    │   └── src/
    │       ├── App.js
    │       ├── App.test.js
    │       ├── index.css
    │       ├── index.js
    │       ├── reportWebVitals.js
    │       ├── setupTests.js
    │       ├── app/
    │       │   ├── constants.js
    │       │   └── store.js
    │       ├── features/
    │       │   ├── admin/
    │       │   │   └── components/
    │       │   │       ├── AdminOrderDetail.js
    │       │   │       ├── AdminOrders.js
    │       │   │       ├── AdminProductDetail.js
    │       │   │       ├── AdminProductList.js
    │       │   │       └── ProductForm.js
    │       │   ├── auth/
    │       │   │   ├── authAPI.js
    │       │   │   ├── authSlice.js
    │       │   │   └── components/
    │       │   │       ├── ForgotPassword.js
    │       │   │       ├── Login.js
    │       │   │       ├── Logout.js
    │       │   │       ├── Protected.js
    │       │   │       ├── ProtectedAdmin.js
    │       │   │       ├── ResetPassword.js
    │       │   │       └── Signup.js
    │       │   ├── brands/
    │       │   │   ├── brandsAPI.js
    │       │   │   └── brandSlice.js
    │       │   ├── cart/
    │       │   │   ├── Cart.js
    │       │   │   ├── cartAPI.js
    │       │   │   └── cartSlice.js
    │       │   ├── category/
    │       │   │   ├── categoryAPI.js
    │       │   │   └── categorySlice.js
    │       │   ├── common/
    │       │   │   └── components/
    │       │   │       ├── Footer.js
    │       │   │       ├── Modal.js
    │       │   │       └── Pagination.js
    │       │   ├── navbar/
    │       │   │   └── Navbar.js
    │       │   ├── order/
    │       │   │   ├── orderAPI.js
    │       │   │   └── orderSlice.js
    │       │   ├── payment/
    │       │   │   ├── paymentAPI.js
    │       │   │   └── paymentSlice.js
    │       │   ├── product/
    │       │   │   ├── productAPI.js
    │       │   │   ├── productSlice.js
    │       │   │   └── components/
    │       │   │       ├── ProductDetail.js
    │       │   │       └── ProductList.js
    │       │   └── user/
    │       │       ├── userAPI.js
    │       │       ├── userSlice.js
    │       │       └── components/
    │       │           ├── UserOrders.js
    │       │           └── UserProfile.js
    │       └── pages/
    │           ├── 404.js
    │           ├── AdminHome.js
    │           ├── AdminOrderDetailPage.js
    │           ├── AdminOrdersPage.js
    │           ├── AdminProductDetailPage.js
    │           ├── AdminProductFormPage.js
    │           ├── CartPage.js
    │           ├── Checkout.js
    │           ├── ForgotPasswordPage.js
    │           ├── Home.js
    │           ├── LoginPage.js
    │           ├── OrderSuccessPage.js
    │           ├── ProductDetailPage.js
    │           ├── ResetPasswordPage.js
    │           ├── SignupPage.js
    │           ├── UserOrdersPage.js
    │           └── UserProfilePage.js
    └── server/
        ├── index.js
        ├── package.json
        ├── pnpm-lock.yaml
        ├── .env.sample
        ├── controllers/
        │   ├── Auth.Controller.js
        │   ├── Brand.Controller.js
        │   ├── Cart.Controller.js
        │   ├── Category.Controller.js
        │   ├── Mail.Controller.js
        │   ├── Order.Controller.js
        │   ├── Payment.Controller.js
        │   ├── Product.Controller.js
        │   └── User.Controller.js
        ├── models/
        │   ├── Brand.Model.js
        │   ├── Cart.Model.js
        │   ├── Category.Model.js
        │   ├── Order.Model.js
        │   ├── Payment.Model.js
        │   ├── Product.Model.js
        │   └── User.Model.js
        ├── routes/
        │   ├── Auth.Routes.js
        │   ├── Brand.Routes.js
        │   ├── Cart.Routes.js
        │   ├── Category.Routes.js
        │   ├── Mail.Routes.js
        │   ├── Order.Routes.js
        │   ├── Payment.Routes.js
        │   ├── Product.Routes.js
        │   └── User.Routes.js
        ├── services/
        │   ├── Common.js
        │   └── Mails/
        │       ├── ConfirmationMail.js
        │       ├── ResetMail.js
        │       ├── SendEMail.js
        │       └── WelcomMail.js
        └── utils/
            └── connectDB.js

````

---

## 🏗️ Architecture

The system is designed for **scalability, modularity, and performance**.  

- **Frontend:** React + TailwindCSS for modern, fast UI.  
- **Backend:** Node.js + Express for REST APIs.  
- **Database:** MongoDB with Mongoose.  
- **Authentication:** JWT-based security.  
- **Payments:** Integrated Razorpay.  

```mermaid
graph TD
    %% Nodes
    U[👤 User]
    F[💻 React Frontend]
    API[⚙️ Express API]
    DB[(🗄 MongoDB)]
    Pay[💳 Payment Gateway]

    %% Edges
    U --> F
    F --> API
    API --> DB
    API --> Pay
    U -->|🔑Login/Signup| API
    U -->|🛒Browse Products| F
    U -->|💰Place Order| Pay
    Pay --> API
    DB --> API

    %% Styling Classes
    classDef user fill:#FFB347,stroke:#333,stroke-width:2px,color:#000,font-weight:bold;
    classDef frontend fill:#61DBFB,stroke:#0d3b66,stroke-width:2px,color:#000,font-weight:bold;
    classDef api fill:#facc15,stroke:#ca8a04,stroke-width:2px,color:#000,font-weight:bold;
    classDef db fill:#4ade80,stroke:#166534,stroke-width:2px,color:#000,font-weight:bold;
    classDef pay fill:#6366f1,stroke:#312e81,stroke-width:2px,color:#fff,font-weight:bold;

    %% Apply classes
    class U user
    class F frontend
    class API api
    class DB db
    class Pay pay
```

---

## ⚙️ Getting Started

### Prerequisites

* Node.js v18+
* MongoDB instance (local/Atlas)
* Payment Gateway API keys

### Installation

```bash
git clone https://github.com/Abhinay-Sikarwar/e-commerce.git
cd your-repo
```

Install client dependencies:

```bash
cd client
npm install
```

Install server dependencies:

```bash
cd ../server
npm install
```

### Configuration

Create a `.env` in **server/**:

```env
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
PAYMENT_GATEWAY_KEY=your_payment_key
```

### Run Development Servers

Backend:

```bash
cd server
npm run dev
```

Frontend:

```bash
cd client
npm start
```

Now open 👉 [http://localhost:3000](http://localhost:3000)

---

## 🛣️ Roadmap

* [x] Authentication (JWT)
* [x] Product Management
* [x] Cart & Checkout
* [x] Payments Integration
* [ ] Email Notifications
* [ ] Analytics Dashboard
* [ ] Multi-language Support

---

## 📜 License

MIT License © 2025 [Abhinay-Sikarwar]

---

## 📬 Contact

👨‍💻 **Abhinay Sikarwar**

📧 **[abhinaysikarwar1234@gmail.com](mailto:abhinaysikarwar1234@gmail.com)**

---

### ⭐ Support

If you like this project, please **star it on GitHub ⭐** and share feedback!

---
