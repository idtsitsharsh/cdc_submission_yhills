# YHills Admin Dashboard

**Server-Rendered Course (Product) Management Dashboard**

🔗 **Live Application:**
👉 [https://cdc-submission-yhills-lb6dbzpke-idtsitsharshs-projects.vercel.app/](https://cdc-submission-yhills-lb6dbzpke-idtsitsharshs-projects.vercel.app/)

---

## Project Overview

This project is a **server-rendered administrative dashboard** built using **Next.js App Router** for managing products (courses) in an e-commerce–style system.
It focuses on **performance, clean architecture, secure admin access, and real-world CRUD workflows**.

The dashboard enables authenticated admins to **create, view, update, and delete courses**, upload images securely, visualize metrics, and manage admin access.

---

## Objective (As per Problem Statement)

* Design a **server-side rendered (SSR) admin dashboard**
* Ensure **fast page loads and improved SEO**
* Provide an **efficient interface** for managing products
* Implement **secure authentication and authorization**

---

## Key Features Implemented

### Authentication & Security

* Admin login using **JWT-based authentication**
* Secure **HTTP-only cookies**
* Auth verification via `/api/admin/check`
* Logout functionality
* Admin-only access to dashboard features

### Product (Course) Management

* Complete **CRUD operations**:

  * Create courses
  * View course details
  * Edit courses
  * Delete courses
* MongoDB-based data persistence
* Dynamic routing for individual course pages

### Multi-Step Course Creation

* Step-by-step course creation wizard:

  * Basic information
  * Pricing details
  * Image upload
  * Review & submit
* Input validation using **Zod**
* User-friendly, structured workflow

### Image Upload & Handling

* Secure image uploads using **Cloudinary**
* Automatic fallback image when no thumbnail is provided
* Optimized image rendering

### Dashboard & Metrics

* Admin overview dashboard
* Metrics API for dashboard statistics
* Interactive charts using **Recharts**
* Sidebar-based navigation for admin actions

### Admin Management

* Admin onboarding panel
* Admin-related actions visible only to authenticated admins

---

## Tech Stack Used

### Core Technologies

* **Next.js (App Router)** – Frontend, backend, and SSR
* **MongoDB** – Database
* **JWT** – Authentication
* **Zod** – Form validation
* **Cloudinary** – Image storage
* **Recharts** – Data visualization

### Architecture

* API routes using `app/api`
* Server and client component separation
* Centralized auth and database utilities
* Modular and scalable folder structure

---

## Application Workflow

1. Admin logs in using credentials
2. JWT token is generated and stored in an HTTP-only cookie
3. Dashboard verifies authentication via API
4. Server fetches and renders course data
5. Admin performs create, edit, or delete actions
6. UI updates reflect latest database state
7. Admin can securely log out

---

## Dummy Admin Credentials

Use the following credentials to access the dashboard:

```
Email:    admin@yhills.com
Password: admin123
```

---

## Local Setup Instructions

1. Clone the repository
2. Install dependencies

   ```bash
   npm install
   ```
3. Create `.env.local` and add:

   ```
   MONGODB_URI=
   JWT_SECRET=
   CLOUDINARY_CLOUD_NAME=
   CLOUDINARY_API_KEY=
   CLOUDINARY_API_SECRET=
   ```
4. Start the development server

   ```bash
   npm run dev
   ```

---

## Deliverables Covered

* ✅ Server-rendered admin dashboard
* ✅ Product (course) CRUD operations
* ✅ Multi-step validated forms
* ✅ Secure image uploads
* ✅ Authentication & authorization
* ✅ Live deployed application

---

## Notes

* The project strictly adheres to the given problem statement
* Only implemented features are documented
* Built to reflect **real-world admin dashboard development practices**
