# ENTNT Dental Center Management Dashboard

Hello there! This is a Dental Center Management system for ENTNT built with React(frontend-only). It allows an Admin (Dentist) to manage patients and appointments, and lets Patients see their own data. All data is stored in localStorage to simulate a real workflow without any backend.

## 🔗 Live Demo

[View Deployed App on Netlify](https://your-netlify-link-here.netlify.app)

## 📂 GitHub Repository

[View Source Code on GitHub](https://github.com/your-github-username/dental-center-management)

## ✨ Features

✅ User Authentication (Admin & Patient)  
✅ Session persistence via localStorage  
✅ Role-based access control  
✅ Dashboard with KPIs  
✅ Patient management (Admin-only)  
✅ Appointment management (Admin-only)  
✅ Calendar view (Admin-only)  
✅ Patient portal with their own appointments and treatment history  
✅ File upload with preview (base64)  
✅ Responsive design

##  User Roles & Pages

### Admin (Dentist)
- **Login:** admin@entnt.in / admin123  
- **Pages for Admin:**
  - Dashboard: Overview of KPIs, greeting, and quick stats.
  - Patients: View, add, edit, and delete patient records.
  - Appointments: Add and manage appointments for patients.
  - Calendar: Visual monthly/weekly view of all appointments.
  - Logout: Clear session and go back to login.

### Patient (e.g., John Doe)
- **Login:** john@entnt.in / patient123  
- **Patient Dashboard:**
  - Shows welcome message.
  - Displays only the patient’s appointments and treatments.
  - Allows viewing attached treatment files (e.g., invoices, X-rays).

## 🔑 Login Credentials

| Role    | Email             | Password   |
|---------|-------------------|------------|
| Admin   | admin@entnt.in    | admin123   |
| Patient | john@entnt.in     | patient123 |

## 🛠️ Tech Stack

- React (Functional Components)
- React Router
- Context API
- TailwindCSS
- LocalStorage (for simulating data persistence)

## 🏗️ Project Structure
src/
components/ Reusable components (KPIs, PatientList, etc.)
contexts/  UserContext for global auth state
pages/ Different pages: Login, AdminDashboard, PatientDashboard, etc.
utils/ Utility functions for data management
App.js
index.js



## 🗂️ Sample Data

The app uses mock data stored in localStorage with two users: one Admin and one Patient. Patient data includes personal details and appointment records. File uploads (e.g., invoices, X-rays) are stored as base64 or blob URLs.

## 🚀 Setup Instructions

1. Clone this repo:
git clone https://github.com/your-github-username/dental-center-management.git
cd dental-center-management


2. Install dependencies:
npm install


3. Start the app locally:
npm start


4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📦 Deployment

The app is deployed on Netlify. You can deploy it yourself by linking your GitHub repo to Netlify or Vercel, and it should work out of the box as it's a static React build.

## ✅ Architecture & State Management

- Auth state and user sessions are managed using React Context (`UserContext`).
- All CRUD operations (add, edit, delete patients/appointments) read/write to `localStorage`.
- Data updates trigger UI re-render via state and context updates.
- App uses React Router for page-based routing (login, dashboards).

## 📝 Technical Decisions

- Chose React Context over Redux for simplicity and because the app state is small.
- Used TailwindCSS for faster styling and responsiveness.
- File uploads are saved as base64 in localStorage to meet frontend-only requirements.
- Avoided external APIs and backends as per assignment guidelines.

## ⚠️ Issues / Limitations

- Since data is in localStorage, it will reset if you clear browser storage.
- File uploads are not optimized for large files (base64 can be heavy).

## 🎉 Bonus Features

- Animated clock and greeting in Admin dashboard.
- Sun/moon switch based on time of day.
- Visual calendar with clickable days showing appointments.


by [KOLLA HARSHA VARDHAN] - vharsha101@gmail.com
