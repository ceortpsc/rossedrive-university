Ross E‑Drive University
Full Application Manifest · LMS · Compliance Engine · AI‑Powered Driver Education
Proprietary — ROSS TAX PRO SOFTWARE CO
1. PRODUCT IDENTITY
Ross E‑Drive University  
AI‑Powered Driver Education, Training & Road‑Safety University

Core Products
E‑Drive LMS

E‑Drive Student Portal

E‑Drive Parent/Guardian Portal

E‑Drive Instructor Console

E‑Drive School Administration

E‑Drive Compliance Center

E‑Drive AI Tutor (Andreaa)

E‑Drive Assessment Engine

E‑Drive Driving Practice Ledger

E‑Drive Credential Center

E‑Drive Skills‑Test Operations

E‑Drive University Administration

E‑Drive Analytics

E‑Drive Regulatory Monitor

Architecture
Next.js 16 · React 19 · NestJS · Prisma · PostgreSQL · RBAC · Audit Logging · Compliance Engine · AI Persona Runtime · Docker · CI/CD · OpenAPI · JSON Schema · TDLR Export/Reconciliation · DPS‑Readiness

2. COMPLETE STUDENT JOURNEY
Code
Landing Page
 ↓
Eligibility Wizard
 ↓
Student Account
 ↓
Parent/Guardian Consent
 ↓
Identity Verification
 ↓
Program Selection
 ↓
Enrollment
 ↓
Diagnostic Assessment
 ↓
AI Personalized Learning Plan
 ↓
Classroom LMS
 ↓
Knowledge Checks
 ↓
Practice Exams
 ↓
Final Assessment
 ↓
Behind‑the‑Wheel Enrollment
 ↓
Driving Ledger (BTW / Observation / Practice / Night)
 ↓
Completion Validation
 ↓
DPS/ITD Workflow
 ↓
Credential Issuance
 ↓
Skills‑Test Readiness
 ↓
Graduation Dashboard
Completion is never granted by clicking through lessons.
Completion requires verified evidence through the compliance engine.

3. PROGRAM ARCHITECTURE
Teen Driver Education
12 modules

48 lessons

1,440 minutes (24 hours)

144 assessment items

68‑chapter textbook

Instructor guide

Parent resources

AI tutoring layer

Mastery assessments

Academic Progression
Orientation

Texas Licensing Fundamentals

Vehicle Controls

Traffic Laws

Signs/Signals/Markings

Defensive Driving

Risk Perception

Distracted Driving

Impaired Driving

Emergency Situations

Highway/Night/Weather

Final Readiness

Adult Driver Education
6‑hour ADE

Written exam prep

ITAD requirement

Adaptive learning plan

Eligibility engine determines correct program based on:

Age

License status

Residency

Prior driver education

Objective

4. AI‑POWERED UNIVERSITY LAYER
Andreaa — AI Instructor
Adaptive academic coach with:

AI Capabilities
Teach

Explain concepts

Re‑teach difficult lessons

Generate examples

Adjust complexity

Scenario‑based instruction

Diagnose

Knowledge graph

Weak concept detection

Misconception classification

Personalized remediation

Coach

Study plans

Lesson recommendations

Exam preparation

Confidence tracking

Simulate

Safe hypothetical driving scenarios

Reasoning evaluation

5. AI SAFETY BOUNDARY
AI may:

Teach

Explain

Coach

Diagnose

Simulate

Evaluate reasoning

AI must not:

Override Texas requirements

Falsify attendance

Generate fraudulent certificates

Replace required human instruction

Claim TDLR/DPS approval

Modify compliance records without authorization

6. MASTERY ENGINE
Competency‑based learning replaces “click‑through LMS.”

Knowledge States
Not Started

Introduced

Developing

Proficient

Mastered

Example Concept Map
Traffic Signals

Signal meanings

Protected turns

Yellow‑light decisions

Pedestrian crossings

Intersection hazards

7. ASSESSMENT ENGINE
Assessment Types
Multiple choice

