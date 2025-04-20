# 📱 sellEase – Mobile Commerce & Live Sales for Youth Entrepreneurs

sellEase is a mobile-first eCommerce and live sales platform designed to empower youth entrepreneurs and small business owners in Africa and beyond. With sellEase, users can create mini-shops, showcase products, go live to sell in real-time, and accept orders via chat — all from their phone.

This full-stack project is built using **Flutter (Riverpod)** for the frontend, **Express.js** for the backend, and **MongoDB** as the database.

---

## 🛠 Tech Stack

| Layer         | Stack                      |
|---------------|----------------------------|
| Mobile App    | Flutter + Riverpod         |
| Backend API   | Node.js + Express.js       |
| Database      | MongoDB + Mongoose         |
| Auth          | JWT                        |
| Media Uploads | Cloudinary / Multer        |
| DevOps        | GitHub Actions, Docker     |

---

## 🎯 Features

### MVP
- ✅ User Registration & Login
- ✅ Seller profile & shop setup
- ✅ Product listing (name, image, price, description, stock)
- ✅ Live video selling interface (mocked in MVP)
- ✅ Chat-based order system (simplified)
- ✅ Cloud image uploads
- ✅ Simple admin dashboard for sellers
- ✅ Mobile-first UI with clean architecture (Flutter)

### Post-MVP (Future Enhancements)
- 🎥 Real-time live video & reactions
- 📊 Analytics dashboard for sellers
- 💵 Mobile money integration (MTN, Airtel)
- 🛍 Shop links for sharing
- 🌍 Multilingual support (Kinyarwanda, English)
- 🚚 Order tracking & delivery integration
- 📲 Progressive Web App (PWA) version
- 🔔 Notifications (push & in-app)
- 💬 Reviews & ratings

---

## 📦 Folder Structure

lib/
│
├── core/                              # Core utilities for the entire app
│   ├── error/
│   │   └── failures.dart
│   ├── network/
│   │   ├── api_client.dart
│   │   └── network_info.dart
│   ├── utils/
│   │   ├── constants.dart
│   │   └── helpers.dart
│   └── injection.dart                  # Dependency injection configuration (using GetIt or Riverpod)
│
├── features/                           # Feature-specific logic
│   ├── auth/                           # Authentication feature (login, sign-up)
│   │   ├── auth_provider.dart          # Riverpod provider for auth-related states
│   │   ├── auth_service.dart           # Authentication service
│   │   ├── auth_page.dart              # UI for auth (login/signup)
│   │   └── user_model.dart             # Auth-related model (User, etc.)
│   │
│   ├── product/                        # Product feature (product list, details, etc.)
│   │   ├── product_provider.dart       # Riverpod provider for products
│   │   ├── product_service.dart        # Service to fetch product data (API call logic)
│   │   ├── product_page.dart           # UI for product list
│   │   └── product_model.dart          # Product data model
│   │
│   ├── live_sales/                     # Live Sales feature (Live streaming, selling)
│   │   ├── live_sales_provider.dart    # Riverpod provider for live sales
│   │   ├── live_sales_service.dart     # Service for live sales handling
│   │   ├── live_sales_page.dart        # UI for live sales (streaming page)
│   │   └── live_sale_model.dart        # Live sales-related model
│
└── main.dart                           # Entry point of the app

```bash
cd sellEase
flutter pub get
flutter run

