# Deep-Learning--Based-Seizure-Detection-From-EEG-Signals
Epilepsy Detection Using EEG Signals A research-driven diagnostic system leveraging Machine Learning for automated epilepsy detection from EEG data. This web-based tool integrates CNN and RNN models to analyze seizure-related patterns in EEG recordings, providing fast and reliable predictions.

#Core Highlights
> FastAPI Backend Architecture — Lightweight, high-performance Python backend managing EEG file uploads, model inference, and user sessions.
> ResNet Deep Learning Model — Trained on TUH EEG dataset for seizure classification, integrated directly into the backend for local inference.
> EEG Processing Pipeline — Preprocessing (filtering, normalization), feature extraction, and model evaluation handled in Python.
> Interactive Web Interface — React frontend for EEG upload, visualization, and displaying model predictions in real-time.
> Secure Storage & Reporting — Persistent file storage on Render Disk and PostgreSQL metadata tracking with downloadable files and reports.
> End-to-End Deployment on Render — Frontend, backend, and database hosted on a single Render setup for low-latency communication.

#Tech Stack
Layer	Technologies Used
 Frontend	React.js (TypeScript, Vite)
> Backend	FastAPI (Python)
> ML Model	TensorFlow / PyTorch (ResNet Architecture)
> Database	PostgreSQL (via Render)
> File Storage	Render Persistent Disk
> Security	JWT Authentication, bcrypt Password Hashing

# Goals
Automate seizure detection using a trained ResNet model on EEG signals
Offer an accessible diagnostic tool for low-resource clinical setups
Provide interpretable model outputs and automated report generation
Demonstrate full-stack ML deployment in a real-world healthcare use case

#System Workflow
User Login → Secure, role-based access for clinicians or researchers
EEG Upload → Users upload .edf or .csv EEG data files
Model Inference → FastAPI backend runs the ResNet model for seizure detection
Visualization → Frontend plots EEG signals and highlights detected seizure zones
Reporting → Backend generates detailed diagnostic reports stored on Render Disk

#Security Features
JWT Authentication: Secure token-based authentication
CORS Protection: Environment-based CORS configuration
Trusted Host Validation: Production mode host header validation
Password Hashing: bcrypt for secure password storage

# Deployment Overview (Render)
Component	Deployment Type	Description
Frontend	Render Web Service	React-based interface
Backend	Render Web Service	FastAPI app exposing REST endpoints
Database	Render PostgreSQL	Stores user data, reports, and metadata
File Storage	Render Persistent Disk	Stores EEG files and generated reports
Continuous Deployment:
Every push to the GitHub main branch automatically triggers a new build and deploy on Render.

# Deployment Documentation
For detailed deployment instructions, see:

RENDER_DEPLOYMENT.md - Complete step-by-step deployment guide
DEPLOYMENT_CHECKLIST.md - Quick deployment checklist
MODEL_STORAGE_GUIDE.md - Guide for storing ML models on Render disk
Quick Start:

Create PostgreSQL database on Render
Deploy backend service (see RENDER_DEPLOYMENT.md)
Deploy frontend service
Configure CORS and environment variables
Run database migrations
Create initial admin user

🎓 Developed By
👨‍💻 Anshu Kumar Shaw
🏫 Quantum University, Roorkee, Uttarakhand
🗓️ Session 2023–2027
