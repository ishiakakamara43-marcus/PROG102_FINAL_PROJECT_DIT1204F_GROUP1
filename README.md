


LIMKOKWING UNIVERSITY OF CREATIVE TECHNOLOGY
Faculty of Information and Communication Technology
Sierra Leone Campus
PROG 102 – PRINCIPLES OF SOFTWARE ENGINEERING
FINAL PROJECT
EduReach SL: Software Design for a Digital Public Good



March 2026 – July 2026
 Table of Contents
Table of Contents	1
1. Introduction	1
1.1 System Overview	1
2. Problem Definition	1
2.1 Background of the Problem	1
2.2 Target Users	1
2.3 Why This Problem Is Important	1
3. Software Development Life Cycle (SDLC)	1
3.1 Selected SDLC Model: Agile (Iterative and Incremental)	1
3.2 SDLC Phases for EduReach SL	1
3.3 SDLC Diagram	1
4. System Architecture Design	1
4.1 Architecture Overview	1
4.2 Architecture Layers	1
4.3 System Architecture Diagram	1
4.4 Component Interaction	1
5. UML Diagrams	1
5.1 Use Case Diagram	1
5.2 Class Diagram	1
5.3 Activity Diagram	1
5.4 Sequence Diagram	1
5.5 State Diagram	1
5.6 Component Diagram	1
5.7 Deployment Diagram	1
6. Entity-Relationship (ER) Diagram	1
7. Network Diagram	1
7.1 Physical Network Diagram	1
8. Prototype Development	1
8.1 Prototype Approach	1
8.2 Design Principles	1
8.3 Figma Screen Inventory	1
8.4 Figma Prototype Link	1
9. Project Management	1
9.1 Project Plan Overview	1
9.2 Gantt Chart	1
9.3 Network Diagram (Critical Path Analysis)	1
10. Git and GitHub Integration	1
10.1 Repository Structure	1
10.2 Branching Strategy	1
10.3 Collaboration Workflow	1
11. License, Design Quality, and SDG Relevance	1
11.1 Software License	1
11.2 Design Quality (UI/UX)	1
11.3 SDG Relevance	1
12. Full System Description	1
12.1 System Name and Purpose	1
12.2 Key Features and Functions	1
12.3 Step-by-Step Workflow	1
13. Conclusion	1
14. References	1

1. Introduction
In an increasingly connected world, technology has become one of the most powerful tools for addressing society's deepest challenges. A Digital Public Good (DPG) is defined as a digital system — such as software, a mobile application, or an online platform — that is designed specifically to serve the public interest. Unlike commercial products, a DPG prioritises access, equity, and impact over profit, and is typically aligned with the United Nations Sustainable Development Goals (SDGs).

This Final Project presents the complete software design of EduReach SL (Education Reach Sierra Leone) — a community-focused digital learning and resource access platform developed specifically for the Sierra Leonean public school context. This document builds on the initial assignment concept and expands it into a fully documented software engineering deliverable, encompassing the Software Development Life Cycle (SDLC), system architecture, UML diagrams, prototype planning, project management artefacts, and licensing decisions.

EduReach SL is aligned with SDG 4: Quality Education, which calls on all nations to ensure inclusive, equitable, and quality education while promoting lifelong learning opportunities for all. Despite global progress, millions of learners in sub-Saharan Africa — including Sierra Leone — still lack consistent access to quality educational resources, trained teachers, and structured learning support. EduReach SL is not imagined as a replacement for schools, but as a digital bridge connecting students, teachers, and parents with accessible learning content even in low-bandwidth environments.




1.1 System Overview
Attribute	Details
System Name	EduReach SL (Education Reach Sierra Leone)
System Type	Web-based and Mobile-accessible Digital Learning Platform
Primary Users	Students, Teachers, Parents/Guardians, Administrators
SDG Alignment	SDG 4: Quality Education
Target Country	Sierra Leone, West Africa
License	MIT Open Source License
Development Model	Agile (Iterative and Incremental)


2. Problem Definition
2.1 Background of the Problem
Sierra Leone has made considerable strides in rebuilding its educational infrastructure following years of civil conflict and the devastating Ebola outbreak of 2014–2016. However, the country continues to face severe systemic challenges. According to UNICEF and the World Bank, net enrolment rates remain below regional averages, and learning outcomes as measured by literacy and numeracy assessments are consistently among the lowest in West Africa. Many public schools operate without adequate textbooks, and a significant proportion of classrooms lack trained, qualified teachers.

The problem is further compounded by geography. Students in rural districts such as Kono, Kailahun, and Pujehun often travel long distances to reach schools, only to find classrooms overcrowded and under-resourced. When schools closed nationwide during the COVID-19 pandemic, the majority of Sierra Leonean students had no digital fallback. EduReach SL addresses this gap directly.


