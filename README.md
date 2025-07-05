# 🎓 InternHub – Internship Management Platform

InternHub is a simple, role-based web app that connects students looking for internships with companies offering them. Students can explore available positions, apply directly, and track their application status. Companies can post internships, manage listings, and review applications.

The focus is on clean UI, smooth user experience, and clear separation between student and company access.

👤 **Roles**
- Students: Apply for internships and track applications  
- Companies: Post internships and review applicants

## 📑 Table of Contents
- [Overview](#-internhub--internship-management-platform)
- [User Roles](#user-roles)
- [✅ Features Checklist](#-features-checklist)
  - [👨‍🎓 Student Features](#-student-features)
  - [🏢 Company Features](#-company-features)
  - [⚙️ System Features](#️-system-features)
- [🚀 Getting Started](#-getting-started)
- [🧱 Tech Stack](#-tech-stack)
- [📸 Screenshots](#-screenshots)
- [🤝 Team & Contributions](#-team--contributions)
- [📝 License](#-license)

## 👥 User Roles

InternHub has two main roles:

- **Student** – apply for internships and track applications  
- **Company** – post internships and review applicants

## ✅ Features Checklist

### 👨‍🎓 Student Features
- Register and log in as a student
- Browse available internship listings
- Filter and search for internships
- View internship details
- Apply to internships with resume upload
- Track past applications status

### 🏢 Company Features
- Register and log in as a company
- Post new internship opportunities
- Edit and delete existing postings
- View list of student applications
- Review applicant details and resumes
- Change application status (e.g., Accepted, Rejected)

### ⚙️ System Features
- Fully containerized using Docker
- Frontend built with Angular
- Backend built with Django
- Uses MinIO for file storage
- PostgreSQL database

## 🚀 Getting Started

InternHub runs fully on Docker. You don't need to clone the code or build anything locally.

### 🛠 Prerequisites
- Docker installed on your machine: [Install Docker](https://docs.docker.com/get-docker/)

### 🧪 Run the Containers

You can start all three services using the following commands:

```bash
# Frontend (Angular)
docker run -p 4200:4200 7sn8k/innotern-frontend

# Backend (Django)
docker run -p 8000:8000 7sn8k/api-django

# MinIO (File Storage)
docker run -p 9000:9000 -p 9001:9001 7sn8k/minio
```

### 🌐 Access the app

- Frontend: http://localhost:4200  
- Backend API: http://localhost:8000  
- MinIO Console: http://localhost:9001

> Make sure ports `4200`, `8000`, `9000`, and `9001` are not used by other apps.

## 🧱 Tech Stack

InternHub is built using a modern, containerized full-stack setup:

### 🌐 Frontend
- **Angular** – SPA for students and companies
- **Tailwind CSS** – utility-first styling

### ⚙️ Backend
- **Django** – RESTful API and business logic
- **PostgreSQL** – relational database for users, internships, and applications

### 🗂 Storage
- **MinIO** – S3-compatible object storage used for storing resumes and cover letters

### 📦 Infrastructure
- **Docker** – all services run as containers
- Public Docker Hub images:
  - [`7sn8k/innotern-frontend`](https://hub.docker.com/r/7sn8k/innotern-frontend)
  - [`7sn8k/api-django`](https://hub.docker.com/r/7sn8k/api-django)
  - [`7sn8k/minio`](https://hub.docker.com/r/7sn8k/minio)

## 📸 Screenshots

Here’s a quick look at some key parts of InternHub in action:

### 🏠 Student Dashboard  
*Browse internships, view listings, and track application status.*

![Student Dashboard](screenshots/student-dashboard.png)

### 📋 Internship Listing  
*Detailed view of a specific internship with option to apply.*

![Internship Listing](screenshots/internship-listing.png)

### 📄 Application Form  
*Resume and cover letter upload with confirmation feedback.*

![Application Form](screenshots/application-form.png)

### 🏢 Company Dashboard  
*Overview of posted internships and applicant summaries.*

![Company Dashboard](screenshots/company-dashboard.png)

### 🧾 Applicant Viewer  
*Review student submissions and update application status.*

![Applicant Viewer](screenshots/applicant-viewer.png)

### ☁️ MinIO File Console  
*S3-style file browser for resumes and cover letters.*

![MinIO Console](screenshots/minio-console.png)

### 🖼 Additional Images

To share extra UI shots, development previews, or miscellaneous views, add them to:

```bash
/screenshots/misc/
```

> All screenshot files should go inside `/screenshots/` or its subfolders.

## 🤝 Team & Contributions

InternHub was developed as a collaborative project. Here are the team members who brought it to life:

| Name             | Role                 |
|------------------|----------------------|
| [Your Name]      | Full-Stack Developer |
| [Member 2 Name]  | Frontend Developer   |
| [Member 3 Name]  | Backend Developer    |
| [Member 4 Name]  | DevOps & Testing     |

> 🛑 **Note**: This project is currently not open to external contributions.

## 📝 License

This project does not yet have an open-source license.  
All rights reserved by the team.
