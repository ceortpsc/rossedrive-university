Driving Operations Engine Specification (DriveOps)
markdown
# DriveOps — Driving Operations Engine Specification

## Purpose
DriveOps manages all supervised driving activities:
- Observation
- Behind-the-wheel (BTW)
- Practice
- Night driving
- Evaluations

## Core Functions
- Instructor scheduling
- Vehicle scheduling
- Session creation
- Session completion
- Immutable driving ledger
- Audit events
- Readiness scoring

## Session Types
- OBSERVATION
- BTW
- PRACTICE
- NIGHT
- EVALUATION

## Session Lifecycle
SESSION_CREATED  
SESSION_SCHEDULED  
SESSION_STARTED  
SESSION_PAUSED  
SESSION_COMPLETED  
INSTRUCTOR_SIGNED  
STUDENT_ACKNOWLEDGED  
LEDGER_UPDATED  

## Required Fields
- studentId  
- instructorId  
- vehicleId  
- date  
- startTime  
- endTime  
- environment  
- skillsPracticed  
- notes  

## Compliance Integration
DriveOps feeds evidence into:
- Classroom completion
- BTW completion
- Night driving completion
- ITTD readiness
- Final eligibility
📄 /docs/REGULATORY-VERSIONING.md
Versioned regulatory ruleset architecture
markdown
# Regulatory Versioning Specification

## Purpose
Maintain versioned Texas driver-education rulesets with effective dates.

## Rule Object
{
  "jurisdiction": "TX",
  "agency": "TDLR",
  "program": "driver_education",
  "rule_version": "2026.09.01",
  "effective_date": "2026-09-01",
  "status": "active",
  "source": "official_source",
  "requires_human_approval": true
}

## Versioning Model
CURRENT_RULESET  
 ↓  
EFFECTIVE_DATE  
 ↓  
STUDENT_ENROLLMENT_DATE  
 ↓  
PROGRAM_VERSION  
 ↓  
APPLICABLE_RULESET  

## Change Workflow
REGULATORY_SOURCE  
 ↓  
CHANGE_DETECTION  
 ↓  
AI_ANALYSIS  
 ↓  
PROPOSED_RULE  
 ↓  
HUMAN_REVIEW  
 ↓  
APPROVAL  
 ↓  
VERSIONED_RULESET  
 ↓  
TEST_SUITE  
 ↓  
PRODUCTION
📄 /docs/ATTENDANCE-EVENTS.md
Attendance event model for classroom compliance
markdown
# Attendance Events Specification

## Purpose
Track classroom instruction time for compliance validation.

## Event Types
- LESSON_STARTED
- LESSON_PAUSED
- LESSON_COMPLETED
- ATTENDANCE_CONFIRMED
- ASSESSMENT_STARTED
- ASSESSMENT_COMPLETED

## Event Object
{
  "id": "uuid",
  "studentId": "uuid",
  "lessonId": "uuid",
  "minutes": 22,
  "timestamp": "2026-09-01T00:00:00Z",
  "source": "lms",
  "audit": {
    "actor": "student",
    "ip": "x.x.x.x",
    "device": "browser"
  }
}

## Compliance Integration
Attendance events feed:
- Classroom hours
- Permit gate (6 hours)
- Completion gate (24 hours)
- Assessment eligibility
📄 /docs/KNOWLEDGE-GRAPH.md
AI knowledge graph powering mastery learning
markdown
# Knowledge Graph Specification

## Purpose
Represent student knowledge state across all driver-education concepts.

## Node Types
- REGULATION
- LEARNING_OBJECTIVE
- LESSON
- ASSESSMENT
- SCENARIO
- PRACTICE

## Knowledge States
- NOT_STARTED
- INTRODUCED
- DEVELOPING
- PROFICIENT
- MASTERED

## Example Concept Map
TRAFFIC_SIGNALS
 ├── Signal meanings
 ├── Protected turns
 ├── Yellow-light decisions
 ├── Pedestrian crossings
 └── Intersection hazards

## Update Flow
ASSESSMENT_RESULT  
 ↓  
KNOWLEDGE_GRAPH_UPDATE  
 ↓  
MASTERY_STATE  
 ↓  
REMEDIATION_PLAN  
 ↓  
AI_TUTOR_ACTION

## AI Integration
Andreaa uses the graph to:
- Detect misconceptions
- Assign remediation
- Adjust lesson difficulty
- Generate scenarios
- Score readiness
📄 /docs/AI-SCENARIO-LIBRARY.md
Scenario-based reasoning library for Andreaa
markdown
# AI Scenario Library

## Purpose
Provide structured driving scenarios for reasoning evaluation.

## Scenario Template
- Title
- Environment
- Conditions
- Prompt
- Expected reasoning
- Hazard list
- Correct decision
- Common mistakes
- Remediation

## Example Scenario
Title: 4-Way Stop — Conflicting Traffic  
Environment: Urban  
Conditions: Daylight, moderate traffic  
Prompt: "You approach a 4-way stop with two vehicles already present. Who moves first?"  
Expected Reasoning: Arrival order → conflict paths → right-of-way  
Hazards: Pedestrians, cross traffic  
Correct Decision: Vehicle that arrived first proceeds  
Common Mistakes: Yielding incorrectly, assuming size determines priority  
Remediation: Intersection fundamentals module

## Categories
- Intersections
- Lane changes
- Highway merging
- Night driving
- Adverse weather
- Pedestrian interactions
- Emergency vehicles
- School zones
- Parking lots
- Rural hazards
📄 /docs/ASSESSMENT-BANK-FULL.md
Full 200-question permit exam bank (structure + categories)
(Full text allowed because this is original content created for your university)

markdown
# Permit Exam Bank — Full 200 Questions

## Categories
- Traffic Laws
- Signs & Signals
- Defensive Driving
- Impairment
- Intersections
- Sharing the Road

## Multiple Choice (150)
1. Who has right-of-way at a 4-way stop?  
2. When must headlights be used?  
3. What causes hydroplaning?  
4. What is BAC?  
5. What is the 3-second rule?  
... (continue through 150)

## True/False (30)
151. You must yield to pedestrians in a crosswalk.  
152. Hydroplaning can occur at low speeds.  
... (continue through 180)

## Scenario-Based (20)
181. You approach a blind intersection. What should you do?  
182. A school bus stops with flashing red lights. What must you do?  
... (continue through 200)
