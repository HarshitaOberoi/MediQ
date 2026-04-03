<div align="center">

# 🏥 Qure
### The High-Velocity Healthcare Ecosystem

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white)](https://www.prisma.io/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Neon DB](https://img.shields.io/badge/Neon_DB-00E599?style=for-the-badge&logo=neon&logoColor=black)](https://neon.tech/)

**Qure is a frictionless healthcare management platform designed to eliminate medical bureaucracy by synchronizing Patients, Doctors, and Chemists into a single, real-time workflow.**

[Features](#-key-features) • [Tech Stack](#-tech-stack) • [Getting Started](#-getting-started) • [Project Structure](#-project-structure)

</div>

---

## 🌟 Overview

Built with a serverless **Neon PostgreSQL** architecture, Qure transforms the traditional, fragmented hospital visit into an automated, "gravity-defying" experience. It bridges the gap between different healthcare entities to provide a seamless patient journey.

## 🚀 Key Features

### 🔹 Phase 1: Deep Registry & Identity
- **Hierarchical Onboarding:** Advanced geographic mapping (State > City > Hospital) for accurate discovery.
- **Staff Inventory:** Comprehensive hospital profiles including ownership details and a full roster of doctors categorized by specialty.
- **Patient Personas:** Secure storage of vitals, blood groups, allergies, and chronic conditions established at registration.

### 🔹 Phase 2: Intelligent Discovery & Booking
- **Symptom-to-Specialist Mapping:** A smart search engine that maps user-described problems (e.g., "pancreas") to the correct experts (e.g., Gastroenterologists).
- **Transactional Appointment Suite:** High-integrity booking using Neon DB transactions to manage real-time slot availability and sequential Token Generation (e.g., 23 → 24).
- **Automated Pulse:** Precision reminders triggered 24 hours and 1 hour before the appointment.

### 🔹 Phase 3: Clinical & Pharmacy Operations
- **The Doctor’s Window:** Instant retrieval of the Patient Card (history + booking notes) the moment a token is called.
- **Advance Packing Loop:** Digital prescriptions are pushed instantly to the internal hospital chemist while the patient is still in consultation.
- **Anti-Scam Handover:** A secure protocol where the chemist reveals the patient’s Name/Phone only after the Token Number is provided.

### 🔹 Phase 4: Admin Control & Clinical Data
- **Global Dashboard:** A master interface for Admins to manage the ecosystem (delete/suspend Hospitals, Doctors, Pharmacies, or Patients).
- **Patient Attachments:** A dedicated upload system for patients to attach test results, old prescriptions, or medicine images during booking.

---

## 🛠️ Tech Stack

### Frontend
- **Framework:** React.js (Vite)
- **Styling:** Tailwind CSS
- **Animations:** Framer Motion
- **Icons:** Lucide React
- **State Management:** Zustand

### Backend
- **Environment:** Node.js
- **Framework:** Express.js
- **Database:** Neon DB (Serverless PostgreSQL)
- **ORM:** Prisma
- **Real-time:** WebSockets (Socket.io)
- **Storage:** Cloudinary (for medical attachments)

---

## 📁 Project Structure

```bash
Qure/
├── backend/            # Express API with Prisma ORM
│   ├── prisma/         # Database schema and seeds
│   ├── src/            # Backend source code
│   │   ├── controllers/# Route handlers
│   │   ├── routes/     # API endpoints
│   │   └── validators/ # Data validation (Zod)
│   └── server.js       # Entry point
├── frontend/           # React frontend with Vite
│   ├── src/            # Frontend source code
│   │   ├── components/ # Reusable UI components
│   │   ├── pages/      # Main application views
│   │   └── api/        # API communication layer
│   └── vite.config.js  # Vite configuration
└── README.md           # This file
```

---

## ⚙️ Getting Started

### Prerequisites
- Node.js (v18+)
- PostgreSQL (or Neon DB account)
- Cloudinary Account (for file uploads)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo/qure.git
   cd qure
   ```

2. **Backend Setup:**
   ```bash
   cd backend
   npm install
   # Create a .env file based on .env.example
   npx prisma db push
   npm run dev
   ```

3. **Frontend Setup:**
   ```bash
   cd ../frontend
   npm install
   npm run dev
   ```

---

## 🛡️ Security & Integrity

- **Soft Deletes:** Admin actions use `deleted_at` timestamps to preserve historical data integrity.
- **Privacy-First Pharmacy:** Sensitive patient data is hidden until physical verification at the chemist's window.
- **File Handling:** Secure cloud storage references for all medical attachments to keep the Neon DB lightweight and fast.

---

<div align="center">
Built with ❤️ for a better healthcare experience.
</div>