Multiple response

True/false

Scenario analysis

Image interpretation

Traffic‑sign identification

Video comprehension

Short‑answer reasoning

Practice exams

Instructor evaluations

Assessment Flow
Code
Assessment
 ↓
Eligibility Check
 ↓
Attempt Authorization
 ↓
Secure Attempt
 ↓
Scoring
 ↓
Mastery Evaluation
 ↓
Pass / Remediation
 ↓
Audit Event
8. COMPLIANCE ENGINE
Example Rule Object
Code
{
  "requirement": "classroom_hours",
  "required": 24,
  "completed": 18,
  "remaining": 6,
  "status": "INCOMPLETE",
  "evidence": [
    "attendance-events",
    "lesson-events",
    "assessment-events"
  ]
}
Completion requires:
ELIGIBLE_FOR_COMPLETION = TRUE

9. REGULATORY GATES
Classroom
6‑hour concurrent

24‑hour block permit gates

Behind‑the‑Wheel
BTW

Observation

Practice

Night

ITTD

ITTD/ITAD
Must be completed before DPS skills test

Certificate valid for 90 days

10. SEPTEMBER 1, 2026 RULESET
Code
RULESET: TX-DRIVER-ED
VERSION: 2026.09.01
EFFECTIVE: 2026-09-01
Rulesets are versioned and applied based on:

Enrollment date

Program version

Effective regulatory date

11. TDLR COMPLIANCE CENTER
Dashboard
License status

Course status

Instructor status

Student records

Attendance integrity

Completion records

Exceptions

Regulatory changes

Export queue

Audit readiness

Compliance States
🟢 Compliant
🟡 Review Required
🟠 Exception
🔴 Blocking Violation
🔵 Pending Agency Action

12. REGULATORY MONITORING
Flow
Code
Regulatory Source
 ↓
Change Detection
 ↓
AI Analysis
 ↓
Proposed Rule
 ↓
Human Review
 ↓
Approval
 ↓
Versioned Ruleset
 ↓
Test Suite
 ↓
Production
13. INSTRUCTOR UNIVERSITY
Instructor Dashboard
Classes

Students

Driving sessions

Assessments

Alerts

Compliance

Messages

Student Profile
Enrollment

Academic progress

Attendance

Assessments

Knowledge map

Driving ledger

Instructor notes

Parent communication

Documents

Compliance

Certificates

Audit history

14. PARENT/GUARDIAN PORTAL
Enrollment status

Course progress

Driving practice

Schedule

Documents

Messages

Payments

Notifications

Parents cannot edit official records.

15. STUDENT DASHBOARD
Modern university‑style UX with:

Progress

Next lesson

AI coach

Driving practice

Readiness score

Continue Learning button

16. DRIVING OPERATIONS (DriveOps)
Session Types
Observation

Behind‑the‑Wheel

Practice

Night

Evaluation

Immutable Events
Session started

Session paused

Session completed

Instructor signed

Student acknowledged

Ledger updated

17. DRIVING LEDGER
Code
Requirement     Completed     Remaining     Status
Classroom       18h          6h            🟡
BTW             8h           —             🟡
Observation     4h           —             🟡
Practice        10h          —             🟡
Night           4h           —             🟡
ITTD            —            —             🔴/🟢
18. CREDENTIAL ENGINE
Flow
Code
Student Record
 ↓
Compliance Engine
 ↓
Completion Eligibility
 ↓
Credential Generator
 ↓
Document Hash
 ↓
Audit Record
 ↓
PDF
Documents
Student identity

Course/program

Provider info

Completion date

Course version

Signatures

Credential ID

Verification QR

Document hash

Audit metadata

19. UNIVERSITY STRUCTURE
Schools
Teen Driver Education

Adult Driver Education

Parent Education

Defensive Driving

Instructor Training

Fleet Safety

Continuing Education

20. AI UNIVERSITY KNOWLEDGE GRAPH
Connects:

Regulation

Curriculum

Lessons

Assessments

Student mastery

