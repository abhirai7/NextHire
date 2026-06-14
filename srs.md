# SOFTWARE REQUIREMENTS SPECIFICATION (SRS)

# AI-Powered Job Portal with ATS Resume Analysis, Subscription Management and AI Auto Job Apply System

Version 1.0

---

# 1. Introduction

## 1.1 Purpose

The purpose of this project is to develop an AI-powered Job Portal that connects job seekers and recruiters through a centralized platform. The system provides ATS-based resume analysis, AI-powered resume optimization, intelligent job recommendations, automated job application services, subscription management, and recruiter hiring tools.

The platform aims to improve the recruitment process by helping candidates enhance their resumes, discover relevant opportunities, and automate job applications while enabling recruiters to efficiently identify suitable candidates.

---

## 1.2 Scope

The proposed system provides:

- Candidate Registration and Login
- Recruiter Registration and Login
- Resume Upload and Analysis
- ATS Score Generation
- AI Resume Optimization
- Job Readiness Assessment
- Intelligent Job Recommendations
- AI Auto Job Apply
- Subscription Management
- Job Posting and Management
- Candidate Screening
- Payment Processing
- Administrative Controls

The system will be accessible through modern web browsers and support desktop, tablet, and mobile devices.

---

## 1.3 Objectives

The main objectives are:

- Simplify job searching
- Improve resume quality
- Increase interview opportunities
- Automate repetitive application processes
- Help recruiters find suitable candidates faster
- Generate revenue through subscription plans

---

## 1.4 Definitions

| Term | Description |
|--------|-------------|
| ATS | Applicant Tracking System |
| AI | Artificial Intelligence |
| Candidate | Job seeker using the platform |
| Recruiter | Employer posting jobs |
| Resume Parser | Extracts information from uploaded resumes |
| Job Match Score | Percentage matching between resume and job |
| Job Readiness Score | Overall employability score |
| Subscription | Paid membership plan |

---

# 2. Overall Description

## 2.1 Product Perspective

The system consists of three primary modules:

1. Candidate Module
2. Recruiter Module
3. Admin Module

The system follows a Three-Tier Architecture:

- Presentation Layer
- Business Logic Layer
- Database Layer

---

## 2.2 User Classes

### Candidate

- Create Profile
- Upload Resume
- View ATS Score
- Improve Resume
- Search Jobs
- Apply Jobs
- Enable Auto Apply
- Purchase Subscription

### Recruiter

- Create Company Profile
- Post Jobs
- Manage Applications
- Search Candidates

### Admin

- Manage Users
- Manage Recruiters
- Manage Subscriptions
- Generate Reports
- Monitor Activities

---

## 2.3 Operating Environment

### Client Side

- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari

### Server Side

- Node.js
- Express.js

### Database

- MongoDB

### Storage

- Cloudinary / AWS S3

### Payment Gateway

- Razorpay

---

# 3. Functional Requirements

## 3.1 User Registration and Authentication

### Description

Users can create accounts and securely access the system.

### Functional Requirements

- FR-01 Register User
- FR-02 Login User
- FR-03 Logout User
- FR-04 Email Verification
- FR-05 Password Recovery
- FR-06 Google Authentication
- FR-07 LinkedIn Authentication

---

## 3.2 Candidate Profile Management

### Description

Candidates can create and manage professional profiles.

### Functional Requirements

- FR-08 Create Profile
- FR-09 Update Profile
- FR-10 Upload Profile Picture
- FR-11 Add Education Details
- FR-12 Add Experience Details
- FR-13 Add Skills
- FR-14 Add Certifications
- FR-15 Delete Profile

---

## 3.3 Resume Upload and ATS Analysis

### Description

Candidates can upload resumes in PDF or DOCX format.

The system performs ATS analysis and generates improvement suggestions.

### Functional Requirements

- FR-16 Upload Resume
- FR-17 Parse Resume
- FR-18 Extract Skills
- FR-19 Generate ATS Score
- FR-20 Identify Missing Keywords
- FR-21 Detect Formatting Issues
- FR-22 Generate ATS Report
- FR-23 Provide Improvement Suggestions

### Example Output

**ATS Score:** 84%

