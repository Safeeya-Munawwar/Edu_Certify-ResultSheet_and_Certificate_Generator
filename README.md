# 🎓 Edu Certify - Result Sheet and Certificate Generator

**Edu Certify** is a web-based application designed for educational institutes to efficiently generate academic result sheets and class certificates for students. It supports **role-based dashboards** for super admin, institute admins,  lecturers and, studnets allows **secure data management**, and provides **PDF generation** for results and certificates.

---

## 🚀 Features

- ✅ Admin & Lecturer Role Management  
- 📋 Student & Subject Management  
- 📚 Marks Entry by Lecturers  
- 🧮 Automatic GPA Calculation  
- 🏅 Class Certificate Generation (1st Class, 2nd Class, etc.)  
- 📄 PDF Download for Result Sheets & Certificates  
- 🏫 Grouped Views by Institute, Department, and Semester/Year  

---

## 🛠️ Technologies Used

### Frontend
- React (Next.js)  
- Tailwind CSS  
- jsPDF – For generating PDFs  
- Axios – For API communication  

### Backend
- Node.js  
- Express  
- MySQL / MariaDB  
- Sequelize or Raw SQL  

---

## 🔐 Roles and Permissions

| Role            | Permissions                                                             |
|-----------------|-------------------------------------------------------------------------|
| **Admin**       | Full access: manage all students, lecturers, subjects, and marks        |
| **Institute Admin** | Access limited to their institute data                              |
| **Lecturer**    | Can only manage/view students in their department within the same institute |
| **Student**     | Can view and download their specific resultsheet and certificate        |

---

## 🧑‍💻 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Safeeya-Munawwar/Edu_Certify-ResultSheet_and_Certificate_Generator.git
cd result-generator
```

---

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend/` folder with the following content:

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=results_db
```

Run the server:

```bash
npm start
```

---

### 3️⃣ Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

Visit the app at: [http://localhost:3000](http://localhost:3000)

---

### 4️⃣ Database Setup

Import the SQL schema:

```bash
mysql -u root -p < database/results_db.sql
```

Or use **phpMyAdmin** / **MySQL Workbench GUI**

---

## 📄 Result Sheet & Certificate Format

### ✅ Result Sheets Include:
- Student Name & ID  
- Subject-wise Marks & Grades  
- GPA per Semester  
- Total GPA  

### ✅ Certificates Include:
- Student Name  
- Class Classification (e.g., First Class, Second Class)  
- Institute & Department Information  

---

## 📸 Screenshots

### 🖥️ Dashboard  
![Dashboard](screenshots/main.PNG)

### 🔐 Login  
![Login](screenshots/login.PNG)

### 🧑‍💼 Admin Dashboard  
![Admin Dashboard](screenshots/admin.PNG)

### 👨‍🏫 Lecturer Dashboard  
![Lecturer Dashboard](screenshots/lecturer.PNG)

### 🎓 Student Dashboard  
![Student Dashboard](screenshots/student.PNG)

### 📄 Result Sheet PDF  
![Result Sheet](screenshots/resultsheet.PNG)

### 🏅 Certificate Generation  
![Certificate](screenshots/certificate.PNG)

---

## 📦 Dependencies

### Backend
- express  
- mysql2  
- dotenv  
- cors  
- nodemon  

### Frontend
- react  
- next.js  
- axios  
- jspdf  
- tailwindcss  

---

## 📌 Future Improvements

- 📧 Email delivery for certificates  
- 🌐 Multi-language support  
- 📊 Admin analytics dashboard  
- 🖨️ Print-optimized layouts  

---

## 🧑‍🎓 Use Cases

- Internal university/college student performance tracking  
- Auto-generation of printable result sheets and award certificates  
- Department-specific academic evaluations  

---

## 🤝 Contributing

We welcome contributions!  
Feel free to **fork** this repository and submit a **pull request** with your improvements.

---

## 📄 License

This project is licensed under the **MIT License**.

---

© 2025 Edu Certify | Built with ❤️ using React, Node.js, Express, and MySQL
