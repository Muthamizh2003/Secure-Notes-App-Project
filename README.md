Secure Notes App

Secure Notes is a privacy-focused note-taking application built with Spring Boot, React.js, MySQL, and AWS. It provides end-to-end encryption, multi-factor authentication (MFA), and OAuth 2.0 login to securely store and manage your personal and professional notes.

🔗 http://secure-notes-app-v1.s3-website.ap-south-1.amazonaws.com/

Features

Encrypted Notes: End-to-end encrypted notes stored securely in the database.

User Authentication:

Secure login/signup with Spring Security

Multi-Factor Authentication (MFA) for added security

OAuth 2.0 login (Google, GitHub) for easy access

Organized & Searchable: Categorize and search notes efficiently.

Responsive UI: Smooth, mobile-friendly interface built with React.js.

Cloud-Ready: Hosted on AWS for reliability and scalability.

Tech Stack

Frontend: React.js

Backend: Spring Boot, Spring Security, OAuth 2.0

Database: MySQL

Cloud/Hosting: AWS

Quick Setup
Backend
cd backend
# Configure MySQL and OAuth 2.0 client credentials in application.properties
mvn spring-boot:run

Frontend
cd frontend
npm install
npm start

API Endpoints (JWT Secured)

POST /api/auth/signup → Signup

POST /api/auth/login → Login

POST /api/auth/mfa-verify → MFA verification

POST /api/notes → Create note

GET /api/notes → Get all notes

PUT /api/notes/{id} → Update note

DELETE /api/notes/{id} → Delete note

OAuth 2.0 login endpoints are integrated for third-party authentication.

Security Highlights

MFA: Adds an extra layer of security via OTP or authenticator apps.

OAuth 2.0: Allows users to log in securely using trusted providers.

JWT Tokens: Secure API access with token-based authentication.
