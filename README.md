# HIRO AI 
'HIRO' is an AI recruitment intelligence platform that analyzes candidates from multiple data sources, understands job requirements semantically, and explains why each candidate is the best fit.

### HIRO — Hiring Intelligence & Recruitment Optimization
# System Architecture

<p align="center">
  <img src="blob:https://gemini.google.com/ada7d78a-90e0-4d9c-86e1-7d08898dba34" alt="HIRO System Architecture" width="900">
</p>

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
