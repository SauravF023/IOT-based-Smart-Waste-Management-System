# ♻️ IOT-based-Smart-Waste-Management-System

> An IoT-powered Smart Waste Management System that monitors garbage bin levels in real time and optimizes waste collection routes, helping cities reduce operational costs, fuel consumption, and carbon emissions.

---

## 📌 Overview

The **Smart Waste Management System** is an IoT-based solution designed to improve urban waste collection through real-time monitoring and intelligent route optimization.

Using Arduino sensors, a Node.js backend, MongoDB database, and a React dashboard, the system continuously tracks bin status and generates optimized routes for garbage collection vehicles.

### ✨ Key Benefits

* 📡 Real-time monitoring of garbage bins
* 🚛 Intelligent route optimization
* ⛽ Reduced fuel consumption
* 🌱 Lower carbon emissions
* 🏙️ Cleaner and smarter cities
* 📊 Interactive monitoring dashboard

---

# 🚀 Features

### 📍 Real-Time Bin Monitoring

* Monitor multiple smart bins simultaneously
* Live fill-level updates
* Bin status:

  * 🟢 Empty
  * 🟡 Moderate
  * 🔴 Full

### 🛣️ Smart Route Optimization

* Truck starts from a fixed depot
* Visits only bins that require collection
* Uses TSP-based route optimization with OSRM

### 🤖 Intelligent Decision Making

* **BIN_01**

  * Fill Level
  * Gas Detection
  * Temperature Monitoring

* **Other Bins**

  * Fill-level based monitoring

### 🔄 Auto Refresh Dashboard

* Live updates every **3 seconds**
* Smooth UI status changes

### 🔐 Authentication

* User Registration
* User Login
* JWT Authentication
* Protected Routes

---

# 🛠 Tech Stack

## Hardware

* Arduino Uno
* HC-SR04 Ultrasonic Sensor
* MQ Gas Sensor
* LM35 Temperature Sensor

## Frontend

* React.js
* Tailwind CSS
* Leaflet Maps

## Backend

* Node.js
* Express.js

## Database

* MongoDB

## Communication

* Arduino Serial Port
* Node.js SerialPort Library

## Route Optimization

* OSRM (Open Source Routing Machine)

---

# ⚙️ System Workflow

```text
Sensors
   │
   ▼
Arduino Uno
   │
Serial Communication
   │
   ▼
Node.js Backend
   │
Express API
   │
MongoDB Database
   │
React Dashboard
   │
Leaflet Map + Route Optimization
```

---

# 📂 Project Structure

```bash
smart-waste-management/
│
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   └── server.js
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── App.jsx
│   └── main.jsx
│
├── arduino/
│   └── smart_bins.ino
│
├── README.md
└── package.json
```

---

# 📡 Data Flow

1. Sensors detect garbage fill levels.
2. Arduino processes sensor readings.
3. Data is transmitted via Serial Port.
4. Node.js reads incoming data.
5. Backend updates MongoDB.
6. React Dashboard fetches updated information.
7. OSRM calculates the shortest collection route.
8. Map displays the optimized path.

---

# 📊 Sample Serial Data

```text
BIN_01,89,100,30
BIN_02,65,0,0
```

| Field       | Description             |
| ----------- | ----------------------- |
| binId       | Bin Identifier          |
| fillLevel   | Garbage fill percentage |
| gasLevel    | Gas sensor reading      |
| temperature | Temperature reading     |

---

# 🔑 Authentication

* Register new users
* Login with credentials
* JWT Token Authentication
* Protected API Routes
* Token stored securely in localStorage

---

# 📥 Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/smart-waste-management.git

cd smart-waste-management
```

---

## 2️⃣ Backend Setup

```bash
cd backend

npm install

npm start
```

---

## 3️⃣ Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

---

## 4️⃣ Arduino Setup

* Open `smart_bins.ino` in Arduino IDE
* Connect all sensors correctly
* Select the correct COM Port
* Upload the code to Arduino Uno

---

# 📸 Screenshots

## 🏠 Landing Page

> *(Add Screenshot Here)*

---

## 🔐 Login Page

> *(Add Screenshot Here)*

---

## 📊 Dashboard

> *(Add Screenshot Here)*

---

## 🗺️ Optimized Route Map

> *(Add Screenshot Here)*

---

# 🔮 Future Improvements

* 📱 Mobile Application
* ☁️ Cloud Deployment
* 📧 SMS & Email Alerts
* 🤖 AI-Based Waste Prediction
* 📍 GPS Tracking of Collection Vehicles
* 🔔 Push Notifications
* 📈 Analytics Dashboard
* 🧠 Machine Learning-Based Route Prediction

---

# 🤝 Contributing

Contributions are welcome!

1. Fork this repository
2. Create your feature branch

```bash
git checkout -b feature/NewFeature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push to the branch

```bash
git push origin feature/NewFeature
```

5. Open a Pull Request

---

# 👨‍💻 Author

**Saurav Mishra**

* 🎓 B.Tech (Electronics & Communication Engineering)
* 💻 Software Developer
* 🌐 MERN Stack | Java | Python | IoT

---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and distribute this project for educational and research purposes.

---

## ⭐ If you found this project helpful, don't forget to give it a Star!