**Missing Skills:**
- Docker
- AWS
- CI/CD

**Suggestions:**
- Add Projects Section
- Include Certifications
- Improve Keyword Density

---

## 3.4 AI Resume Enhancement

### Description

AI assists candidates in optimizing resumes.

### Functional Requirements

- FR-24 AI Resume Review
- FR-25 Resume Optimization Suggestions
- FR-26 Grammar Checking
- FR-27 Resume Rewriting Assistance
- FR-28 Skill Gap Analysis
- FR-29 Keyword Optimization

---

## 3.5 Job Readiness Assessment

### Description

The system calculates a Job Readiness Score based on profile completeness, ATS performance, skills, certifications, and experience.

### Functional Requirements

- FR-30 Calculate Job Readiness Score
- FR-31 Evaluate Profile Completeness
- FR-32 Evaluate Skills Relevance
- FR-33 Generate Readiness Report

### Example

- ATS Score: 82%
- Profile Completeness: 90%
- Skills Relevance: 88%
- Job Readiness Score: 87%

---

## 3.6 Intelligent Job Recommendation System

### Description

Jobs are recommended based on resume content and profile information.

### Functional Requirements

- FR-34 Extract Resume Keywords
- FR-35 Analyze Skills
- FR-36 Match Jobs
- FR-37 Calculate Match Percentage
- FR-38 Recommend Jobs
- FR-39 Sort Jobs by Relevance

### Example

- MERN Stack Developer: 95%
- Frontend Developer: 91%
- Backend Developer: 85%

---

## 3.7 Job Search and Application Management

### Description

Candidates can search and apply for jobs.

### Functional Requirements

- FR-40 Search Jobs
- FR-41 Filter Jobs
- FR-42 Save Jobs
- FR-43 View Job Details
- FR-44 Apply to Jobs
- FR-45 Track Application Status
- FR-46 Withdraw Application
- FR-47 View Application History

### Filters

- Location
- Experience
- Salary
- Job Type
- Skills
- Company

---

## 3.8 Subscription Management

### Description

The platform provides subscription-based premium access.

New users receive a limited free trial period. After the trial expires, premium access requires an active subscription.

### Subscription Plans

#### Free Trial

Duration: 7 Days

Features:

- Limited ATS Resume Checks
- Limited Job Applications
- Basic Job Recommendations

#### Premium Weekly Plan

Duration: 7 Days

#### Premium Monthly Plan

Duration: 30 Days

#### Premium Yearly Plan

Duration: 365 Days

### Premium Features

- Unlimited ATS Resume Analysis
- Unlimited Resume Uploads
- AI Resume Suggestions
- Job Readiness Analysis
- Unlimited Job Applications
- Advanced Job Recommendations
- AI Cover Letter Generator
- AI Auto Job Apply
- Application Tracking Dashboard
- Priority Support

### Functional Requirements

- FR-48 View Plans
- FR-49 Purchase Subscription
- FR-50 Renew Subscription
- FR-51 Cancel Subscription
- FR-52 Verify Plan Status
- FR-53 Restrict Premium Features After Expiry

---

## 3.9 Payment Gateway Integration

### Description

Users can purchase subscriptions using secure payment methods.

### Functional Requirements

- FR-54 Process Payments
- FR-55 Verify Transactions
- FR-56 Generate Payment Receipts
- FR-57 Store Payment History
- FR-58 Handle Failed Payments

---

## 3.10 AI Auto Job Apply System

### Description

The AI Auto Job Apply System automatically identifies and applies to relevant job opportunities using resume analysis and keyword matching.

The user can define preferences such as preferred roles, locations, salary ranges, and minimum match score.

### Workflow

```text
Resume Upload
     ↓
Resume Parsing
     ↓
Keyword Extraction
     ↓
Job Matching
     ↓
Compatibility Scoring
     ↓
Automatic Application Submission
     ↓
User Notification
```

### Functional Requirements

- FR-59 Extract Resume Keywords
- FR-60 Scan Available Jobs
- FR-61 Calculate Match Scores
- FR-62 Automatically Apply to Relevant Jobs
- FR-63 Send User Notifications
- FR-64 Allow Enable/Disable Auto Apply
- FR-65 Configure Auto Apply Preferences
- FR-66 Maintain Auto Apply History

