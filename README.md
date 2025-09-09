HealthMate Web API

HealthMate is a graduation project — a healthcare management system built with ASP.NET Core 8.0.
This API is part of the larger HealthMate System, which also includes a web application for healthcare providers and a mobile app for patients.
👉 Check out the HealthMate Website Repository here: HealthMate Website Repo

It provides APIs for patient records, encounters, lab tests, medical documents, mental health assessments, and AI-powered decision support.

🚀 Features

User Management: Patients, Healthcare Providers, and Admins with JWT authentication

Medical Records: FHIR-compliant patient data storage

Encounters: Track visits, conditions, and treatments

Lab Tests: Manage lab orders and results

Documents: Store medical images and prescriptions

AI Integration:

Emergency Department health assessment engine

Sina chatbot powered by Google Gemini AI

Mental Health: Mood and anxiety assessments

Messaging: Real-time patient–provider communication

🛠️ Tech Stack

Backend: ASP.NET Core 8.0 (Web API)

Database: SQL Server with Entity Framework Core

Auth: ASP.NET Identity + JWT tokens

AI: Google Gemini API

Docs: Swagger / OpenAPI

Testing: xUnit

📦 Dependencies

EF Core

EF Core SQL Server provider

ASP.NET Core Identity + JWT

Swagger (Swashbuckle)

⚙️ Getting Started
Prerequisites

.NET 8 SDK

SQL Server (LocalDB or full instance)

Visual Studio 2022 or VS Code

Google Gemini API key (for AI features)

Setup
# 1. Clone repo
git clone <repo-url>
cd HealthMate

# 2. Restore packages
dotnet restore

# 3. Update connection string in appsettings.json

# 4. Apply migrations
dotnet ef database update

# 5. Run the app
dotnet run --project src/HealthMate


Visit Swagger UI at:
👉 https://localhost:5001/swagger

🔒 Security

JWT-based authentication

Role-based authorization

File validation for uploads (JPG/PNG, max 2MB)

CORS enabled for cross-origin requests

👥 User Roles

Patient: Access to personal records and encounters

Provider: Manage assigned patients and treatments

Admin: Full access and system control

📄 License

MIT License – open for contributions.
