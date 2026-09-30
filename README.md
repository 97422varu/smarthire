<div align="center">

# 🤖 SmartHire: AI Resume Intelligent System

**AI-powered platform for resume analysis, ATS scoring, job matching, and interview preparation**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_Llama_3-F55036?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active_Development-brightgreen?style=for-the-badge)

</div>

---

## 📌 Overview

- SmartHire simplifies the **job search and hiring process** with AI
- Analyzes resumes, matches them to job descriptions, and finds missing skills
- Gives AI-based recommendations and interview preparation
- Combines **resume parsing, NLP, LLM APIs, ATS-style analysis, and job matching** in one platform

---

## ✨ Key Features

### 📄 Resume Analysis
- Upload and analyze resumes
- Extract skills, education, experience, projects, and certifications
- Generate an AI-powered resume summary
- Identify strengths and improvement areas

### 📊 ATS Resume Scoring
- Analyze resumes using ATS-oriented criteria
- Generate an overall resume score
- Detect missing or weak sections
- Suggest improvements for ATS compatibility

### 🎯 Job Description Matching
- Compare resumes with job descriptions
- Calculate candidate-job match score
- Identify matching and missing skills
- Highlight key job requirements

### 💡 AI Career Recommendations
- Suggest relevant skills for the target role
- Provide personalized improvement tips
- Recommend suitable jobs based on the candidate profile

### 🎤 Interview Preparation
- Technical questions
- HR questions
- Aptitude questions
- Role-specific questions

### 🧰 AI Resume & Career Tools
- Resume summary generation
- Cover letter generation
- Portfolio content generation
- Career recommendations

### 💬 AI Chatbot
- Voice-enabled assistant
- Career guidance
- Resume and job-search help
- Interactive candidate support

### 📈 Candidate Dashboard
- Resume analysis
- ATS score
- Job match results
- Recommended jobs
- Missing skills
- Interview preparation
- Career recommendations

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │        User         │
                    │  Resume / Job Data  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   React Frontend    │
                    │   User Dashboard    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  Node.js + Express  │
                    │       Backend       │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
      Resume Parsing      NLP Analysis        Database
             │                 │                 │
             └─────────────────┼─────────────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    AI / LLM API     │
                    │    Groq Llama 3     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   AI Results &      │
                    │   Recommendations   │
                    └─────────────────────┘
```

---

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| **React.js** | Frontend and user interface |
| **Node.js** | Backend runtime |
| **Express.js** | REST API development |
| **Python** | AI and data-processing tasks |
| **Flask** | Python API services |
| **NLP** | Resume and job-description analysis |
| **Groq Llama 3** | AI-powered generation and analysis |
| **JavaScript** | Application logic |
| **HTML & CSS** | Frontend structure and styling |
| **Database** | Candidate and application data |
| **Git & GitHub** | Version control |

---

## 🔄 Project Workflow

```text
Resume Upload
      ↓
Resume Parsing
      ↓
Information Extraction
      ↓
Skills & Profile Analysis
      ↓
ATS Score Generation
      ↓
Job Description Matching
      ↓
Missing Skills Detection
      ↓
AI Recommendations
      ↓
Interview Preparation
      ↓
