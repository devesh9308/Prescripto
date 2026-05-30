# Prescripto 🩺 -   Doctor Appointment Booking Platform

Prescripto is a full-stack medical appointment booking platform designed to streamline interactions between patients, doctors, and administrators.
Built with the MERN stack, it enables online consultations, doctor discovery, real-time appointment tracking, and admin-level controls.

## 🚀 Features

### 👤 Patient Portal
- Browse doctors by specialization and fee
- Book appointments with preferred doctors
- Secure online payments via Razorpay
- Track appointment status in real-time

### 🩺 Doctor Dashboard
- Approve or reject patient appointment requests
- View schedule and patient list
- Track earnings and history

### 🔐 Admin Panel
- Add and manage doctor accounts
- Cancel or reschedule appointments
- Monitor doctor earnings and activity

## 🛠️ Tech Stack

- **Frontend:** React.js, Tailwind CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** jwt
- **Payments:** Razorpay
- **Cloud Storage:** Cloudinary
  

## 📁 Project Structure

```
medilink/
│
├── admin/ # Admin dashboard
│ ├── public/
│ │ └── index.html
│ ├── src/
│ │ ├── assets/
│ │ ├── components/ 
│ │ │ ├── Navbar.jsx
│ │ │ └── Sidebar.jsx
│ │ ├── context/ 
│ │ │ ├── AdminContext.jsx
│ │ │ ├── AppContext.jsx
│ │ │ └── DoctorContext.jsx
│ │ ├── pages/
│ │ │ ├── Admin/ # Admin pages
│ │ │ │ ├── AddDoctor.jsx
│ │ │ │ ├── AllAppointments.jsx
│ │ │ │ ├── Dashboard.jsx
│ │ │ │ └── DoctorsList.jsx
│ │ │ ├── Doctor/ # Doctor pages (inside admin panel)
│ │ │ │ ├── DoctorAppointment.jsx
│ │ │ │ ├── DoctorDashboard.jsx
│ │ │ │ └── DoctorProfile.jsx
│ │ │ └── Login.jsx # Admin/Doctor login page
│ │ ├── App.jsx # App root component
│ │ ├── index.css 
│ │ └── main.jsx # React entry point
│ ├── .env
│ ├── package.json
│ └── vite.config.js
│
├── backend/ 
│ ├── config/ 
│ │ ├── cloudinary.js
│ │ └── mongodb.js
│ ├── controllers/
│ │ ├── adminController.js
│ │ ├── doctorController.js
│ │ └── userController.js
│ ├── middlewares/ # Middleware for authentication & uploads
│ │ ├── authAdmin.js
│ │ ├── authDoctor.js
│ │ ├── authUser.js
│ │ └── multer.js
│ ├── models/ 
│ │ ├── appointmentModel.js
│ │ ├── doctorModel.js
│ │ └── userModel.js
│ ├── routes/ 
│ │ ├── adminRoute.js
│ │ ├── doctorRoute.js
│ │ └── userRoute.js
│ ├── uploads/ # Uploaded files
│ ├── server.js # Main server entry point
│ ├── .env
│ └── package.json
│
├── frontend/
│ ├── public/
│ │ └── index.html
│ ├── src/
│ │ ├── assets/ 
│ │ │ └── dp.svg
│ │ ├── components/ # UI Components
│ │ │ ├── Banner.jsx
│ │ │ ├── Footer.jsx
│ │ │ ├── Header.jsx
│ │ │ ├── Navbar.jsx
│ │ │ ├── RelatedDoctors.jsx
│ │ │ ├── SpecialityMenu.jsx
│ │ │ ├── TopDoctors.jsx
│ │ │
│ │ ├── context/ 
│ │ │ └── AppContext.js
│ │ ├── pages/ 
│ │ │ ├── About.jsx
│ │ │ ├── Appointment.jsx
│ │ │ ├── Contact.jsx
│ │ │ ├── Doctor.jsx
│ │ │ ├── Home.jsx
│ │ │ ├── Login.jsx
│ │ │ ├── MyAppointments.jsx
│ │ │ └── MyProfile.jsx
│ │ ├── App.jsx
│ │ ├── index.css
│ │ └── main.jsx # React entry point
│ ├── .env
│ ├── package.json
│ ├── tailwind.config.js
│ └── vite.config.js
│
├── package.json 
└── README.md

