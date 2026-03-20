# AI-Adaptive Onboarding Engine
A full-stack web application that analyzes a candidate's resume against a job description to identify skill gaps and generate a personalized learning roadmap.

Features
1. File Upload: Supports PDF and text files for both Resume and Job Description.
2. NLP Extraction: Uses regex-based simple NLP to extract skills from text.
3. Gap Analysis: Identifies missing or partial skills with a confidence score.
4. Reasoning Trace: Explains why a specific learning module was recommended.
5. Adaptive Roadmap: Generates a timeline UI for learning steps (skips basics if skill is partially present).

Tech Stack
1. Frontend: React, Tailwind CSS
2. Backend: Node.js, Express
3. Libraries: pdf-parse (PDF reading), multer (File uploads)

Setup Instructions
Prerequisites
1. Node.js (v14+)
2. npm

Installation
1. Clone the repository:-
git clone <repository-url>, then cd ai-onboarding-engine

2. Setup Backend
cd backend,
npm install,
npm start
Server will run on http://localhost:5000

3. Setup Frontend
Open a new terminal:
cd frontend,
npm install,
npm start
React app will run on http://localhost:3000

Usage
1. Open http://localhost:3000 in your browser.
2. Upload a Resume file (PDF/TXT).
3. Upload a Job Description file (PDF/TXT).
4. Click "Analyze & Generate Roadmap".
5. View extracted skills, confidence scores, and the recommended learning path.

Notes
1. The skill list and learning paths are hardcoded in backend/data/skillData.js.
2. Confidence scores are calculated based on the frequency of skill mentions relative to the Job Description.