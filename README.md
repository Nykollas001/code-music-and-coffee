# Code, Music, and Coffee

This project is a **security-first learning platform idea** that combines:
- Programming practice
- Music as motivation and context
- English immersion in all content

The goal is to build the project in phases: first the soul (purpose + plan), then the body (implementation).

## Vision
Create a product where learning to code is connected to music workflows and all interaction happens in English, so the creator can improve technical skills and language fluency at the same time.

## Core Principles
1. **English-first:** documentation, UI copy, and user interaction in English.
2. **Security-first:** no coding before architecture and threat model are clear.
3. **Step-by-step execution:** small milestones to avoid overload and keep momentum.
4. **Participative decisions:** every major technical choice should be discussed with pros/cons.

## Phase 0 (Current): Project Understanding and Strategy
No coding yet. Focus only on structure.

### 0.1 Problem Statement
How can one product help a developer reconnect with programming while improving English through a music-centered experience?

### 0.2 Initial Target User
- Primary: solo creator (you) using the platform as a learning engine.
- Secondary (future): beginners/intermediate learners who like coding + music.

### 0.3 Value Proposition
A practical learning environment that mixes coding challenges, music-themed tasks, and English communication in one workflow.

## Phase 1: Security-First Blueprint (Before Choosing Final Language)

### 1.1 Scope Draft (MVP Sketch)
Define exactly what the first version does and does not do.

**In scope (example):**
- User account
- Daily coding/music/English mission
- Progress tracking
- Basic content management

**Out of scope (for now):**
- Social feed
- Complex AI tutor
- Advanced integrations

### 1.2 Security Architecture (Pre-Code)
Mandatory deliverables before implementation:
- Threat model (assets, attackers, vectors)
- Data classification (public, private, sensitive)
- Authentication strategy (MFA-ready)
- Authorization model (roles/permissions)
- Secrets management policy
- Logging and monitoring baseline
- Backup and recovery strategy
- Dependency and supply-chain policy

### 1.3 Language Decision (After Security Requirements)
The final language choice should be made **after** the security requirements are documented.

Current recommendation shortlist:
1. **Java (Spring Boot):** mature security ecosystem, strong enterprise patterns.
2. **C# (.NET):** very strong identity/auth tooling and secure defaults.
3. **Go:** simple deployment, good performance, straightforward secure services.
4. **Python (FastAPI/Django):** great productivity, but needs stricter discipline for long-term hardening.

## Phase 2: First Implementation Slice (Login + Admin)
After Phase 1 is approved, the first coding slice will be authentication and an administrative visibility panel.

### 2.1 Login Logic (MVP)
- Sign up with email + password
- Sign in with secure session/token strategy
- Password reset flow
- Basic account lock/rate-limit protections
- Optional MFA-ready design (enabled later)

### 2.2 Admin Visibility (MVP)
Administrative dashboard should allow safe access to these user/account fields:
- User ID
- Last known IP (with privacy/legal policy)
- Nickname
- Email
- Total time inside the application (session duration)
- Account creation date

### 2.3 Security Notes for Admin Data
- Restrict admin area by role-based authorization.
- Log all admin reads/exports.
- Mask sensitive data where possible.
- Keep data retention rules explicit.

## Phase 3: Technical Decisions (Guided Discussions)
Before coding each block, discuss options in a teacher-style format:
- Option A vs Option B
- Pros and cons
- Complexity level
- Security implications
- Recommendation + why

Example topics:
- Frontend approach (e.g., static + API vs SPA)
- Backend language stack
- Database type
- Hosting and deployment model
- CI/CD and security checks

## Phase 4: Implementation Plan (After Approval)
Only starts when Phase 1 + 2 + 3 are documented and approved.

1. Repository structure
2. Secure scaffolding
3. Authentication and authorization
4. Admin dashboard (minimum fields)
5. MVP features
6. Observability and hardening
7. Local test launch

## English Coaching Mode (Always On)
To support English learning in every session:
- All technical artifacts stay in English.
- Explanations can be bilingual (PT-BR + EN) when needed.
- At the end of each session, include:
  - 3 useful English technical phrases
  - 2 corrections for common mistakes
  - 1 short practice sentence to repeat/use

## Working Method (ADHD-Friendly)
- One objective per session
- Checklists with very small tasks
- Frequent recap: “What we decided / next step”
- No long jumps between topics
- Always end with a clear next action

## Next Conversation Checklist
In the next step, we can decide these five items together:
1. Login method (session cookie vs JWT)
2. Minimal admin fields and who can see them
3. Threat model draft focused on auth flows
4. Data retention policy for IP/session logs
5. Final language decision criteria (security + learning curve)

---
If you want, the next iteration can be a one-page **Auth & Admin Security Requirements v1** document, fully in English.
