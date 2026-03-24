# Cyber Triage Tool  
### _Streamlining Digital Evidence Analysis for Faster, Tamper-Evident Investigations_

---

The Cyber Triage Tool is an automated digital forensics platform designed to collect, analyze, and report digital evidence efficiently. It accelerates investigations through automated triage, tamper-proof hashing, and court-ready reporting, ensuring reliability, speed, and legal defensibility.

---

## Tech Stack  

|         Layer        |                   Technologies |
|----------------------|----------------------------------------------------------------|
| **Frontend**         | HTML + Tailwind CSS + React.js (Dashboards)                    |
| **Backend**          | Flask (FastAPI-style routing)                                  |
| **Forensic Engine**  | Python (hashlib, os, stat, exifread, mailparser, python-magic) |
| **Database**         | SQLite                                                         |
| **Reporting**        | ReportLab                                                      |
| **Automation**       | Playwright (for browser integration)                           |
| **Version Control**  | Git & GitHub                                                   |

---

## Repository Structure
```
cyber-triage-tool/
│
├── data/
├── evidence/
│
├── modules/
│   ├── utils.py
│   ├── hshing.py
│   ├── scoring.py
│   ├── ...
│
├── scripts/
│
├── templates/
│   ├── base.html
│   ├── coc_case.html
│   ├── ...
│
├── static/
│   ├── css/
│   ├── js/
│
├── heuristics.py
├── app.py
│
├── requirements.txt
└── README.md
```

---

## Setup & Run
### 1. Clone Repository
```
cd $env:USERPROFILE\Desktop
git clone <repo-url> cyber-triage-tool
cd .\cyber-triage-tool
```

### 2. Create Virtual Environment
```
python -m venv .venv
.\.venv\Scripts\Activate
```

### 3. Install Dependencies
```
pip install --upgrade pip
pip install -r requirements.txt
python -m playwright install chromium
```

### 4. Run Application
```
python app.py
```

---

## 🧩 Core Features  

### 🔹 Ingest & Normalize  
- Accepts diverse files data sources.  
- Normalizes timestamps and metadata.  
- Auto-categorizes and generates searchable previews.  

### 🔹 Forensic Engine  
- Computes SHA-256 hashes for tamper-evidence.  
- Detects duplicates and mismatched extensions.  
- Extracts metadata and flags suspicious keywords.  
- Assigns weighted suspicion scores for prioritization.  

### 🔹 Correlate & Report  
- Correlates data by user, IP, time, and hash.  
- Maintains immutable audit logs for chain-of-custody.  
- Generates court-ready PDF reports using ReportLab.  

---

## 🧭 Future Enhancements
- Case comparison — uncover cross-case links and similarities.
- AI-based anomaly and pattern detection.
- Cloud case synchronization.
- Role-based access control and digital signatures.
- Real-time dashboard analytics.

---

## 👩‍💻 Author
-> ASMITHA B 
-> Bachelor of Engineering, Computer Science and Design  

**Cyber Triage Tool transforms fragmented digital investigations into a unified, automated, and tamper-evident forensic solution.**
