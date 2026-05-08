# Vingo - Real-time Food Delivery Application

Vingo is a comprehensive, full-stack food delivery application built using the MERN stack. It features real-time order tracking, role-based dashboards (User, Shop Owner, Delivery Boy), and integrated payment gateways.

## 🚀 Features

### For Users
- **Location-based Search:** Automatically detects city or allows manual selection to find nearby shops and items.
- **Real-time Search:** Quickly find food items or categories.
- **Cart & Checkout:** Seamlessly manage cart items and choose between COD or Online Payment (Razorpay).
- **Live Order Tracking:** Track your order's journey in real-time on a map.
- **Ratings:** Rate your favorite food items after delivery.

### For Shop Owners
- **Shop Management:** Create and edit shop profiles including images.
- **Item Management:** Add, edit, or delete food items with category and pricing.
- **Order Processing:** Manage incoming orders and update status (Pending, Preparing, Out for Delivery).
- **Delivery Assignment:** Automatically broadcasts orders to nearby available delivery boys.

### For Delivery Boys
- **Real-time Tracking:** Broadcasts live location while on duty.
- **Assignment Management:** Accept new delivery assignments in real-time.
- **OTP Verification:** Secure delivery using customer-provided OTP.
- **Earnings Dashboard:** Visualize daily deliveries and earnings with interactive charts.

---

## 🛠️ Tech Stack

- **Frontend:** React (Vite), Redux Toolkit, Tailwind CSS, Leaflet (Maps), Socket.io-client, Recharts.
- **Backend:** Node.js, Express, MongoDB (Mongoose), Socket.io, JWT, Multer.
- **Services:** Cloudinary (Images), Razorpay (Payments), Geoapify (Geocoding), Nodemailer (Email notifications).

---

## 📦 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/official1saurabh-ship-it/vingo.git
cd vingo
```

### 2. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add the following variables:
   ```env
   PORT=8000
   MONGODB_URL=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   EMAIL=your_gmail_address
   PASS=your_gmail_app_password
   CLOUDINARY_CLOUD_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   ```
4. Start the server:
   ```bash
   npm run dev
   ```

### 3. Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add the following variables:
   ```env
   VITE_FIREBASE_APIKEY=your_firebase_key
   VITE_GEOAPIKEY=your_geoapify_api_key
   VITE_RAZORPAY_KEY_ID=your_razorpay_test_id
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

---

## 🛡️ Security
- Environment variables are protected and ignored by Git.
- Authentication is handled via secure JWT cookies.
- Role-based authorization on all critical API endpoints.

## 📄 License
This project is licensed under the ISC License.
