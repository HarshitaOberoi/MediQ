<div align="center">

# 🏥 Qure Backend
### The Core Healthcare API

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white)](https://www.prisma.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)

</div>

---

## 🚀 Features

- **RBAC (Role-Based Access Control):** Secure endpoints for Patients, Doctors, Chemists, and Admins.
- **Prisma ORM:** Type-safe database queries with a robust schema.
- **Neon Serverless DB:** Optimized for high performance and scalability.
- **Cloudinary Integration:** Secure storage and retrieval of patient medical attachments.
- **WebSockets:** Real-time prescription pushing and appointment updates.
- **Automated Cron Jobs:** Scheduled reminders for appointments and system maintenance.

## 🛠️ Tech Stack

- **Framework:** Express.js 5
- **ORM:** Prisma 6
- **Validation:** Zod
- **Authentication:** JWT + Bcryptjs
- **File Uploads:** Multer + Cloudinary
- **Scheduling:** Node-Cron
- **Real-time:** Socket.io

## 📁 Structure

- `src/controllers`: Business logic and route handlers.
- `src/routes`: API endpoints definition.
- `src/prisma`: Database schema and migration seeds.
- `src/middleware`: Authentication, error handling, and file uploads.
- `src/validators`: Zod schemas for request validation.
- `src/utils`: Helper classes (AppError, catchAsync).

## ⚙️ Development

1. **Install Dependencies:**
   ```bash
   npm install
   ```

2. **Environment Variables:**
   Copy `.env.example` to `.env` and configure your credentials.

3. **Database Setup:**
   ```bash
   npx prisma db push
   npx prisma generate
   ```

4. **Run Server:**
   ```bash
   npm run dev
   ```

---

<div align="center">
Part of the [Qure Ecosystem](../README.md)
</div>
