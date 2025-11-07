# Smart Policy & Document Validator  
A full-stack web application that validates uploaded documents (policy papers, KYC files, legal forms) for completeness, required fields, blur level, and basic formatting.  
Built using **FastAPI**, **React**, **PostgreSQL**, **Docker**, and deployed on **AWS**.

---

## 🚀 Features

### ✅ Document Upload & Processing
- Upload PDF or image documents.
- Extract text using rule-based parsing.
- Detect missing required fields (e.g., Name, Address, Policy No).
- Validate page count.
- Check document clarity using blur detection (OpenCV).

### ✅ Document Validation Rules
- Required fields detection via regex/string search.
- Page count validation.
- Blurry/low-quality document detection.
- Corrupted/incomplete PDF handling.

### ✅ Backend (FastAPI)
- `/upload` → Upload document for validation  
- `/history` → Fetch past validations  
- `/document/:id` → Get full validation details  

### ✅ Frontend (React)
- Simple file upload UI  
- Display:
  - Validation status (Pass/Fail)
  - Missing fields
  - Page info
  - Blur score
  - Suggestions  

### ✅ Database (PostgreSQL)
Stores:
- File metadata
- Extracted text
- Missing fields
- Validation status (PASS/FAIL)
- Timestamps

### ✅ DevOps
- Fully Dockerized (FastAPI + PostgreSQL)
- AWS S3 for file storage
- Deployed on AWS EC2 (Docker container)
- Environment variables supported for production

---

## 🏗️ Tech Stack

### 🔹 Backend
- FastAPI  
- PyPDF2 / pdfplumber  
- OpenCV (blur detection)  
- Regex for rule-based validation  

### 🔹 Frontend
- React (minimal UI)
- Axios

### 🔹 Database
- PostgreSQL

### 🔹 Deployment / DevOps
- Docker & Docker Compose
- AWS EC2
- AWS S3 (optional but recommended)

---

## 📁 Project Structure

