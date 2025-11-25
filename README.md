# MediScan-2.0
🏥 MediScan AI - Medical Diagnostic System

MediScan AI is a comprehensive medical imaging and diagnostic suite that leverages both Generative AI (Google Gemini) and Traditional Deep Learning (DenseNet121) to analyze medical scans (X-rays, MRIs). The system features patient management, automated clinical report generation, and explainable AI visualizations.

🚀 Key Features

1. MediScan AI (Main Application)

Visual Scan: Uses Gemini 2.5 Flash to identify organs and detect anomalies with bounding boxes.

Clinical Reporting: Generates deep clinical narratives, risk percentages, and recommendations.

AI Doctor Assistant: Interactive chat for doctors to discuss diagnoses.

PDF Reports: Auto-generates downloadable PDF reports with visual evidence.

2. Deep Learning X-Ray Analyzer

Organ Classification: Uses a custom-trained DenseNet121 model to classify organs (Heart, Lungs, Bone, Brain).

Pneumonia Detection: Dedicated CNN model for pneumonia screening.

Explainable AI (XAI): Grad-CAM integration to visualize heatmap overlays showing where the model is looking.

3. Doctor Portal & Registry

Secure Login: Role-based access for Cardiologists, Orthologists, Pulmonologists, etc.

Patient Database: Searchable registry of patient records (JSON-backed mock DB).

Analytics Dashboard: Visual breakdown of patient demographics and disease distribution.

🛠️ Tech Stack

Framework: Streamlit

AI/LLM: Google Gemini (via google-generativeai)

Deep Learning: PyTorch (torchxrayvision), TensorFlow/Keras

Image Processing: OpenCV, PIL (Pillow)

Utilities: ReportLab (PDF), Pandas, NumPy

📦 Installation

Clone the Repository

git clone [https://github.com/yourusername/mediscan-ai.git](https://github.com/yourusername/mediscan-ai.git)
cd mediscan-ai


Install Dependencies
It is recommended to use a virtual environment.

pip install -r requirements.txt


Setup Environment Variables
Create a .env file in the root directory to store your API key:

GEMINI_API_KEY=your_google_gemini_api_key_here


🖥️ Usage Guide

This project contains multiple Streamlit applications for different purposes.

1. Run the Main App (MediScan GenAI)

This is the primary interface featuring the modern UI and Gemini integration.

streamlit run medi_scan_app.py


2. Run the Deep Learning Tool

This tool focuses on the PyTorch/Keras models and Grad-CAM visualizations.

streamlit run app.py


3. Run the Standalone Doctor Portal

A dedicated interface for record management.

streamlit run doctor_portal.py


🔐 Login Credentials (Demo)

The system uses mock authentication for demonstration purposes. Use the following credentials to access the Doctor Portal or restricted sections.

Application

Role

Username

Password

medi_scan_app.py

General Doctor

doc

123

medi_scan_app.py

Cardiologist

cardio

123









doctor_portal.py

General Doctor

general_doc

general123

doctor_portal.py

Cardiologist

cardio_doc

cardio123

doctor_portal.py

Orthologist

ortho_doc

ortho123

📂 Project Structure

medi_scan_app.py: The main GenAI-powered application.

app.py: The Deep Learning specific app with Grad-CAM.

xray_analyzer.py: An alternative dashboard implementation.

doctor_portal.py: Standalone portal for viewing patient records.

patient_db.py: Handles database operations (currently using in-memory list & patient_data.json).

pdf_gen.py: Generates medical PDF reports using ReportLab.

preprocessing.py: Helper functions for image normalization and Grad-CAM calculation.

densenet121_xray_classifier.py: The training script used to create the organ classifier model.

requirements.txt: List of required Python packages.

🤖 Models Used

Gemini 2.5 Flash: For general image understanding and report text generation.

DenseNet121 (CheXNet weights): Fine-tuned for organ classification.

Custom CNN: For Pneumonia binary classification.

👥 Credits

Satvik Gupta - Software Developer

Naman Agrawal - AI/ML Engineer
