Database Schema

Database: "hiro_db"

---

Collection: Recruiters

Stores recruiter accounts.

Field| Type| Description
_id| ObjectId| Unique ID
name| String| Recruiter name
email| String| Email address
company| String| Company name
role| String| Recruiter/Admin
createdAt| Date| Account creation

---

Collection: Jobs

Stores job postings.

Field| Type| Description
_id| ObjectId| Job ID
title| String| Job title
description| String| Full job description
requiredSkills| Array| Required skills
preferredSkills| Array| Preferred skills
experience| String| Required experience
location| String| Job location
employmentType| String| Full-time/Internship
embedding| Array| Vector embedding for semantic search
createdBy| ObjectId| Recruiter ID
createdAt| Date| Timestamp

---

Collection: Candidates

Stores candidate profiles.

Field| Type| Description
_id| ObjectId| Candidate ID
name| String| Candidate name
email| String| Email
phone| String| Phone number
resumeUrl| String| Resume file
github| String| GitHub profile
linkedin| String| LinkedIn profile
portfolio| String| Portfolio
skills| Array| Extracted skills
education| Array| Education history
experience| Array| Work experience
projects| Array| Projects
certifications| Array| Certifications
embedding| Array| Candidate embedding

---

Collection: AI Analysis

Stores AI-generated insights.

Field| Type| Description
_id| ObjectId| Analysis ID
candidateId| ObjectId| Candidate reference
jobId| ObjectId| Job reference
semanticScore| Number| Semantic similarity
technicalScore| Number| Technical fit
leadershipScore| Number| Leadership
learningScore| Number| Learning ability
cultureFit| Number| Culture fit
confidence| Number| AI confidence
explanation| String| Explainable AI summary
strengths| Array| Strengths
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
