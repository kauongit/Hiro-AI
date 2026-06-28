
API Specification

Base URL

/api/v1

---

Authentication

Register Recruiter

Method| Endpoint
POST| "/auth/register"

Request

{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "********"
}

Response

{
  "success": true,
  "message": "Recruiter registered successfully"
}

---

Login

Method| Endpoint
POST| "/auth/login"

---

Jobs

Create Job

Method| Endpoint
POST| "/jobs"

---

Get All Jobs

Method| Endpoint
GET| "/jobs"

---

Get Job by ID

Method| Endpoint
GET| "/jobs/{jobId}"

---

Analyze Job Description

Method| Endpoint
POST| "/jobs/analyze"

Function

- Extract skills
- Experience
- Soft skills
- Semantic embedding

---

Candidates

Upload Resume

Method| Endpoint
POST| "/candidates/upload"

---

Get All Candidates

Method| Endpoint
GET| "/candidates"

---

Get Candidate

Method| Endpoint
GET| "/candidates/{candidateId}"

---

Compare Candidates

Method| Endpoint
POST| "/candidates/compare"

---

AI Ranking

Generate Rankings

Method| Endpoint
POST| "/ai/rank"

Returns:

- Overall Score
- Technical Score
- Leadership
- Learning
- Culture Fit
- Explainability

---

Candidate DNA

Method| Endpoint
GET| "/ai/dna/{candidateId}"

---

Explain Ranking

Method| Endpoint
POST| "/ai/explain"

---

Skill Gap Analysis

Method| Endpoint
POST| "/ai/skill-gap"

---

AI Copilot

Chat

Method| Endpoint
POST| "/copilot/chat"

Example prompts:

- Find backend developers.
- Compare Candidate A and Candidate B.
- Explain why Candidate X ranked first.
- Show candidates with leadership skills.

---

Shortlist

Add to Shortlist

Method| Endpoint
POST| "/shortlist"

---

Get Shortlist

Method| Endpoint
GET| "/shortlist"

---

Analytics

Dashboard Analytics

Method| Endpoint
GET| "/analytics/dashboard"

Returns:

- Total Candidates
- Active Jobs
- Shortlisted Candidates
- Hiring Funnel
- AI Insights

---

Health Check

Method| Endpoint
GET| "/health"

Returns:

{
  "status": "OK"
}