21. APPLICATION ARCHITECTURE
Code
ROSS E-DRIVE UNIVERSITY OS
 │
 ├── LEARN (LMS + AI)
 ├── MASTER (Assessment + Knowledge Graph)
 ├── DRIVE (Scheduling + Ledger)
 ├── COMPLY (Rules + Evidence)
 └── CREDENTIAL (Certificates + Verification)
22. CORE SERVICES
identity-service
enrollment-service
student-service
parent-service
instructor-service
lms-service
assessment-service
mastery-service
ai-tutor-service
driving-service
scheduling-service
vehicle-service
attendance-service
compliance-service
regulatory-service
credential-service
document-service
notification-service
billing-service
reporting-service
audit-service

23. RBAC
Roles:

SUPER_ADMIN

UNIVERSITY_ADMIN

SCHOOL_ADMIN

COMPLIANCE_ADMIN

INSTRUCTOR

DRIVING_INSTRUCTOR

ASSESSOR

STUDENT

PARENT_GUARDIAN

SUPPORT

AUDITOR

24. AUDIT ARCHITECTURE
Every sensitive operation logs:

Who

What

When

Where

Why

Before

After

Authorization

Source

IP/Device

Correlation ID

25. ANALYTICS
Academic
Completion rate

Drop‑off points

Mastery

Assessment performance

Operational
Instructor utilization

Vehicle utilization

Driving sessions

No‑shows

Compliance
Exceptions

Missing evidence

Expiring credentials

ITTD expiration

Attendance anomalies

AI
Misunderstood concepts

Students needing intervention

Curriculum gaps

Question quality

26. SECURITY ARCHITECTURE
MFA

RBAC

Encryption

Immutable audit logs

Signed credentials

Rate limiting

API validation

Secrets management

Backup/restore

Disaster recovery

Parental‑consent workflows

27. APPLICATION NAVIGATION
Public
Home · Programs · How It Works · Pricing · Contact · Support · Login · Verify Credential · Privacy · Terms · Regulatory Disclosures

Student
Dashboard · Lessons · AI Coach · Assessments · Driving · Documents · Messages · Progress · Achievements · Profile

Parent
Dashboard · Student Progress · Driving Practice · Schedule · Documents · Messages · Payments · Notifications

Instructor
Dashboard · Classes · Students · Attendance · Assessments · DriveOps · Calendar · Messages · Reports · Compliance

Admin
Command Center · Students · Enrollment · LMS · Curriculum · AI · Instructors · DriveOps · Vehicles · Compliance · TDLR · DPS Readiness · Documents · Billing · Reports · Audit · Settings

28. ENROLLMENT WIZARD
01 Applicant
02 Age/Eligibility
03 License Status
04 Program Recommendation
05 Guardian
06 Consent
07 Account
08 Documents
09 Payment
10 Orientation
11 Diagnostic
12 Personalized Learning Plan

29. ENROLLMENT STATE MACHINE
STARTED → APPLICATION_CREATED → IDENTITY_PENDING → GUARDIAN_PENDING → CONSENTS_PENDING → ELIGIBILITY_REVIEW → PROGRAM_SELECTED → PAYMENT_PENDING → ENROLLED → ORIENTATION → ACTIVE

Exceptions: INCOMPLETE · REVIEW · CANCELLED · WITHDRAWN · SUSPENDED · EXPIRED · COMPLETED

30. TDLR FRAMEWORK
Ruleset ingestion → Human review → Versioning → Compliance engine → Application

31. REQUIREMENT MATRIX
Tracks:

Provider requirements

Instructor requirements

Curriculum

Attendance

Instruction hours

BTW

Observation

Night driving

ITTD/ITAD

Records

32. REGULATORY NOTICE
Ross E‑Drive University is designed to operate in accordance with applicable Texas driver‑education requirements.
Regulatory requirements may change.
Program requirements displayed during enrollment are based on current regulatory information maintained by Ross E‑Drive University.
No governmental endorsement or approval is implied unless explicitly granted.
