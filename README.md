# 🧩 CropDoctor Backend Service

This repository contains the backend API service for the CropDoctor platform.

The backend is responsible for:
- User authentication & authorization
- Image diagnosis request handling
- Integration with the AI inference service
- Community & diary management
- Data persistence and business logic orchestration

---

## 🚀 Overview

The backend acts as the core orchestration layer between:

- Frontend client (React)
- AI inference module (CNN-based classifier)
- Database (MySQL)
- Cloud infrastructure (AWS)

It ensures secure communication, structured API responses, and scalable service boundaries.

---

## 🏗 Architecture

### Tech Stack

- **Node.js (v18.13.0)**
- **NestJS**
- **MySQL**
- **JWT Authentication**
- **AWS Integration (S3, EC2)**

---

## 🔐 Authentication & Security

- JWT-based authentication (Access Token & Refresh Token)
- Role-based access control (Admin guard)
- Secure password handling
- Sensitive data exclusion using serializers

---

## 📦 Core Features

### 1️⃣ AI Diagnosis Integration

- Accept plant image metadata from frontend
- Forward request to AI inference service
- Receive classification result
- Store diagnosis history in database
- Return structured response to client

---

### 2️⃣ Growth Diary Management

- Create, update, delete crop growth logs
- Associate diary entries with authenticated users
- Enable data retrieval and filtering

---

### 3️⃣ Community Board

- Post creation and commenting
- Ranking logic for popular posts
- Role-based moderation support

---

### 4️⃣ Admin Dashboard

- Manage plant disease categories
- Manage nutrient database
- Control restricted endpoints

---

## 🗄 Database Structure

Key entities include:

- Users
- Diagnoses
- Posts
- Comments
- Nutrients
- Categories

Relationships designed to:
- Maintain referential integrity
- Support scalable feature expansion

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```env
DB_HOST=
DB_USER=
DB_PASSWORD=
```
These variables configure database connectivity.

⚠️ Do not commit .env files to version control.

---

🖥 Running the Backend Service

# move into backend directory
```
cd backend
```
# install dependencies
```
npm install
```
# start development server
```
npm run start:dev
```

---
## 🎯 Design Considerations
- Clear separation between AI inference and business logic
- Modular service architecture
- Role-based access control
- Cloud deployment compatibility
- Scalable API structure

---
👨‍💻 Author

Jin Lee
AI-focused Software Engineer