2.2 Target Users
User Group	Description
Students (Ages 8–22)	Primary and secondary school learners lacking access to quality materials beyond overcrowded classrooms.
Teachers	Both qualified and untrained teachers who need digital tools to share content, set assignments, and monitor progress.
Parents / Guardians	Adults seeking visibility into their children’s learning progress through a structured digital channel.
School Administrators	Staff responsible for managing enrolment records, academic calendars, and performance reporting.
Content Moderators	Reviewers who ensure all uploaded content is appropriate, accurate, and curriculum-aligned.

2.3 Why This Problem Is Important
Education is both a human right and the foundation of sustainable development. When children do not receive quality education, the effects ripple through generations — limiting economic mobility, deepening inequality, and weakening civic participation. A lightweight, accessible digital platform represents a realistic, cost-effective intervention that does not require high-end devices or stable internet connections to function meaningfully.
 3. Software Development Life Cycle (SDLC)
3.1 Selected SDLC Model: Agile (Iterative and Incremental)
EduReach SL will be developed using the Agile Software Development methodology. Agile is selected because the system serves a real community with evolving requirements — particularly in a low-resource, high-uncertainty environment such as Sierra Leone’s public school system. Agile allows the development team to deliver working functionality in short iterations (sprints), incorporate feedback from real users (students, teachers, administrators), and adapt to infrastructure constraints such as intermittent internet connectivity and limited device capabilities.

The Agile model is structured around sprints of two weeks each, with the full project spanning six sprints across a twelve-week development period (Weeks 1–12 of the semester). Each sprint produces a tested, deployable increment of the system.

3.2 SDLC Phases for EduReach SL
Phase	Activities for EduReach SL
1. Planning	Define project scope, identify stakeholders, establish team roles, create the project Gantt chart and network diagram, select MIT license, set up GitHub repository and project board.
2. Requirements Analysis	Conduct stakeholder interviews with teachers and students, document functional requirements (course library, assessment engine, parent portal), document non-functional requirements (offline mode, 2G/3G support, low device specs).
3. System Design	Design system architecture (3-tier model), produce all UML diagrams (Use Case, Class, Activity, Sequence, State, Component, Deployment), design ER diagram and database schema, create wireframes for all 10 Figma screens.
4. Implementation (Sprints 1–4)	Sprint 1: User authentication and registration. Sprint 2: Course library and content browsing. Sprint 3: Assessment engine (quizzes and assignments). Sprint 4: Parent portal and admin panel. Code committed to GitHub after each sprint.
5. Testing	Unit testing of all modules, integration testing of component interactions, user acceptance testing (UAT) with pilot school in Freetown, performance testing under 2G network conditions, bug reporting and resolution.
6. Deployment	Deploy to cloud server (e.g., DigitalOcean or AWS Lightsail), configure domain, set up SSL certificate, conduct teacher training sessions, distribute student login credentials via school administration.
7. Maintenance	Monitor system uptime, release monthly updates based on user feedback, patch security vulnerabilities, add new content categories as curriculum expands.

3.3 SDLC Diagram
The diagram below illustrates the Agile SDLC cycle as applied to EduReach SL. The circular flow represents the iterative nature of the development process, where each sprint passes through planning, design, implementation, testing, and review before feeding back into the next sprint.

FIGURE 1 – EduReach SL Agile SDLC Cycle (PlantUML Source)
 