---

## 3.11 Recruiter Module

### Description

Recruiters can manage job postings and candidate applications.

### Functional Requirements

- FR-67 Recruiter Registration
- FR-68 Create Company Profile
- FR-69 Post Job
- FR-70 Edit Job
- FR-71 Delete Job
- FR-72 View Applications
- FR-73 Download Resumes
- FR-74 Search Candidates
- FR-75 Contact Candidates

---

## 3.12 Candidate Ranking System

### Description

Candidates are ranked according to ATS score, skills, experience, and job compatibility.

### Functional Requirements

- FR-76 Rank Applicants
- FR-77 Calculate Skill Match
- FR-78 Compare ATS Scores
- FR-79 Generate Candidate Rankings
- FR-80 Shortlist Candidates

---

## 3.13 Admin Module

### Description

Administrators manage the overall platform.

### Functional Requirements

- FR-81 Manage Users
- FR-82 Manage Recruiters
- FR-83 Verify Companies
- FR-84 Manage Job Listings
- FR-85 Manage Subscriptions
- FR-86 Manage Payments
- FR-87 Generate Reports
- FR-88 Monitor Activities
- FR-89 Suspend Accounts

---

# 4. Non-Functional Requirements

## Performance

- Response Time less than 3 seconds
- Support 10,000+ concurrent users
- Fast job recommendation generation

## Security

- JWT Authentication
- Password Encryption
- HTTPS Communication
- Secure Payment Processing
- Role-Based Access Control

## Reliability

- 99% System Availability
- Daily Database Backups

## Scalability

- Cloud Deployment Support
- Horizontal Scaling

## Maintainability

- Modular Code Structure
- API-Based Architecture

## Usability

- Responsive User Interface
- Mobile-Friendly Design
- Easy Navigation

---

# 5. Database Design

## Users

- UserID
- Name
- Email
- Password
- Phone
- Role
- SubscriptionID

## Profiles

- ProfileID
- UserID
- Skills
- Education
- Experience
- Certifications

## Resumes

- ResumeID
- UserID
- FileURL
- ATSScore
- ReadinessScore

## Jobs

- JobID
- RecruiterID
- Title
- Description
- Skills
- Salary
- Location

## Applications

- ApplicationID
- UserID
- JobID
- Status
- AppliedDate

## Subscriptions

- SubscriptionID
- PlanName
- Price
- Duration

## Payments

- PaymentID
- UserID
- Amount
- PaymentDate
- Status

## Companies

- CompanyID
- RecruiterID
- CompanyName
- Description

---

# 6. System Architecture

Presentation Layer
- React.js
- Tailwind CSS

Application Layer
- Node.js
- Express.js

AI Processing Layer
- Resume Parser
- ATS Engine
- Job Matching Engine
- Auto Apply Engine
- AI Recommendation Engine

Database Layer
- MongoDB

Storage Layer
- Cloudinary / AWS S3

Payment Layer
- Razorpay

---

# 7. Use Cases

## Candidate

- Register/Login
- Create Profile
- Upload Resume
- Check ATS Score
- Improve Resume
- Search Jobs
- Apply Jobs
- Enable Auto Apply
- Purchase Subscription
- Track Applications

## Recruiter

- Register/Login
- Create Company Profile
- Post Jobs
- View Applicants
- Search Candidates
- Shortlist Candidates

## Admin

- Manage Users
- Verify Companies
- Manage Recruiters
- Manage Payments
- Generate Reports

---

# 8. Future Enhancements

- Mobile Application
- AI Mock Interviews
- AI Career Guidance
- Video Resume Upload
- LinkedIn Integration
- Interview Scheduling
- Job Alert Notifications
- Multi-Language Support
- AI Salary Prediction
- AI Skill Roadmaps

---

# 9. Conclusion

The AI-Powered Job Portal is an intelligent recruitment platform that combines ATS resume analysis, AI-based resume optimization, job readiness assessment, subscription management, recruiter hiring tools, and an innovative AI Auto Job Apply System. The platform enhances job search efficiency, improves candidate employability, and streamlines recruitment processes, making it a comprehensive solution for modern hiring and career development.