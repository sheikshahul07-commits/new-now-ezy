# VECTR — The Next-Generation Talent Discovery Network

> **"Your Next Opportunity Starts Here."**  
> *The traditional way of finding opportunities needs a rethink. We believe talent shouldn't get lost in endless applications. People deserve to be discovered, and companies deserve better access to emerging talent.*

Built with the design aesthetic and technical rigor of high-growth technology companies (inspired by **Linear.app**, **Deel**, **Stripe**, **Framer**, and **Arc**).

---

## 🚀 Live Demo & Getting Started

### 1. Set Active Workspace & Start Dev Server
```bash
cd "C:\Users\DELL\.gemini\antigravity\scratch\vectr-network"
npm run dev
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser.

---

## ⚡ Instant Persona Switcher (For Evaluation & Demo)

A floating **Persona Switcher** is embedded directly into the header navigation bar, allowing immediate switching between all 3 platform roles without manual login:

| Persona | Role | Preloaded Credentials | Focus / Core Journey |
| :--- | :--- | :--- | :--- |
| **Rahul Kumar** | **Candidate** | `rahul.kumar@gmail.com` / `demo123` | Civil Engineering fresher from Hosur. View 100% profile score, toggle employer visibility, accept/decline introduction requests. |
| **Apex Infrastructure** | **Employer** | `hiring@apexengineering.com` / `demo123` | Verified construction firm in Hosur. Post hiring requirements, browse matching candidate pools, track sent introductions. |
| **Terminal Superuser** | **Administrator** | `admin@vectr.network` / `demo123` | View real-time database metrics, approve/reject employer registrations, manage talent pools, configure curation fees, export candidate registry. |

---

## 🏗️ Architecture & Core Systems

### 1. The 11-Section Homepage
- **Section 1: Sticky Navigation Bar** with glassmorphism, brand vector mark, role switcher, and responsive drawer.
- **Section 2: Hero** with bold editorial typography, interactive talent stream preview, and live category tabs.
- **Section 3: The Problem** with split-screen comparison: Candidate friction (3,000+ random applications) vs. Employer drain (screening 90% irrelevant mass applications).
- **Section 4: Our Solution** with interactive 4-stage diagram: `CANDIDATES` ➔ `TALENT POOLS` ➔ `EMPLOYERS` ➔ `OPPORTUNITIES`.
- **Section 5: How It Works** covering the 4 phases: Join Network ➔ Enter Talent Pool ➔ Get Discovered ➔ Connect & Move Forward.
- **Section 6: Talent Categories** featuring 10 dynamic categories with candidate counts computed strictly from actual database records.
- **Section 7: For Candidates** highlighting contact shielding, zero keyword-bot rejection, and structured discovery.
- **Section 8: For Employers** showcasing multi-criteria filtering, verified candidates, and direct 48-hour introductions.
- **Section 9: Brand Philosophy** with large editorial typography: *"THE NEXT GENERATION DESERVES A BETTER WAY IN."*
- **Section 10: Final CTA** with dual conversion paths for job seekers and hiring teams.
- **Section 11: Footer** with legal links, social channels, and zero-spam guarantee.

### 2. Talent Discovery Engine (`/discovery`)
- **Criteria Matching Engine**: Calculates candidate match scores based on genuine qualifications, experience level, location, and technical skill overlap.
- **Benchmark Requirement Preset**: 1-click test button loads the exact benchmark requirement from the prompt:
  - *Role: Junior Civil Engineer*
  - *Location: Hosur*
  - *Experience: Fresher*
  - *Qualification: Diploma / B.E. Civil*
  - *Skills: AutoCAD, Structural Analysis, Site Supervision, Estimation*
- **Privacy Shielding**: Full candidate contact information (phone, email) remains protected until an employer requests an introduction and the candidate explicitly accepts.

### 3. Candidate Onboarding & Dashboard (`/register/candidate` & `/candidate/dashboard`)
- 4-step progressive onboarding with live skill tag creation and resume simulation.
- Profile completion score meter.
- Visibility switch (toggle between public in pool and hidden).
- Inbound employer introduction inbox with "Accept & Share Contact Info" or "Decline".
- Transparent curation fee payment gateway integration simulation (fully configurable in Admin).
- **Compliance**: Explicit notice stating no promise of employment or guaranteed interviews.

### 4. Employer Portal (`/register/employer` & `/employer/dashboard`)
- Employer registration subject to administrator approval.
- Post and manage live hiring requirements.
- Direct link from each requirement to pre-filtered candidate pool matches.
- Real-time introduction request tracker with lifecycle status: `Pending` ➔ `Connected` ➔ `Hired`.

### 5. Administrator Console (`/admin`)
- Real-time metric analytics computed strictly from database state.
- Candidate moderation (approve, hold, delete, export to JSON).
- Employer verification & approval workflow.
- Dynamic Talent Pool creator (add new categories with custom slug and skills).
- Curation fee configuration (toggle enabled/disabled, amount, currency).

---

## 🛠️ Technology Stack
- **Framework**: Next.js 16 (App Router + Turbopack)
- **Language**: TypeScript (Strict mode)
- **Styling**: Tailwind CSS v4 with custom dark Obsidian & Electric Volt design system
- **Icons**: Lucide React
- **State & Storage**: Client/Server-synchronized state provider with persistent `localStorage` cache
- **Typography**: Geist Sans & Geist Mono
