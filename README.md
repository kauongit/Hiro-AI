# Hiro AI 💼
'Hiro' is an AI recruitment intelligence platform that analyzes candidates from multiple data sources, understands job requirements semantically, and explains why each candidate is the best fit.

# System Architecture

```
                               HIRO
               AI Recruitment Intelligence Platform
──────────────────────────────────────────────────────────────────────

                    👨‍💼 Recruiter Portal
                           │
          ┌────────────────┴────────────────┐
          │                                       │
          ▼                                       ▼
  Upload Job Description                Upload Candidate Resumes
          │                                       │
          └──────────────┬──────────────────┘
                         ▼
              📄 Document Processing Layer
        ┌────────────────────────────────────┐
        │ • Resume Parser (PDF/DOCX)                │
        │ • Job Description Parser                  │
        │ • Text Extraction                         │
        │ • Metadata Extraction                     │
        └────────────────────────────────────┘
                         │
                         ▼
             🧠 AI Intelligence Engine
        ┌────────────────────────────────────┐
        │ • Semantic Job Understanding              │
        │ • Candidate DNA Generation                │
        │ • Skill Extraction                        │
        │ • Experience Analysis                     │
        │ • Career Timeline Analysis                │
        │ • Embedding Generation                    │
        └────────────────────────────────────┘
                         │
                         ▼
            ⚡ Intelligent Ranking Engine
        ┌────────────────────────────────────┐
        │ • Semantic Similarity                     │
        │ • Technical Skill Matching                │
        │ • Learning Potential                      │
        │ • Leadership Analysis                     │
        │ • Culture Fit                             │
        │ • Confidence Score                        │
        └────────────────────────────────────┘
                         │
                         ▼
              💡 Explainable AI Layer
        ┌────────────────────────────────────┐
        │ • Why this candidate?                     │
        │ • Evidence & Reasoning                    │
        │ • Skill Gap Analysis                      │
        │ • Strengths & Weaknesses                  │
        │ • Hiring Recommendations                  │
        └────────────────────────────────────┘
                         │
                         ▼
             📊 Recruiter Intelligence Hub
        ┌────────────────────────────────────┐
        │ • AI Copilot                              │
        │ • Candidate Ranking Dashboard             │
        │ • Candidate Profiles                      │
        │ • Team Builder                            │
        │ • Hiring Analytics                        │
        └────────────────────────────────────┘
```

---

## Technology Stack

| Layer | Technology |
|--------|------------|
| Frontend | React + Tailwind CSS |
| Backend | FastAPI (Python) |
| AI Model | Google Gemini |
| Embeddings | Gemini Embeddings |
| Vector Database | ChromaDB |
| Database | MongoDB |
| Resume Parsing | PyMuPDF |
| Authentication | Firebase Auth |
| Deployment | Vercel + Railway/Render |

---

## AI Pipeline

```
Job Description
        │
        ▼
Semantic Understanding
        │
        ▼
Candidate Resume Parsing
        │
        ▼
Embedding Generation
        │
        ▼
Vector Similarity Search
        │
        ▼
Multi-Factor AI Scoring
        │
        ▼
Explainable Ranking
        │
        ▼
Recruiter Dashboard
```

### AI Scoring Factors

- 🎯 Semantic Skill Match
- 💼 Experience Relevance
- 📈 Career Growth Trajectory
- 🧠 Learning Potential
- 👥 Leadership Indicators
- 🤝 Cultural Alignment
- 📂 Project & Portfolio Quality
- ⭐ Overall Confidence Score
