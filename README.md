# 📱 sellEase – Mobile eCommerce & Live Sales for Youth Entrepreneurs

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

## lib/
Main directory for all app logic.

## core/ – Core Utilities
Contains global resources used throughout the app.

error/
failures.dart – Defines custom error and failure classes.

network/
api_client.dart – Handles HTTP client setup (Dio or Http).

network_info.dart – Checks for internet connectivity.

utils/
constants.dart – App-wide constants like colors, strings, etc.

helpers.dart – Helper functions and extensions.

injection.dart –
Sets up dependency injection (via Riverpod or GetIt).

## features/ – Feature-Based Modules
Each app feature is isolated for clean code organization.

### auth/ – Authentication
Handles login, sign-up, and user-related logic.

auth_provider.dart – Riverpod state notifier for auth flow.

auth_service.dart – Logic for login, registration, logout.

auth_page.dart – UI for sign-in/sign-up.

user_model.dart – Defines User model.

### product/ – Product Listings
Handles everything related to listing and showing products.

product_provider.dart – Riverpod provider for product state.

product_service.dart – API calls and business logic.

product_page.dart – Product list/grid UI.

product_model.dart – Product model structure.

### live_sales/ – Live Streaming for Selling
Allows sellers to go live and promote products.

live_sales_provider.dart – Riverpod state for live session handling.

live_sales_service.dart – Start/stop stream, push product updates.

live_sales_page.dart – Live stream screen UI.

live_sale_model.dart – Live sales session data.

## main.dart
The app entry point. Initializes providers and routes.

```bash
cd sellEase
flutter pub get
flutter run

