# 📄 Resume Builder App — Zidio Trial Task

## 🚀 Project Overview
This is a full-stack **Resume Builder Application** built with React.js and Node.js, using **Supabase** for authentication and database storage.  
It allows users to securely register, verify their account via email, create and manage resumes, choose templates, generate PDFs, and share them via QR codes.

---

## ✨ Key Features

- 🔐 **User Authentication (Supabase)**
  - Users can sign up using their email and receive a **verification email** from Supabase.
  - Once verified, users can log in and access their dashboard.

- 🧾 **Resume Builder**
  - Create resumes by entering personal, educational, and professional details.
  - Select from multiple **HTML templates** stored in Supabase.
  - Preview the resume before saving or downloading.

- 📄 **PDF Download**
  - Resumes can be exported as **PDF files** using backend rendering.

- 🔗 **QR Code Integration**
  - Every generated resume includes a **QR code**.
  - Scanning the QR code opens the resume in the browser instantly.

- 🕓 **Resume History**
  - Users can view all saved resumes.
  - Edit, update, or delete resumes anytime from the dashboard.

---

## 🧠 My Approach

The main goal was to create a **secure and flexible platform** that:
- Uses **Supabase Auth** for email verification and secure access.
- Stores resume data and templates efficiently in **Supabase Database**.
- Generates dynamic resumes that can be downloaded or shared.
- Offers an intuitive and responsive user experience.

---

## 🛠️ Tech Stack

**Frontend:** React.js, HTML, CSS, JavaScript  
**Backend:** Node.js, Express.js  
**Database & Auth:** Supabase  
**File Storage:** Supabase Storage  
**Email Verification:** Supabase built-in Auth service  
**Other Tools:** QRCode library, Axios, HTML-to-PDF renderer  

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Chandinipriya6/zidio-trial-task.git
   cd zidio-trial-task


2. **Install dependencies**

   ```bash
   cd backend && npm install
   cd ../frontend && npm install
   ```

3. **Create a `.env` file** in the backend directory:

   ```bash
   SUPABASE_URL=your_supabase_project_url
   SUPABASE_ANON_KEY=your_supabase_anon_key
   SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
   GEMINI_API_KEY=your_gemini_api_key
   BACKEND_URL=http://localhost:5000
   SUPABASE_TEMPLATE_URL=https://your-supabase-template-bucket-url/
   ```

4. **Run the app**

   ```bash
   # Start backend
   cd backend
   npm start

   # Start frontend (in another terminal)
   cd ../frontend
   npm start
   ```

5. **Access the app**
   Open your browser and go to:

   ```
   http://localhost:3000
   ```

---

## 🧩 Database Schema (Supabase)

**Table: `resumes`**

| Column Name     | Type      | Description                    |
| --------------- | --------- | ------------------------------ |
| id              | UUID (PK) | Unique resume ID               |
| user_id         | UUID (FK) | Linked to Supabase Auth users  |
| name            | Text      | User’s full name               |
| email           | Text      | User’s email                   |
| summary         | Text      | Short profile summary          |
| education       | JSONB     | Array of education entries     |
| experience      | JSONB     | Array of work experiences      |
| skills          | JSONB     | List of user skills            |
| custom_sections | JSONB     | Extra sections (optional)      |
| template_url    | Text      | Link to selected template HTML |
| created_at      | Timestamp | Created date                   |

---

## 🔍 What I Would Improve

If given more time, I would:

* Add **AI-based resume optimization** using Gemini API.
* Implement **custom template builder** for more personalization.
* Integrate **analytics** (views/downloads per resume).
* Add **public sharing links** with access controls.

---

## 📨 Zidio Submission Note

This project was developed as part of the **Zidio Development Trial Task** to demonstrate skills in:

* Full-stack web development (React + Node + Supabase)
* Authentication and email verification
* Dynamic data rendering and PDF generation
* Clean and responsive frontend design

---

## 👩‍💻 Author

**Pasagada Chandini Priya**
📧 [Your Email Address]
🌐 [https://github.com/Chandinipriya6](https://github.com/Chandinipriya6)

````

---

✅ Next Steps:
1. Replace `[Your Email Address]` with your real email.  
2. Save this as `README.md` in your project root.  
3. Run:
   ```bash
   git add README.md
   git commit -m "Added detailed project README for Zidio trial"
   git push origin main
````

Would you like me to include **screenshots** or **preview GIFs** in the README (like login page, resume preview, etc.) to make your GitHub project even more impressive for Zidio?
