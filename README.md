# 🩸 Blood Donation Network

## 🚀 Overview

The **Blood Donation Network** is a real-time web application designed to connect blood donors with recipients during emergencies. It enables users to quickly find nearby donors, raise urgent requests, and communicate instantly — potentially saving lives when every second matters.

---

## 🎯 Problem Statement

In emergency situations, finding compatible blood donors quickly is extremely difficult, especially in rural or semi-urban areas. Existing systems are slow, uncoordinated, or lack real-time communication.

---

## 💡 Solution

This platform provides:

* Real-time donor-recipient matching
* Emergency request broadcasting
* Location-based donor discovery
* Instant communication via chat

---

## 🛠 Tech Stack

### Backend

* Flask (Python)
* Flask-SQLAlchemy (Database ORM)
* Flask-SocketIO (Real-time communication)
* SQLite (Database)

### Frontend

* HTML, CSS, JavaScript

---

## 📂 Project Structure

```
blood_network/
│
├── app.py
├── models.py
├── init_db.py
│
├── templates/
│   └── index.html
│
├── static/
│   ├── css/
│   └── js/
│
└── blood.db
```

---

## ⚙️ Features

### 👤 User System

* Register as donor or recipient
* Store blood group, contact info, and location
* Availability toggle for donors

### 🚨 Emergency Requests

* Raise urgent blood requests
* Specify blood group and urgency level
* Track request status

### 📍 Location-Based Matching

* Stores latitude & longitude of users
* Helps find nearest available donors

### 💬 Real-Time Chat

* Direct communication between donor and recipient
* Powered by WebSockets (SocketIO)

---

## 🗄 Database Models

### User

* Name, blood group, phone
* Role (donor/recipient)
* Location (latitude, longitude)
* Donation count & availability

### EmergencyRequest

* Requester ID
* Blood group
* Location
* Urgency level & status

### ChatMessage

* Sender & receiver
* Message content
* Timestamp

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository

```
git clone <your-repo-link>
cd blood_network
```

### 2️⃣ Create virtual environment

```
python -m venv venv
venv\Scripts\activate   (Windows)
```

### 3️⃣ Install dependencies

```
pip install flask flask-sqlalchemy flask-socketio eventlet
```

### 4️⃣ Initialize database

```
python init_db.py
```

### 5️⃣ Run the server

```
python app.py
```

### 6️⃣ Open in browser

```
http://127.0.0.1:5000/
```

---

## 🌟 Unique Features

* Real-time emergency alerts
* Live donor availability tracking
* Location-based smart matching
* Integrated chat system

---

## 🔮 Future Enhancements

* AI-based donor prioritization
* Integration with hospitals/PHCs
* Mobile app version
* SMS/Call alerts for rural areas
* Blood inventory tracking


---

## 📌 Hackathon Note

This project is designed to be built within a **24-hour hackathon**, focusing on core functionality, real-time communication, and impactful problem-solving.

---

## ❤️ Impact

This system can significantly reduce the time required to find blood donors, especially in critical situations, and can help build a strong, responsive donor community.

---
