# 🩺 MediScan AI

An advanced AI-powered medical imaging diagnostic platform built with Streamlit and Google Gemini AI. MediScan AI provides intelligent analysis of medical scans (X-rays, MRIs) with real-time anomaly detection, clinical report generation, and comprehensive patient management.

![MediScan AI](https://img.shields.io/badge/AI-Powered-blue) ![Python](https://img.shields.io/badge/Python-3.8+-green) ![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red)

## ✨ Features

### 🔍 Visual Scan Analysis
- **AI-Powered Image Analysis**: Upload X-rays or MRI scans for instant AI analysis
- **Anomaly Detection**: Automatic detection and highlighting of medical anomalies
- **Real-time Annotation**: Visual bounding boxes around detected conditions
- **Multi-organ Support**: Analyzes lungs, heart, bones, brain, and more

### 📄 Clinical Report Generation
- **Deep Clinical Analysis**: Comprehensive medical narrative generation
- **Risk Assessment**: Automated risk percentage calculation
- **PDF Export**: Professional medical reports with annotated images
- **Specialist Routing**: Automatic assignment to appropriate medical departments

### 🤖 Doctor AI Assistant
- **Interactive Consultation**: Chat with AI for diagnosis clarification
- **Treatment Recommendations**: Evidence-based treatment suggestions
- **Differential Diagnosis**: Explore alternative diagnoses
- **Medical Literature Integration**: Responses backed by medical knowledge

### 👨‍⚕️ Doctor Portal
- **Secure Authentication**: Role-based access for medical professionals
- **Patient Registry**: Comprehensive patient record management
- **Department Filtering**: View patients by specialization
- **Status Tracking**: Monitor patient progress (Pending/Reviewed/Discharged)

### 📊 Analytics Dashboard
- **Department Statistics**: Patient distribution across specializations
- **Age Demographics**: Visual age distribution analysis
- **Performance Metrics**: Track diagnostic efficiency
- **Real-time Updates**: Live dashboard with current statistics

### 👥 Credits & Team
- **Team Profiles**: LinkedIn-style circular profile display
- **Privacy-First**: Base64 encoded images for data security
- **Professional Layout**: Glassmorphism design with hover effects

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8 or higher
pip (Python package manager)
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/mediscan-ai.git
cd mediscan-ai
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Set up environment variables**

Create a `.env` file in the root directory:
```env
GEMINI_API_KEY=your_google_gemini_api_key_here
```

To get a Gemini API key:
- Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
- Create a new API key
- Copy and paste it into your `.env` file

4. **Run the application**
```bash
streamlit run medi_scan_app.py
```

5. **Access the app**
Open your browser and navigate to `http://localhost:8501`

## 📁 Project Structure

```
mediscan-ai/
├── medi_scan_app.py      # Main Streamlit application
├── patient_db.py         # Patient database management
├── pdf_gen.py            # PDF report generation
├── utils.py              # Utility functions
├── doctor_portal.py      # Doctor authentication & portal
├── assests/              # Base64 encoded team images
│   ├── professor.txt
│   ├── student1.txt
│   └── student2.txt
├── patient_data.json     # Patient records database
├── .env                  # Environment variables (create this)
├── requirements.txt      # Python dependencies
└── README.md            # This file
```

## 🛠️ Technology Stack

- **Frontend**: Streamlit (Python web framework)
- **AI/ML**: Google Gemini 2.5 Flash Lite
- **Image Processing**: PIL (Python Imaging Library)
- **PDF Generation**: ReportLab
- **Data Storage**: JSON-based database
- **Styling**: Custom CSS with Glassmorphism design

## 💡 Usage Guide

### For Patients/Technicians

1. **Upload Medical Scan**
   - Navigate to "🔍 Visual Scan" tab
   - Upload X-ray or MRI image (JPG, PNG, JPEG)
   - Click "🚀 Run Diagnostic Scan"

2. **View Analysis**
   - AI will detect and highlight anomalies
   - Review detected conditions and severity levels

3. **Generate Report**
   - Go to "📄 Clinical Report" tab
   - Click "⚡ Generate Clinical Narrative"
   - Download PDF report for records

### For Doctors

1. **Login**
   - Navigate to "👨‍⚕️ Doctor Portal" tab
   - Enter credentials (Demo: username: `doc`, password: `123`)

2. **Review Patients**
   - View all patient records in your department
   - Update patient status
   - Access full diagnostic reports

3. **Consult AI**
   - Use "🤖 Doctor AI" tab for consultation
   - Ask questions about diagnosis
   - Get treatment recommendations

## 🔐 Security Features

- **Base64 Image Encoding**: Team photos stored securely
- **Role-based Access**: Separate portals for doctors and patients
- **Data Privacy**: Local JSON storage with no external data sharing
- **Secure Authentication**: Password-protected doctor portal

## 📊 Sample Credentials

**Doctor Portal Access:**
- Username: `doc` | Password: `123` (General)
- Username: `cardio` | Password: `123` (Cardiologist)
- Username: `ortho` | Password: `123` (Orthologist)

## 🎨 Design Philosophy

MediScan AI features a modern, professional interface with:
- **Dark Navy Theme**: Easy on the eyes for long sessions
- **Glassmorphism Effects**: Modern, translucent card designs
- **Responsive Layout**: Works on desktop and tablet devices
- **Intuitive Navigation**: Tab-based workflow for easy access

## 🤝 Contributing Team

### 👨‍🏫 Mentor
**Dr. Ashish Kumar Diwedi**
- Assistant Professor @ LNMIIT
- Project Mentor & Guide

### 👨‍💻 Developers
**Satvik Gupta**
- Software Developer
- B.Tech CSE @ LNMIIT

**Naman Agrawal**
- AI/ML Engineer
- B.Tech MME @ LNMIIT

## 📝 License

This project is developed as an academic project at LNMIIT (The LNM Institute of Information Technology).

© Nov-2025, mediscan-health, Inc. or its affiliates

## 🐛 Known Limitations

- **Simulation Mode**: When Gemini API is unavailable, uses mock data
- **Single User**: Currently supports one session at a time
- **Local Storage**: Data stored locally in JSON format
- **Demo Credentials**: Uses simplified authentication for demonstration

## 🔮 Future Enhancements

- [ ] Multi-user support with proper authentication
- [ ] Database integration (PostgreSQL/MongoDB)
- [ ] DICOM format support
- [ ] 3D scan visualization
- [ ] Mobile app version
- [ ] Multi-language support
- [ ] Integration with hospital management systems
- [ ] Advanced analytics and reporting

## 📞 Support

For questions or issues, please contact the development team or create an issue in the repository.

## 🙏 Acknowledgments

- Google Gemini AI for powerful image analysis
- Streamlit for the amazing web framework
- LNMIIT for academic support and resources
- All contributors and testers

---

**Built with ❤️ using Streamlit & Google Gemini AI**

*Disclaimer: This is an educational project and should not be used for actual medical diagnosis without proper validation and regulatory approval.*
