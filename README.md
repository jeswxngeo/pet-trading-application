# 🐾 AI-Powered Pet Trading Platform

<p align="center">

![Flutter](https://img.shields.io/badge/Flutter-3.x-blue?logo=flutter)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?logo=fastapi)
![Python](https://img.shields.io/badge/Python-3.11+-yellow?logo=python)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?logo=postgresql)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-CatBoost-orange)
![Mapbox](https://img.shields.io/badge/Mapbox-Maps-black?logo=mapbox)
![JWT](https://img.shields.io/badge/JWT-Authentication-red)
![License](https://img.shields.io/badge/License-MIT-green)

</p>

---

# 📌 Overview

The **AI-Powered Pet Trading Platform** is a cross-platform marketplace developed to simplify the buying and selling of pets while integrating modern Artificial Intelligence, personalized recommendations, secure communication, location-based services, and administrative management.

The application enables users to list pets for sale, browse available pets, communicate securely with sellers, receive AI-generated price predictions, and manage their listings efficiently. The platform also includes a comprehensive **Admin Portal** for monitoring platform activity, moderating listings, managing users, overseeing AI model retraining, and generating analytics.

This project was developed as part of a **Full Stack Development Internship** and demonstrates expertise in mobile application development, backend API development, machine learning integration, database management, and scalable software architecture.

---

# 🚀 Key Features

## 👤 User Management

- Secure User Registration
- JWT Authentication
- Login & Logout
- Skip Login Mode
- Profile Management
- Role-Based Access Control
- Account Settings
- Delete Account
- Logout From All Devices

---

## 🐶 Pet Marketplace

- Post New Pet Listings
- Edit Listings
- Delete Listings
- My Listings
- Previously Sold Listings
- Favourite Pets
- Advanced Search
- Category Filtering
- Breed Filtering
- State & City Filtering
- Seller Ratings
- Reviews
- Multiple Image Upload
- Dynamic Pet Categories
- Vaccination Details
- Age
- Weight
- Gender
- City & State Based Listings

---

## 💬 Real-Time Chat System

- Buyer & Seller Chat
- Buying Section
- Selling Section
- Chat Time Updates
- Important Chats
- Delete Multiple Chats
- Mark Trade as Completed
- Store Buying Price
- Store Selling Price
- Predefined Quick Questions
- Trade History

---

## 🤖 Artificial Intelligence

### AI Price Prediction

Predicts an optimal selling price using:

- Pet Category
- Breed
- Age
- Gender
- Weight
- Vaccination Status
- Location
- Additional Listing Features

Powered by:

- CatBoostRegressor

Features:

- Automatic Prediction
- Manual Retraining
- Continuous Learning
- Admin Approval Based Retraining
- Prediction Storage
- Sold Price Learning

---

## 🎯 Recommendation Engine

Personalized recommendations based on:

- Buying History
- Selling History
- Completed Trades
- Favourite Categories
- Previously Viewed Pets

Model continuously improves recommendations using newly completed trade information.

---

## 🗺️ Maps & Location

Integrated using Mapbox.

Features include:

- User Location
- Map Picker
- City & State Detection
- Current Location Support
- Mobile & Windows Compatibility

---

## ⭐ Reviews & Ratings

- 5 Star Ratings
- Seller Reviews
- Review History
- Trust Score
- Rating Visibility

---

## ❤️ Favourite System

- Add to Favourites
- Remove from Favourites
- Favourite Pets Screen
- Prevent Favourite of Own Listings

---

## 📈 Admin Portal

Complete administrative dashboard featuring:

### Dashboard

- Total Users
- Total Listings
- Completed Trades
- Active Listings
- Analytics
- Reports
- AI Statistics

### User Management

- View Users
- Suspend Accounts
- Delete Accounts
- Search Users
- User Details

### Listing Management

- View Listings
- Remove Listings
- Approve Listings
- Manage Sold Listings

### Trade Management

- Buying Price
- Selling Price
- Completed Trades
- Trade Analytics

### AI Management

- Model Retraining
- Training Approval
- Prediction Analytics
- Dataset Monitoring
- Model Status

### Reports

- User Reports
- Listing Reports
- Review Reports

### Notifications

- Broadcast Notifications
- System Alerts

### Help & Support Management

- FAQ Management
- User Queries

---

# 🧠 Machine Learning

The application integrates Machine Learning using **CatBoostRegressor**.

## Model Features

- AI Price Prediction
- Continuous Retraining
- Sold Price Learning
- Feature Engineering
- Automatic Encoding
- Model Persistence

Training Data Sources

- Initial Dataset
- Completed Trades
- Sold Price Records
- Approved Admin Data

---

# 🏗️ System Architecture

```
Flutter Application
        │
        │ REST API
        ▼
FastAPI Backend
        │
 ┌──────┼─────────┐
 │      │         │
 ▼      ▼         ▼
PostgreSQL   AI Engine   Mapbox
 Database   CatBoost     Maps
```

---

# 🗂️ Project Structure

```
pet-trading-platform/

│

├── frontend/

│ ├── lib/

│ ├── assets/

│ ├── android/

│ ├── ios/

│ ├── windows/

│ └── pubspec.yaml

│

├── backend/

│ ├── app/

│ ├── routers/

│ ├── models/

│ ├── schemas/

│ ├── services/

│ ├── ml/

│ ├── database/

│ └── main.py

│

├── admin_portal/

│ ├── src/

│ ├── public/

│ └── package.json

│

├── docs/

│

├── database/

│

└── README.md

```

---

# 🛠️ Technology Stack

## Frontend

- Flutter
- Dart
- Material UI

---

## Backend

- FastAPI
- Python
- SQLAlchemy
- Alembic
- JWT Authentication
- Pydantic

---

## Database

- PostgreSQL

---

## Machine Learning

- CatBoostRegressor
- Pandas
- NumPy
- Scikit-Learn

---

## Maps

- Mapbox
- OpenStreetMap

---

## Development Tools

- Android Studio
- VS Code
- pgAdmin
- Git
- GitHub
- Postman

---

# 📊 Database Modules

The application consists of relational database modules including:

- Users
- Pets
- Reviews
- Ratings
- Messages
- Favourite Pets
- Trading Prices
- AI Predictions
- Notifications
- Reports
- Admin
- User Sessions

---

# 🔐 Security

- JWT Authentication
- Password Hashing
- Protected APIs
- Role-Based Authorization
- Admin Authentication
- Secure Password Storage
- Request Validation
- API Authorization

---

# 📱 Cross Platform Support

- Android
- Windows Desktop
- Web *(Backend Ready)*

---

# 📷 Screenshots

## Login

```
docs/screenshots/login.png
```

## Home Page

```
docs/screenshots/home.png
```

## Sell Your Pet

```
docs/screenshots/add_pet.png
```

## Chat

```
docs/screenshots/chat.png
```

## Admin Dashboard

```
docs/screenshots/admin_dashboard.png
```


# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/jeswxngeo/pet-trading-platform.git

cd pet-trading-platform
```

---

## Backend

```bash
cd backend

python -m venv venv

venv\Scripts\activate

pip install -r requirements.txt

uvicorn main:app --reload
```

---

## Frontend

```bash
cd frontend

flutter pub get

flutter run
```

---

## Admin Portal

```bash
cd admin_portal

npm install

npm run dev
```

---

# 📄 API Documentation

FastAPI automatically generates API documentation.

Swagger UI

```
http://localhost:8000/docs
```

ReDoc

```
http://localhost:8000/redoc
```

---

# 🧪 Testing

The application has been tested for:

- User Authentication
- Listing Management
- Chat
- AI Price Prediction
- Recommendation Engine
- Admin Portal
- Database CRUD Operations
- API Endpoints
- Maps Integration
- Reviews
- Ratings

---

# 📈 Future Enhancements

- Membership Plans
- Online Payments
- Premium Seller Accounts
- Video Calling
- AI Health Detection
- Vaccination Reminder
- Pet Adoption Module
- Appointment Booking
- Pet Insurance
- Veterinary Marketplace
- Cloud Deployment
- Push Notifications
- Multi-Language Support

---

# 🤝 Contributing

Contributions are welcome.

Please fork the repository and create a pull request for any improvements or bug fixes.

---

# 📜 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Jeswin Geo**

Full Stack Developer

- Flutter
- FastAPI
- PostgreSQL
- Python
- Machine Learning
- Artificial Intelligence
- REST APIs
- Cross Platform Development

---

# 🙏 Acknowledgements

Special thanks to:

- OneThe416 Pvt. Ltd.
- Flutter
- FastAPI
- PostgreSQL
- CatBoost
- Open Source Community

---

## ⭐ If you found this project useful, please consider giving it a star!