Source: Adapted from Sommerville (2016) and Pressman & Maxim (2020). The Agile model was selected due to its suitability for evolving community requirements and constrained infrastructure environments.
4. System Architecture Design
4.1 Architecture Overview
EduReach SL is built on a Three-Tier (3-Tier) Client-Server Architecture. This model separates the system into three logical layers: the Presentation Layer (front-end), the Application Logic Layer (back-end), and the Data Layer (database). This separation ensures maintainability, scalability, and security — making it suitable for incremental community deployment.
4.2 Architecture Layers
Layer	Technology / Components
Presentation Layer (Client)	HTML5, CSS3, JavaScript (React.js). Mobile-responsive design accessible via smartphone browser. Offline capability via Service Workers (PWA).
Application Logic Layer (Server)	Node.js with Express.js REST API. Authentication via JWT tokens. Business logic: enrolment processing, quiz grading, progress calculation, report generation.
Data Layer (Database)	MySQL relational database for user data, courses, enrolments, and assessments. File storage (PDFs, videos) via AWS S3 or local file server.
External Integrations	SMS gateway (Africa's Talking API) for login PIN delivery. Email notification service (SendGrid). CDN for video content delivery.

4.3 System Architecture Diagram
The diagram below shows how the three tiers interact. Client devices communicate with the Application Server via HTTPS REST API calls. The Application Server processes business logic and queries the Database Layer. File resources are served via a CDN or file server.




FIGURE 2 – EduReach SL System Architecture Diagram (PlantUML Source)











4.4 Component Interaction
When a student logs in, the Presentation Layer sends a login request to the Auth Service via HTTPS. The Auth Service validates credentials against the Users Table and returns a JWT token. The student's dashboard is then populated by the Course Service and Progress Tracker, which query their respective database tables. When a quiz is submitted, the Assessment Engine auto-grades the responses and the Progress Tracker updates the Enrolments Table. The Report Generator aggregates this data for teacher and admin review.
5. UML Diagrams

This section presents all seven required UML diagrams for EduReach SL. Each diagram is accompanied by a PlantUML source code block for reproducibility and a written explanation of the diagram's purpose and key elements.
5.1 Use Case Diagram
The Use Case Diagram identifies all system actors and the functional capabilities they interact with. It provides a high-level behavioural view of the EduReach SL system without detailing implementation. Five actors are identified: Student, Teacher, Parent/Guardian, Administrator, and Content Moderator.









FIGURE 3 – Use Case Diagram (PlantUML Source)


The Use Case Diagram confirms that EduReach SL supports five distinct actor roles, each with specific and non-overlapping primary responsibilities. The Student interacts most frequently with the system (seven use cases), reflecting the platform's learner-centric design. Content uploaded by Teachers passes through the Moderator before becoming accessible to Students, ensuring quality assurance.

5.2 Class Diagram
The Class Diagram represents the structural backbone of EduReach SL. It shows the main classes, their attributes and methods, and the relationships between them (inheritance, association, and composition). This diagram directly informs the database schema and back-end object model.



FIGURE 4 – Class Diagram (PlantUML Source)


The Class Diagram reveals that User is an abstract parent class inherited by Student, Teacher, and Parent subclasses. The Enrolment class serves as a junction entity managing the many-to-many relationship between Students and Courses. Each Course may contain multiple Assessments, and both Teachers and the system can generate Reports based on assessment and progress data.

5.3 Activity Diagram
The Activity Diagram maps the step-by-step workflow a student follows when using EduReach SL — from opening the application through to completing an assessment and viewing their progress report. The diagram uses swim lanes to distinguish between Student actions and automated System responses.

FIGURE 5 – Activity Diagram: Student Learning Workflow (PlantUML Source)



The Activity Diagram demonstrates that the system handles both online and offline modes, ensuring continuity of learning even without active internet access. The credential validation loop allows students to retry login without being locked out, which is essential in a shared-device environment where typing errors are common.

5.4 Sequence Diagram
The Sequence Diagram shows the time-ordered interaction between objects when a student submits a quiz. It illustrates how messages pass between the Student, the Web Browser (client), the Application Server, the Assessment Engine, and the Database across the timeline of a single use case.

FIGURE 6 – Sequence Diagram: Quiz Submission (PlantUML Source)


The Sequence Diagram confirms that quiz grading is performed server-side by the Assessment Engine, which queries the database for correct answers before computing the score. This server-side grading approach prevents answer manipulation by clients and ensures that all results are reliably stored and auditable.

5.5 State Diagram
The State Diagram models the different states that a Course object can exist in throughout its lifecycle within EduReach SL — from initial creation by a teacher through to archival or deletion. It shows the conditions (transitions) that move a course from one state to another.



FIGURE 7 – State Diagram: Course Lifecycle (PlantUML Source)


The State Diagram reveals that EduReach SL enforces a mandatory content moderation step before any course is visible to students. A course cannot transition from Draft directly to Published without passing through the UnderReview state, ensuring quality control. Archived courses retain their data for reporting purposes but are hidden from the active catalogue.

5.6 Component Diagram
The Component Diagram illustrates the major software components of EduReach SL and how they are structured and interconnected. Unlike the architecture diagram (which shows tiers), the component diagram focuses on software modules and their interfaces.

FIGURE 8 – Component Diagram (PlantUML Source)
@startuml
title EduReach SL – Component Diagram

package "Frontend (React.js SPA)" {
  [Student Dashboard UI]
  [Teacher Portal UI]
  [Admin Panel UI]
  [Parent Portal UI]
  [Offline PWA Module]
}

package "Backend API (Node.js / Express)" {
  [Auth Module] --> [JWT Token Manager]
  [Course Module]
  [Assessment Module]
  [Progress Module]
  [Reporting Module]
  [Notification Module]
  [Content Moderation Module]
}

package "Data Layer" {
  database [MySQL DB]
  [File Storage (S3)]
}

package "External APIs" {
  [SMS Gateway]
  [Email Service]
  [CDN]
}

[Student Dashboard UI] --> [Auth Module] : REST/HTTPS
[Student Dashboard UI] --> [Course Module]
[Student Dashboard UI] --> [Assessment Module]
[Teacher Portal UI] --> [Course Module]
[Teacher Portal UI] --> [Assessment Module]
[Teacher Portal UI] --> [Reporting Module]
[Admin Panel UI] --> [Auth Module]
[Admin Panel UI] --> [Reporting Module]
[Parent Portal UI] --> [Progress Module]
[Offline PWA Module] ..> [Course Module] : sync when online

[Auth Module] --> [MySQL DB]
[Course Module] --> [MySQL DB]
[Course Module] --> [File Storage (S3)]
[Assessment Module] --> [MySQL DB]
[Progress Module] --> [MySQL DB]
[Notification Module] --> [SMS Gateway]
[Notification Module] --> [Email Service]
[Course Module] --> [CDN]
[Content Moderation Module] --> [MySQL DB]
@enduml

The Component Diagram shows that each major functional area of EduReach SL is encapsulated in its own back-end module, promoting separation of concerns and allowing individual components to be maintained or upgraded independently. The Offline PWA Module communicates with the Course Module only when connectivity is restored, supporting intermittent internet environments.

5.7 Deployment Diagram
The Deployment Diagram shows the physical distribution of EduReach SL components across computing nodes — specifically, how software components are deployed on actual servers, devices, and cloud infrastructure.

FIGURE 9 – Deployment Diagram (PlantUML Source)
@startuml
title EduReach SL – Deployment Diagram

node "Student / Teacher Device\n(Smartphone / PC)" {
  artifact "React.js SPA\n(Chrome / Firefox)"
  artifact "PWA Cache\n(Offline Content)"
}

node "Cloud Server\n(DigitalOcean / AWS Lightsail)" {
  artifact "Node.js App Server\n(Express API)"
  artifact "Nginx Reverse Proxy"
  artifact "SSL Certificate (Let's Encrypt)"
}

node "Database Server\n(Managed MySQL)" {
  artifact "MySQL 8.0"
  artifact "Daily Backup Agent"
}

node "File Storage\n(AWS S3 / Local NAS)" {
  artifact "PDF & Video Files"
  artifact "CDN Distribution"
}

node "External Services" {
  artifact "Africa's Talking\n(SMS Gateway)"
  artifact "SendGrid\n(Email)"
}

"Student / Teacher Device\n(Smartphone / PC)" --> "Cloud Server\n(DigitalOcean / AWS Lightsail)" : HTTPS (Port 443)
"Cloud Server\n(DigitalOcean / AWS Lightsail)" --> "Database Server\n(Managed MySQL)" : TCP (Port 3306, Private Network)
"Cloud Server\n(DigitalOcean / AWS Lightsail)" --> "File Storage\n(AWS S3 / Local NAS)" : HTTPS
"Cloud Server\n(DigitalOcean / AWS Lightsail)" --> "External Services" : HTTPS APIs
@enduml

The Deployment Diagram shows that all student and teacher devices communicate exclusively with the Cloud Server via encrypted HTTPS connections. The Database Server is isolated on a private network, accessible only from the App Server — this is a critical security measure to prevent direct public access to the database. File content is served via CDN to reduce server load and improve delivery speed to devices on slow connections.
 6. Entity-Relationship (ER) Diagram
The Entity-Relationship (ER) Diagram represents the logical data model of EduReach SL. It identifies all database entities, their attributes, primary and foreign keys, and the relationships between entities (one-to-one, one-to-many, and many-to-many). The ER diagram directly drives the MySQL database schema implementation.

FIGURE 10 – ER Diagram (PlantUML Source)
@startuml
title EduReach SL – Entity-Relationship Diagram
!define primary_key(x) <b><u>x</u></b>

entity User {
  primary_key(userID): INT
  --
  name: VARCHAR(100)
  email: VARCHAR(100) UNIQUE
  password_hash: VARCHAR(255)
  role: ENUM('STUDENT','TEACHER','ADMIN','PARENT')
  school: VARCHAR(100)
  createdAt: DATETIME
}

entity Course {
  primary_key(courseID): INT
  --
  title: VARCHAR(150)
  description: TEXT
  category: VARCHAR(50)
  grade_level: VARCHAR(20)
  createdBy_teacherID: INT (FK)
  status: ENUM('DRAFT','REVIEW','PUBLISHED','ARCHIVED')
  createdAt: DATETIME
}

entity Enrolment {
  primary_key(enrolID): INT
  --
  studentID: INT (FK)
  courseID: INT (FK)
  dateEnrolled: DATE
  status: ENUM('ACTIVE','DROPPED','COMPLETED')
  progressPercent: INT DEFAULT 0
}

entity Assessment {
  primary_key(assessID): INT
  --
  courseID: INT (FK)
  type: ENUM('QUIZ','ASSIGNMENT')
  title: VARCHAR(150)
  maxScore: INT
  deadline: DATETIME
  isPublished: BOOLEAN
}

entity Submission {
  primary_key(subID): INT
  --
  assessID: INT (FK)
  studentID: INT (FK)
  submittedAt: DATETIME
  score: INT
  feedback: TEXT
}

entity Report {
  primary_key(reportID): INT
  --
  generatedBy: INT (FK - User)
  reportType: ENUM('PROGRESS','PERFORMANCE','ENROLMENT')
  generatedAt: DATETIME
  dataJSON: JSON
}

User ||--o{ Course : "creates (Teacher)"
User ||--o{ Enrolment : "makes (Student)"
Course ||--o{ Enrolment : "has"
Course ||--o{ Assessment : "contains"
Assessment ||--o{ Submission : "receives"
User ||--o{ Submission : "submits (Student)"
User ||--o{ Report : "generates"
@enduml

The ER Diagram confirms that EduReach SL uses seven primary entities. The Enrolment entity resolves the many-to-many relationship between Users (Students) and Courses. The Submission entity similarly resolves the many-to-many relationship between Assessments and Students. All foreign key relationships are enforced at the database level to maintain referential integrity.
 7. Network Diagram
7.1 Physical Network Diagram
The Network Diagram illustrates the physical and logical network infrastructure required to run EduReach SL in a school environment. It shows how student devices, teacher workstations, the school's local network, and the cloud infrastructure are interconnected.

FIGURE 11 – Network Diagram (PlantUML Source)
@startuml
!include <awslib/AWSCommon>
title EduReach SL – Network Diagram

node "School Campus" {
  node "Student Devices" {
    [Smartphone (Android)]
    [Shared Desktop PC]
    [Tablet]
  }
  node "Teacher Workstation" {
    [Teacher Laptop / PC]
  }
  node "School Network" {
    [WiFi Router / Access Point]
    [Switch]
  }
  node "Local Offline Server (optional)" {
    [Raspberry Pi / NAS\n(Offline Content Cache)]
  }
}

node "Internet" {
  [ISP / 2G-4G Mobile Network]
}

node "Cloud Infrastructure" {
  [Nginx Reverse Proxy]
  [Node.js App Server]
  [MySQL Database Server]
  [AWS S3 File Storage]
  [CDN Edge Node]
}

node "External Services" {
  [Africa's Talking SMS API]
  [SendGrid Email API]
}

[Smartphone (Android)] --> [WiFi Router / Access Point]
[Shared Desktop PC] --> [Switch]
[Tablet] --> [WiFi Router / Access Point]
[Teacher Laptop / PC] --> [Switch]
[Switch] --> [WiFi Router / Access Point]
[WiFi Router / Access Point] --> [Local Offline Server (optional)] : LAN
[WiFi Router / Access Point] --> [ISP / 2G-4G Mobile Network] : WAN / HTTPS
[ISP / 2G-4G Mobile Network] --> [Nginx Reverse Proxy] : HTTPS 443
[Nginx Reverse Proxy] --> [Node.js App Server]
[Node.js App Server] --> [MySQL Database Server] : TCP Private
[Node.js App Server] --> [AWS S3 File Storage] : HTTPS
[AWS S3 File Storage] --> [CDN Edge Node]
[Node.js App Server] --> [Africa's Talking SMS API] : HTTPS
[Node.js App Server] --> [SendGrid Email API] : HTTPS
@enduml

The Network Diagram demonstrates that EduReach SL can operate in two modes: (1) fully online via the cloud infrastructure, and (2) partially offline via the optional local Raspberry Pi/NAS cache on the school's LAN. In offline mode, downloaded content is served locally without requiring internet access. This dual-mode design is essential for schools in rural Sierra Leone where internet connectivity is intermittent or only available at certain hours.
 8. Prototype Development
8.1 Prototype Approach
EduReach SL will be prototyped as a high-fidelity UI/UX design using Figma. The prototype will contain a minimum of ten key screens, covering all major user journeys identified in the Use Case Diagram. The Figma prototype uses a mobile-first design approach, reflecting the fact that the majority of Sierra Leonean students access digital content via smartphones rather than desktop computers.

8.2 Design Principles
•	Simplicity: Maximum two taps or clicks to reach any core function from the home screen.
•	Accessibility: Large font sizes, high-contrast colour scheme, and icon-based navigation to support users with lower digital literacy.
•	Offline Indication: Clear visual indicators showing which content is available offline and which requires connectivity.
•	Localisation: English-language interface with provision for future translation into Krio (Sierra Leone's lingua franca).
•	Performance: Lightweight assets (compressed images, minimal animations) optimised for 2G/3G bandwidth.

8.3 Figma Screen Inventory
Screen #	Screen Name	Primary Actor
01	Splash / Welcome Screen	All Users
02	Login Screen (Student / Teacher)	All Users
03	Student Dashboard (Home)	Student
04	Course Library / Browse Catalogue	Student
05	Course Detail & Enrol Page	Student
06	Video Lesson / Content Viewer	Student
07	Quiz / Assessment Interface	Student
08	Progress Report Screen	Student / Parent
09	Teacher Upload Content Screen	Teacher
10	Admin Panel — User Management	Administrator

8.4 Figma Prototype Link
The interactive Figma prototype is accessible via the GitHub repository for this project and will be submitted alongside this report. The prototype demonstrates all ten screens with clickable navigation flows simulating the student learning journey and teacher content upload workflow.

GitHub Repository: https://github.com/[student-username]/EduReach-SL
 9. Project Management
9.1 Project Plan Overview
The EduReach SL Final Project is planned across twelve weeks (March 2026 to July 2026), corresponding to Weeks 1 through 12 of the academic semester. The project plan is divided into seven phases aligned with the Agile SDLC model. A Gantt chart and Critical Path Network Diagram are presented below.

9.2 Gantt Chart
The Gantt chart below shows the timeline for each project phase, including start week, end week, and duration in weeks. Tasks on the critical path are those with zero float — any delay in these tasks will delay the overall project completion.

Task ID	Task Name	Start Week	End Week	Duration	Critical Path
T1	Project Planning & GitHub Setup	1	2	2 weeks	Yes
T2	Requirements Analysis	2	3	2 weeks	Yes
T3	System Design & UML Diagrams	3	5	3 weeks	Yes
T4	Figma Prototype (10 screens)	4	6	3 weeks	No
T5	Sprint 1 – Auth & Registration	5	6	2 weeks	Yes
T6	Sprint 2 – Course Library	6	7	2 weeks	Yes
T7	Sprint 3 – Assessment Engine	7	8	2 weeks	Yes
T8	Sprint 4 – Portals & Admin Panel	8	9	2 weeks	Yes
T9	Testing (Unit + UAT)	9	11	3 weeks	Yes
T10	Documentation & Report Writing	8	11	4 weeks	No
T11	Deployment & Submission	11	12	1 week	Yes
					

FIGURE 12 – Gantt Chart (PlantUML Source)
@startgantt
title EduReach SL – Project Gantt Chart
Project starts 2026-03-02
saturday are closed
sunday are closed

[T1 – Planning & GitHub Setup] lasts 14 days
[T2 – Requirements Analysis] starts at [T1 – Planning & GitHub Setup]'s end and lasts 14 days
[T3 – System Design & UML] starts at [T2 – Requirements Analysis]'s end and lasts 21 days
[T4 – Figma Prototype] starts at [T3 – System Design & UML]'s start and lasts 21 days
[T5 – Sprint 1: Auth Module] starts at [T3 – System Design & UML]'s end and lasts 14 days
[T6 – Sprint 2: Course Library] starts at [T5 – Sprint 1: Auth Module]'s end and lasts 14 days
[T7 – Sprint 3: Assessment Engine] starts at [T6 – Sprint 2: Course Library]'s end and lasts 14 days
[T8 – Sprint 4: Portals & Admin] starts at [T7 – Sprint 3: Assessment Engine]'s end and lasts 14 days
[T9 – Testing & UAT] starts at [T8 – Sprint 4: Portals & Admin]'s end and lasts 21 days
[T10 – Documentation] starts at [T7 – Sprint 3: Assessment Engine]'s start and lasts 28 days
[T11 – Deployment & Submission] starts at [T9 – Testing & UAT]'s end and lasts 7 days
@endgantt

9.3 Network Diagram (Critical Path Analysis)
The Network Diagram below uses the Activity-on-Node (AON) method to identify the Critical Path — the longest sequence of dependent tasks that determines the minimum possible project duration. Float values indicate how many days a non-critical task can be delayed without affecting the final deadline.

FIGURE 13 – Network Diagram / Critical Path (PlantUML Source)
@startuml
title EduReach SL – Network Diagram (Critical Path)

rectangle "START" as S
rectangle "T1\nPlanning\n2 wks" as T1
rectangle "T2\nRequirements\n2 wks" as T2
rectangle "T3\nSystem Design\n3 wks" as T3
rectangle "T4\nFigma\n3 wks\n[Float: 1 wk]" as T4
rectangle "T5\nSprint 1\n2 wks" as T5
rectangle "T6\nSprint 2\n2 wks" as T6
rectangle "T7\nSprint 3\n2 wks" as T7
rectangle "T8\nSprint 4\n2 wks" as T8
rectangle "T9\nTesting\n3 wks" as T9
rectangle "T10\nDocumentation\n4 wks\n[Float: 2 wks]" as T10
rectangle "T11\nDeployment\n1 wk" as T11
rectangle "END" as E

S --> T1
T1 --> T2
T2 --> T3
T3 --> T4
T3 --> T5
T5 --> T6
T6 --> T7
T7 --> T8
T7 --> T10
T8 --> T9
T9 --> T11
T10 --> T11
T4 --> T9
T11 --> E
@enduml

Critical Path: START → T1 → T2 → T3 → T5 → T6 → T7 → T8 → T9 → T11 → END. Total Critical Path Duration: 12 weeks. T4 (Figma Prototype) has one week of float and can be delayed by up to one week without impacting the final deadline. T10 (Documentation) has two weeks of float.
 10. Git and GitHub Integration
10.1 Repository Structure
A GitHub repository has been created for EduReach SL to manage version control, facilitate team collaboration, and serve as the submission platform for all project artefacts. The repository follows a structured branching strategy aligned with Agile sprint cycles.

Repository Structure
EduReach-SL/
├── README.md
├── LICENSE
├── docs/
│   ├── Final_Project_Report.pdf
│   ├── diagrams/
│   │   ├── use_case.puml
│   │   ├── class_diagram.puml
│   │   ├── activity_diagram.puml
│   │   ├── sequence_diagram.puml
│   │   ├── state_diagram.puml
│   │   ├── component_diagram.puml
│   │   ├── deployment_diagram.puml
│   │   ├── er_diagram.puml
│   │   ├── network_diagram.puml
│   │   └── gantt_chart.puml
│   └── prototype/
│       └── figma_export/
├── src/
│   ├── frontend/
│   └── backend/
└── .github/
    └── ISSUE_TEMPLATE/

10.2 Branching Strategy
Branch Name	Purpose
main	Stable, production-ready code. Protected — no direct pushes.
develop	Integration branch for all sprint work.
feature/auth-module	Sprint 1: Authentication and registration module.
feature/course-library	Sprint 2: Course browsing and content access.
feature/assessment-engine	Sprint 3: Quiz and assignment functionality.
feature/portals	Sprint 4: Parent portal and admin panel.
docs/diagrams	All UML PlantUML source files and exported images.

10.3 Collaboration Workflow
1.	Each sprint begins with a GitHub Issues board listing all tasks for that sprint.
2.	Team members create feature branches from develop and commit code with descriptive messages.
3.	Pull Requests are opened against develop at sprint end and reviewed by at least one team member.
4.	Merged branches are deleted to maintain a clean repository.
5.	At the end of the project, develop is merged into main and a release tag is created (v1.0.0).
 11. License, Design Quality, and SDG Relevance
11.1 Software License
EduReach SL is released under the MIT License. The MIT License was selected because it is one of the most permissive and widely-recognised open source licenses, consistent with the Digital Public Good (DPG) standard requirement that DPGs use open source licenses. Under the MIT License, any school, NGO, government body, or community organisation may freely use, copy, modify, and distribute EduReach SL without restriction, provided the original copyright notice is retained.

MIT License Notice
MIT License
Copyright (c) 2026 EduReach SL Development Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

All third-party libraries used in EduReach SL (React.js, Node.js, Express.js, MySQL) are either MIT-licensed or Apache 2.0-licensed, ensuring full license compatibility for open-source distribution.

11.2 Design Quality (UI/UX)
The EduReach SL interface has been designed according to the following UI/UX quality principles, reflected in the Figma prototype:

Design Principle	Implementation in EduReach SL
Consistency	A single design system with consistent colour palette (primary blue #1F4E79, accent green #27AE60), typography (Nunito Sans), and icon set (Material Design Icons) across all 10 screens.
Simplicity	Maximum two taps from any screen to reach the nearest core function. No features requiring technical expertise.
Accessibility	Minimum contrast ratio of 4.5:1 (WCAG AA), font size minimum 16px, large touch targets (minimum 44px height) for mobile users.
Feedback	All system actions (login, enrolment, quiz submission) provide immediate visual confirmation to the user.
Offline UX	Cached content is visually indicated with a download icon badge, and users see an offline banner notification when connectivity is lost.

11.3 SDG Relevance
EduReach SL directly addresses Sustainable Development Goal 4: Quality Education. It contributes to the following specific SDG 4 sub-targets:

SDG 4 Sub-Target	EduReach SL Contribution
4.1 – Free, equitable primary/secondary education	All curriculum content is freely accessible to all enrolled students regardless of geographic location or household income.
4.4 – Skills for employment and entrepreneurship	The platform can host vocational and skills development content alongside academic materials.
4.5 – Eliminate gender disparities	Designed for basic smartphones, reducing barriers that disproportionately affect girls and students from low-income households.
4.c – Increase supply of qualified teachers	Provides teachers with ready-made, quality-assured content, reducing the impact of teacher shortages and skill gaps.
 12. Full System Description
12.1 System Name and Purpose
EduReach SL (Education Reach Sierra Leone) is a lightweight, browser-based digital learning management platform designed for use in Sierra Leone's public school system. Its primary purpose is to provide students with structured, curriculum-aligned learning content they can access at school, at home, or through community internet access points.

12.2 Key Features and Functions
•	Course Library: A structured repository of curriculum-aligned learning materials organised by subject, grade level, and topic, including PDFs, video lessons, and revision notes.
•	Student Dashboard: A personalised home screen showing enrolled courses, upcoming assignments, recent quiz scores, and a progress indicator for each subject.
•	Assessment Engine: A built-in quiz and assignment module that allows teachers to create timed, auto-graded quizzes or manually graded assignments with deadlines.
•	Progress Tracking: Automated tracking of each student's completion rate, quiz scores, and assignment grades, visible to both the student and their teacher.
•	Parent Portal: A simplified read-only portal giving parents and guardians access to their child's attendance, grades, and learning progress.
•	Offline Mode: Core content is downloadable for offline reading, ensuring usability in areas with intermittent internet access.
•	Admin Panel: A back-office interface for school administrators to manage registrations, generate term reports, and oversee platform usage.
•	Content Moderation: Before any teacher-uploaded material is visible to students, it passes through a moderation queue to ensure quality and appropriateness.

12.3 Step-by-Step Workflow
Step	Description
Step 1 – Registration	A school administrator creates user accounts for students and teachers using a bulk CSV upload. Students receive a login PIN via SMS or printed card.
Step 2 – Login	The student or teacher opens the platform in their browser and logs in with their credentials. The system authenticates and loads the relevant dashboard.
Step 3 – Content Access	Students browse the course catalogue and enrol in subjects. Teachers upload lesson notes, videos, or links to the relevant course.
Step 4 – Learning	Students watch video lessons, read notes, and download materials. Progress is automatically tracked as sections are marked complete.
Step 5 – Assessment	The teacher publishes a quiz or assignment. Students attempt it within the set deadline. Auto-graded quizzes receive instant scores.
Step 6 – Feedback	Teachers review assignment submissions and enter grades. Students and parents can view scores and feedback on the dashboard.
Step 7 – Reporting	At the end of a term, administrators and teachers generate downloadable performance reports for each class or individual student.
 13. Conclusion
EduReach SL represents a thoughtful, practical, and technically grounded response to one of Sierra Leone's most persistent development challenges: unequal access to quality education. By designing a system that connects students with curriculum-aligned content, equips teachers with digital tools, and brings parents into the learning process, the platform addresses the educational crisis from multiple angles simultaneously.

This Final Project has demonstrated the complete software engineering process for EduReach SL — from initial problem definition and SDLC planning, through full system architecture design, comprehensive UML modelling, prototype screen design, project management planning, and open-source licensing. Each section of this report has been produced in alignment with professional software engineering standards as described by Sommerville (2016) and Pressman and Maxim (2020).

What makes EduReach SL compelling as a Digital Public Good is not just its technical sophistication, but its alignment with real-world constraints. It is lightweight enough to run on basic devices, honest about the connectivity limitations of rural communities, and flexible enough to serve both primary school children and senior secondary students. It does not require massive government investment to launch — a single school, NGO, or district council could implement it with modest funding and a basic cloud hosting plan.

In the broader context of SDG 4 and Sierra Leone's national development ambitions, EduReach SL demonstrates that effective digital public goods do not need to be sophisticated or expensive — they need to be appropriate, accessible, and built around the real lives of the people they are meant to serve. With the right implementation strategy and community buy-in, EduReach SL has the potential to meaningfully improve educational outcomes for tens of thousands of Sierra Leonean learners and, in doing so, contribute to a more equitable and prosperous future for the country as a whole.
 14. References
Abubakar, I. (2021). Digital transformation in education: Opportunities for developing economies. Journal of Educational Technology in Society, 24(3), 45–59.

Boehm, B. W. (1988). A spiral model of software development and enhancement. IEEE Computer, 21(5), 61–72. https://doi.org/10.1109/2.59

Digital Public Goods Alliance. (2022). Digital public goods standard. DPGA. https://digitalpublicgoods.net/standard/

Fowler, M. (2003). UML distilled: A brief guide to the standard object modeling language (3rd ed.). Addison-Wesley Professional.

Jacobson, I., Booch, G., & Rumbaugh, J. (1999). The unified software development process. Addison-Wesley.

Ministry of Basic and Senior Secondary Education, Sierra Leone. (2022). Education sector plan 2022–2026. Government of Sierra Leone.

Object Management Group. (2017). Unified modeling language specification version 2.5.1. OMG. https://www.omg.org/spec/UML/

Pressman, R. S., & Maxim, B. R. (2020). Software engineering: A practitioner's approach (9th ed.). McGraw-Hill Education.

Schwaber, K., & Sutherland, J. (2020). The Scrum guide: The definitive guide to Scrum — The rules of the game. Scrum.org. https://scrumguides.org

Sommerville, I. (2016). Software engineering (10th ed.). Pearson Education.

UNESCO. (2022). Reimagining our futures together: A new social contract for education. UNESCO Publishing. https://unesdoc.unesco.org

UNICEF Sierra Leone. (2023). Education country profile: Sierra Leone. UNICEF West and Central Africa. https://www.unicef.org/wca/sierraleone

United Nations. (2015). Transforming our world: The 2030 agenda for sustainable development. United Nations. https://sdgs.un.org/2030agenda

World Bank. (2022). Sierra Leone education sector analysis. World Bank Group. https://www.worldbank.org
