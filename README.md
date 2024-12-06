# SwiftGo - Enjoy your Journey!  

Hi dosto,
Welcome to **SwiftGo**, a feature-rich, full-stack ride-sharing application inspired by Uber, built using the **MERN (MongoDB, Express.js, React.js, Node.js)** technology stack. This platform allows users to book rides, track drivers in real-time, and enjoy a seamless journey experience. 

## 📝 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Folder Structure](#folder-structure)
- [Installation Guide](#installation-guide)
- [API Endpoints](#api-endpoints)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

---

## 🌟 Project Overview

SwiftGo is designed to connect riders with drivers, offering a fast, reliable, and convenient travel solution. The platform includes user-friendly interfaces for both riders and drivers, as well as an admin panel for efficient management.

---

## ✨ Features

### Rider Features
- **User Registration/Login** with JWT Authentication
- **Ride Booking**: Select pickup and drop-off locations.
- **Real-Time Tracking**: View driver’s location on a map.
- **Fare Estimation**: Dynamic fare calculation based on distance and time.
- **Payment Integration**: Pay using cards, wallets, or UPI.
- **Ride History**: View past rides and payments.

### Driver Features
- **Driver Authentication**: Register, verify documents, and login securely.
- **Ride Requests**: Accept/decline ride requests.
- **Navigation**: Integrated with Google Maps for optimal routes.
- **Earnings Dashboard**: Track daily and weekly earnings.

### Admin Panel
- **User Management**: Add/remove users and drivers.
- **Ride Analytics**: Monitor active rides and revenue.
- **Complaint Handling**: Address user and driver complaints.
- **System Configuration**: Dynamic updates to fare rules and availability.

---

## 🔧 Tech Stack

### Frontend
- **React.js** with Hooks & Context API
- **Redux Toolkit** for state management
- **Material-UI** and custom CSS for styling
- **Google Maps API** for real-time location tracking

### Backend
- **Node.js** with Express.js
- **MongoDB** for the database
- **Socket.io** for real-time ride updates
- **JWT** for authentication and security

### Others
- **Cloudinary** for profile image and document uploads
- **Stripe API** for payment gateway integration
- **Docker** for containerized deployment

---

## 📁 Folder Structure

```
SwiftGo/
│
├── client/            # Frontend application
│   ├── public/
│   ├── src/
│       ├── components/
│       ├── pages/
│       ├── services/  # API calls
│       ├── utils/     # Helper functions
│       ├── App.js
│       └── index.js
│
├── server/            # Backend application
│   ├── config/        # Configuration files
│   ├── controllers/   # Route logic
│   ├── models/        # MongoDB schemas
│   ├── routes/        # API endpoints
│   ├── utils/         # Utility functions
│   └── server.js      # Entry point
│
├── README.md
├── package.json
└── .env               # Environment variables
```

---

## Installation Guide

### Prerequisites
- Node.js (v18+)
- MongoDB (local or cloud-based)
- Google Maps API key
- Stripe account for payment gateway

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/SwiftGo.git
   cd SwiftGo
   ```

2. Install dependencies:
   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the `server/` directory with:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     GOOGLE_MAPS_API_KEY=your_google_maps_api_key
     STRIPE_API_KEY=your_stripe_api_key
     ```

4. Start the development server:
   - Run the backend:
     ```bash
     cd server
     npm start
     ```
   - Run the frontend:
     ```bash
     cd client
     npm start
     ```

5. Open the application in your browser:
   - Frontend: `http://localhost:3000`
   - Backend: `http://localhost:5000`

---

## 📋 API Endpoints

### User Routes
| Method | Endpoint             | Description                  |
|--------|----------------------|------------------------------|
| POST   | `/api/users/register`| Register a new user          |
| POST   | `/api/users/login`   | Login a user                 |
| GET    | `/api/users/profile` | Fetch user profile           |

### Ride Routes
| Method | Endpoint             | Description                  |
|--------|----------------------|------------------------------|
| POST   | `/api/rides/request` | Request a ride               |
| GET    | `/api/rides/:id`     | Get ride details             |

### Payment Routes
| Method | Endpoint             | Description                  |
|--------|----------------------|------------------------------|
| POST   | `/api/payments/create` | Initiate payment            |

---

## 🔮 Future Enhancements
- **AI-Based Ride Matching**: Optimize driver allocation.
- **Multi-Language Support**: Expand user base with multiple languages.
- **In-App Chat**: Communication between riders and drivers.
- **Driver Ratings**: Improve service quality with a feedback system.
- **Ride Sharing**: Pool rides for cost-efficiency.

---

## 🤝 Contributing

I welcome for contributions! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Commit your changes.
4. Push to your branch.
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Feel free to reach out if you have any questions or feedback! 

Have a nice day!!!