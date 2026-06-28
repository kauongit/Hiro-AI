Database Schema

Database Name

"hiro_db"

---

Collection: Recruiters

Purpose: Stores recruiter accounts.

_id: ObjectId
name: String
email: String
company: String
role: String
createdAt: Date

---

Collection: Jobs

Purpose: Stores job descriptions and requirements.

_id: ObjectId
title: String
description: String
requiredSkills: Array
preferredSkills: Array
experience: String
location: String
employmentType: String
embedding: Array
createdBy: ObjectId
createdAt: Date

---

Collection: Candidates

Purpose: Stores candidate profiles.

_id: ObjectId
name: String
email: String
phone: String
resumeUrl: String
github: String
linkedin: String
portfolio: String
skills: Array
education: Array
experience: Array
projects: Array
certifications: Array
embedding: Array
createdAt: Date

---

Collection: AI_Analysis

Purpose: Stores AI-generated analysis for each candidate.

_id: ObjectId
candidateId: ObjectId
jobId: ObjectId
semanticScore: Number
technicalScore: Number
leadershipScore: Number
learningScore: Number
cultureFit: Number
confidenceScore: Number
overallScore: Number
strengths: Array
weaknesses: Array
missingSkills: Array
explanation: String
recommendation: String
createdAt: Date

---

Collection: Shortlists

Purpose: Stores shortlisted candidates.

_id: ObjectId
recruiterId: ObjectId
jobId: ObjectId
candidateId: ObjectId
status: String
notes: String
createdAt: Date

---

Collection: Chat_History

Purpose: Stores recruiter conversations with the AI Copilot.

_id: ObjectId
recruiterId: ObjectId
message: String
response: String
timestamp: Date

---

Relationships

Recruiter
    │
    ├── creates ─────► Jobs
    │
    ├── shortlists ──► Candidates
    │
    └── chats with ──► AI Copilot

Jobs
    │
    └── analyzed against ──► Candidates

Candidates
    │
    └── generate ──► AI Analysis

AI Analysis
    │
    └── produces ──► Ranked Candidatesstrengths| Array| Strengths
weaknesses| Array| Weaknesses
missingSkills| Array| Missing skills

---

Collection: Shortlists

Stores shortlisted candidates.

Field| Type| Description
_id| ObjectId| Shortlist ID
recruiterId| ObjectId| Recruiter
jobId| ObjectId| Job
candidateId| ObjectId| Candidate
status| String| Shortlisted/Rejected/Hired
createdAt| Date| Timestamp

---

Collection: Chat History

Stores AI Copilot conversations.

Field| Type| Description
_id| ObjectId| Chat ID
recruiterId| ObjectId| Recruiter
message| String| User prompt
response| String| AI response
createdAt| Date| Timestamp
