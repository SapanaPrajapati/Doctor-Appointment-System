# 🏥 Doctor Appointment Booking App 

This project is a full-stack web application that allows patients to book appointments with doctors online. It provides a platform for doctors to manage their profiles and schedules, and for administrators to oversee the entire system. The application aims to streamline the appointment booking process, making it more efficient and convenient for both patients and healthcare providers.

🚀 **Key Features**

*   **User Authentication:** Secure registration and login for patients, doctors, and administrators.
*   **Doctor Profiles:** Doctors can create and manage their profiles, including specialization, experience, and availability.
*   **Appointment Booking:** Patients can easily search for doctors and book appointments based on their availability.
*   **Admin Panel:** Administrators can manage users, doctors, and appointment statuses.
*   **Notifications:** Real-time notifications for appointment confirmations, cancellations, and updates.
*   **Role-Based Access Control:** Different user roles (patient, doctor, admin) have different levels of access and permissions.
*   **Loading Indicators:** Display loading indicators to improve user experience during data fetching.
*   **Profile Updates:** Users and doctors can update their profile information.

🛠️ **Tech Stack**

*   **Frontend:**
    *   React
    *   Redux Toolkit
    *   React Router DOM
    *   Ant Design
    *   Axios
    *   React Toastify
*   **Backend:**
    *   Node.js
    *   Express.js
*   **Database:**
    *   MongoDB
    *   Mongoose
*   **Authentication:**
    *   JSON Web Tokens (JWT)
    *   bcryptjs
*   **Middleware:**
    *   cors
    *   morgan
*   **Other:**
    *   dotenv
    *   colors
    *   dayjs

📦 **Getting Started / Setup Instructions**

**Prerequisites**

*   Node.js and npm installed
*   MongoDB installed and running
*   A code editor (e.g., VS Code)

**Installation**

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2.  **Install backend dependencies:**
    ```bash
    cd backend
    npm install
    ```

3.  **Install frontend dependencies:**
    ```bash
    cd doctor-appointment
    npm install
    ```

4.  **Configure environment variables:**

    *   Create a `.env` file in the `backend` directory.
    *   Add the following environment variables:

        ```
        MONGODB_URL=<your_mongodb_connection_string>
        PORT=<port_number> (e.g., 8080)
        JWT_SECRET=<your_jwt_secret>
        ```

**Running Locally**

1.  **Start the backend server:**
    ```bash
    cd backend
    npm start
    ```

2.  **Start the frontend development server:**
    ```bash
    cd doctor-appointment
    npm start
    ```

3.  **Open the application in your browser:**
    `http://localhost:3000` (or the port specified in your frontend configuration)

📂 **Project Structure**

```
├── backend/
│   ├── configure/
│   │   └── mongodb.js
│   ├── controller/
│   │   ├── adminControl.js
│   │   ├── doctor.Control.js
│   │   └── userControl.js
│   ├── middlewares/
│   │   └── authMiddleware.js
│   ├── models/
│   │   ├── appointmentModel.js
│   │   ├── doctorModel.js
│   │   └── userModel.js
│   ├── routes/
│   │   ├── adminRoute.js
│   │   ├── doctorRoute.js
│   │   └── userRoute.js
│   ├── server.js
│   └── package.json
├── doctor-appointment/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── DoctorList.js
│   │   │   ├── Layout.js
│   │   │   ├── ProtectRoute.js
│   │   │   ├── PublicRoute.js
│   │   │   └── Spinner.js
│   │   ├── pages/
│   │   │   ├── Admin/
│   │   │   │   ├── Doctors.js
│   │   │   │   └── Users.js
│   │   │   ├── Doctor/
│   │   │   │   ├── DoctorAppointmentList.js
│   │   │   │   └── Profile.js
│   │   │   ├── AppointmentList.js
│   │   │   ├── BookingPage.js
│   │   │   ├── Home_page.js
│   │   │   ├── Login.js
│   │   │   ├── Notification.js
│   │   │   └── Register.js
│   │   ├── Redux/
│   │   │   ├── features/
│   │   │   │   ├── alertSlice.js
│   │   │   │   └── userSlice.js
│   │   │   └── store.js
│   │   ├── App.js
│   │   ├── App.css
│   │   ├── index.js
│   │   └── index.css
│   ├── package.json
├── .gitignore
└── README.md
```


