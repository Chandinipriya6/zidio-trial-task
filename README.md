# 📄 Resume Builder App — Zidio Trial Task

## 🚀 Project Overview
This is a full-stack **Resume Builder Application** that allows users to create, customize, and manage their resumes easily.  
It includes secure authentication with email verification, multiple templates, QR code access, and resume history management.

---

## ✨ Key Features

- 🔐 **User Authentication**
  - Users can register and receive a **verification email**.
  - Clicking the verification link activates the account and redirects to the login page.

- 🧑‍💼 **Resume Creation**
  - Users can enter their personal, educational, and professional details.
  - Select from multiple **resume templates**.
  - Instantly **preview** the selected design before saving.

- 📄 **PDF Download**
  - Generate and download the resume in **PDF format** with one click.

- 🔗 **QR Code Integration**
  - Each resume includes a **QR code**.
  - Scanning the QR code opens the digital version of the resume online.

- 🕓 **Resume History**
  - Users can view all their previously created resumes.
  - Option to **view, edit, and update** resumes anytime.

---

## 🧠 My Approach

The focus was on building a **complete, user-friendly, and functional platform** where:
- Authentication and verification flow ensure security.
- Template selection and preview provide flexibility.
- PDF and QR code features enhance usability.
- A clean UI ensures a seamless experience.

---

## 🛠️ Tech Stack

**Frontend:** React.js, HTML, CSS, JavaScript  
**Backend:** Node.js, Express.js  
**Database:** MongoDB  
**Other Tools:** Nodemailer (for email verification), QRCode library, HTML-to-PDF generation  

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Chandinipriya6/zidio-trial-task.git
   cd zidio-trial-task
Install dependencies

bash
Copy code
cd backend && npm install
cd ../frontend && npm install
Set environment variables
Create .env files in backend and frontend with:

ini
Copy code
MONGO_URI=your_mongodb_connection_string
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
JWT_SECRET=your_jwt_secret
Run the app

bash
Copy code
cd backend
npm start
Then open another terminal:

bash
Copy code
cd frontend
npm start
🔍 What I Would Improve
If given more time, I would:

Add AI-powered suggestions to improve resume content.

Include drag-and-drop sections for better customization.

Integrate cloud storage for saving and sharing resumes securely.

Add dark mode and more professional templates.

📨 Zidio Submission Note
This project was developed as part of the Zidio Development Trial Task to demonstrate full-stack web development skills — combining authentication, database integration, file generation, and responsive UI design.

👩‍💻 Author
Pasagada Chandini Priya
📧 [chandini.priya@example.com]
🌐 [LinkedIn or Portfolio link if you want to add]

yaml
Copy code

---

Would you like me to include your **actual LinkedIn profile or GitHub Pages live demo link** in the “Author” section before you push this to GitHub?  
That makes your submission more professional when Zidio reviews it.






You said:
the data base of supabase


ChatGPT said:
Perfect 👍 — since your Resume Builder project uses Supabase (not MongoDB), we’ll update your README to correctly reflect that.

Here’s the corrected and complete version 👇

markdown
Copy code
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
Install dependencies

bash
Copy code
cd backend && npm install
cd ../frontend && npm install
Create a .env file in the backend directory:

bash
Copy code
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
GEMINI_API_KEY=your_gemini_api_key
BACKEND_URL=http://localhost:5000
SUPABASE_TEMPLATE_URL=https://your-supabase-template-bucket-url/
Run the app

bash
Copy code
# Start backend
cd backend
npm start

# Start frontend (in another terminal)
cd ../frontend
npm start
Access the app
Open your browser and go to:

arduino
Copy code
http://localhost:3000
🧩 Database Schema (Supabase)
Table: resumes

Column Name	Type	Description
id	UUID (PK)	Unique resume ID
user_id	UUID (FK)	Linked to Supabase Auth users
name	Text	User’s full name
email	Text	User’s email
summary	Text	Short profile summary
education	JSONB	Array of education entries
experience	JSONB	Array of work experiences
skills	JSONB	List of user skills
custom_sections	JSONB	Extra sections (optional)
template_url	Text	Link to selected template HTML
created_at	Timestamp	Created date

🔍 What I Would Improve
If given more time, I would:

Add AI-based resume optimization using Gemini API.

Implement custom template builder for more personalization.

Integrate analytics (views/downloads per resume).

Add public sharing links with access controls.

📨 Zidio Submission Note
This project was developed as part of the Zidio Development Trial Task to demonstrate skills in:

Full-stack web development (React + Node + Supabase)

Authentication and email verification

Dynamic data rendering and PDF generation

Clean and responsive frontend design