Career & Job Recommendations
```

---

## 🔬 How It Works

### 📑 Resume Processing
- Extracts personal information
- Extracts technical skills
- Extracts education and work experience
- Extracts projects, certifications, and achievements
- Uses the data for ATS analysis, job matching, interview prep, and recommendations

### 🎯 AI-Powered Job Matching
- Compares candidate data with the job description
- Evaluates:
  - Required vs candidate skills
  - Educational requirements
  - Experience requirements
  - Role-specific keywords
  - Overall profile compatibility
- Returns a **job match score** with improvement areas

### 🎤 Interview Preparation

| Type | Topics |
|---|---|
| **Technical** | Programming, data structures, databases, web development, AI/ML, resume projects |
| **HR** | Introduction, strengths & weaknesses, career goals, teamwork, problem solving, project experience |
| **Aptitude** | Role-relevant aptitude and reasoning practice |

---

## 🖼️ Screenshots

<!-- Add screenshots here -->
<!-- ![Dashboard](images/dashboard.png) -->
<!-- ![ATS Score](images/ats-score.png) -->
<!-- ![Job Match](images/job-match.png) -->
<!-- ![Interview Prep](images/interview-prep.png) -->

---

## 📁 Project Structure

```text
SmartHire/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── services/
│   ├── models/
│   └── server.js
│
├── python/
│   ├── resume_parser/
│   ├── nlp/
│   └── ai_services/
│
├── uploads/
├── README.md
├── package.json
└── .gitignore
```

> The exact folder structure may vary with the current implementation.

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/SmartHire.git
cd SmartHire
```

### 2️⃣ Install Frontend Dependencies

```bash
cd frontend
npm install
```

### 3️⃣ Install Backend Dependencies

```bash
cd ../backend
npm install
```

### 4️⃣ Install Python Dependencies

```bash
python -m venv venv
venv\Scripts\activate        # Windows
pip install -r requirements.txt
```

### 5️⃣ Configure Environment Variables

Create a `.env` file:

```env
PORT=5000
GROQ_API_KEY=your_groq_api_key
DATABASE_URL=your_database_connection
```

> ⚠️ Never commit API keys, passwords, or database credentials to GitHub.

### 6️⃣ Start the Backend

```bash
npm start
```

### 7️⃣ Start the Frontend

```bash
cd frontend
npm start
```

- Open the local URL shown in the terminal

---

## 🔌 API Modules

```text
/api/resume
/api/jobs
/api/ai
/api/interview
/api/portfolio
/api/chat
```

> Endpoints may change as the project evolves.

---

## 🧠 AI Integration

- Uses an **LLM API (Groq Llama 3)** for career-related generation and analysis
- **Capabilities:**
  - Resume analysis and summaries
  - Skill recommendations
  - Job matching assistance
  - Interview question generation
  - Cover letter generation
  - Portfolio content generation
  - Career guidance
- **Prompt engineering** is used for structured, role-specific responses

---

## 🔒 Security Considerations

- API credentials stored in environment variables
- `.gitignore` for sensitive files
- Backend API validation
- Controlled file uploads
- Separate frontend and backend services

**For production, add:**
- Authentication and authorization
- Rate limiting
- File validation
- Secure database configuration

---

## 🔮 Future Enhancements

- User authentication and role-based access
- Advanced ATS scoring
- Semantic job matching
- Job application tracking
- LinkedIn profile analysis
- AI-generated portfolio hosting
- Resume template generation
- SOP generation
- Personalized learning roadmaps
- AI interview simulation
- Voice-based mock interviews
- Recruiter dashboard
- Candidate ranking and filtering
- Cloud deployment

---

## 🎯 Project Goals

- Help users understand their **resume quality**
- Identify **missing skills**
- Find **suitable job opportunities**
- Improve resumes with AI feedback
- Prepare for **interviews**
- Build a stronger **professional profile**

---

## 🧠 Learning Outcomes

- Full-stack development (React, Node.js, Express)
- REST API design and integration
- Python-based processing
- Natural Language Processing
- Prompt engineering and AI API integration
- Resume parsing
- Database management
- Git & GitHub
- End-to-end project development

---

## 🚧 Project Status

- **Status:** Active Development
- Continuously improved with new AI features and career tools

---

## 👤 Author

**Varunasiddesha H E**
Bachelor of Engineering, Computer Science & Engineering
Sambhram Institute of Technology

[LinkedIn](https://linkedin.com/in/your-profile) · [GitHub](https://github.com/your-username)

---

## 📄 License

- Developed for educational, internship, and portfolio purposes

<div align="center">

⭐ If you found this project useful, consider giving it a star!

</div>
