# Collection: Recruiters

**Purpose:** Stores recruiter accounts.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Unique recruiter ID |
| name | String | Recruiter name |
| email | String | Email address |
| company | String | Company name |
| role | String | Recruiter/Admin |
| createdAt | Date | Account creation timestamp |

---

# Collection: Jobs

**Purpose:** Stores job descriptions.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Unique job ID |
| title | String | Job title |
| description | String | Full job description |
| requiredSkills | Array | Required skills |
| preferredSkills | Array | Preferred skills |
| experience | String | Required experience |
| location | String | Job location |
| employmentType | String | Full-time / Internship |
| embedding | Array | Vector embedding |
| createdBy | ObjectId | Recruiter ID |
| createdAt | Date | Timestamp |

---

# Collection: Candidates

**Purpose:** Stores candidate profiles.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Candidate ID |
| name | String | Candidate name |
| email | String | Email |
| phone | String | Phone number |
| resumeUrl | String | Resume file URL |
| github | String | GitHub profile |
| linkedin | String | LinkedIn profile |
| portfolio | String | Portfolio URL |
| skills | Array | Extracted skills |
| education | Array | Education history |
| experience | Array | Work experience |
| projects | Array | Projects |
| certifications | Array | Certifications |
| embedding | Array | Candidate embedding |
| createdAt | Date | Timestamp |

---

# Collection: AI_Analysis

**Purpose:** Stores AI-generated candidate insights.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Analysis ID |
| candidateId | ObjectId | Candidate reference |
| jobId | ObjectId | Job reference |
| semanticScore | Number | Semantic similarity |
| technicalScore | Number | Technical fit |
| leadershipScore | Number | Leadership score |
| learningScore | Number | Learning ability |
| cultureFit | Number | Culture fit |
| confidenceScore | Number | AI confidence |
| overallScore | Number | Final weighted score |
| strengths | Array | Candidate strengths |
| weaknesses | Array | Candidate weaknesses |
| missingSkills | Array | Missing skills |
| explanation | String | AI explanation |
| recommendation | String | AI recommendation |
| createdAt | Date | Timestamp |

---

# Collection: Shortlists

**Purpose:** Stores shortlisted candidates.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Shortlist ID |
| recruiterId | ObjectId | Recruiter reference |
| jobId | ObjectId | Job reference |
| candidateId | ObjectId | Candidate reference |
| status | String | Shortlisted / Rejected / Hired |
| notes | String | Recruiter notes |
| createdAt | Date | Timestamp |

---

# Collection: Chat_History

**Purpose:** Stores AI Copilot conversations.

| Field | Type | Description |
|-------|------|-------------|
| _id | ObjectId | Chat ID |
| recruiterId | ObjectId | Recruiter reference |
| message | String | User message |
| response | String | AI response |
| timestamp | Date | Conversation timestamp |
