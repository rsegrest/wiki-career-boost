---
title: NASA
created: 2026-05-30
updated: 2026-10-16
type: entity
tags: [organization, employer, space, government, engineering, simulation]
sources: [raw/articles/linkedin-ricksegrest-2026.md, raw/articles/gemini-career-outlook-2026-10-16.md]
---

# NASA

**Type:** Organization | **Industry:** Space / Aeronautics / Research

## Overview

National Aeronautics and Space Administration. Primary US government agency responsible for civilian space program, aeronautics research, and space science.

## Rick's Role

- **Site / Center:** Marshall Space Flight Center (MSFC), Huntsville, AL
- **Contractor support:** [[entities/amentum]] provides staffing/contracting services under the ESSCA contract
- **Tenure:** 7.5+ years (since March 2019) ^[raw/articles/gemini-career-outlook-2026-10-16.md]
- **Title:** Full-stack Cloud-based Web Application Architect
- **Clearance:** Held Secret clearance on prior job before March 2019; dormant/inactive since NASA work has been unclassified, but remains in DISS/NBIS and eligible for accelerated reactivation/sponsorship ^[raw/articles/gemini-career-outlook-2026-10-16.md]

## Relevance to Career

- **Space/defense pedigree** — NASA on resume carries weight across tech and aerospace
- **Simulation & Human Factors background** — M.S. in Modeling & Simulation applied to space mission planning, telemetry visualization, ergonomic UI design, and standalone engineering tools ^[raw/articles/gemini-career-outlook-2026-10-16.md]
- **Legacy modernization** — "Breathing new life into legacy" refers to modernizing NASA's aging web/internal engineering tools
- **AI opportunity** — NASA increasingly interested in AI for mission planning, data analysis, autonomy; internal advocate potential
- **Huntsville connection** — Marshall Space Flight Center is a major NASA facility

## Tech Stack & Team Transfer (April 2026)

- **October 2025 Shutdown / Hospice Incident (Previous Group):** Right after the October 2025 government shutdown began, Rick's mother entered hospice. A key NASA customer/stakeholder callously told Rick he should have *"planned ahead"* and *"coordinated with the other team members"* to finish his project while civil servants were at home not working. Rick took **short-term disability** to recover from the burnout/grief and requested a team transfer ^[raw/articles/gemini-career-outlook-2026-10-16.md].
- **April 2026 Lateral Transfer (Current Group):** Moved to a much calmer, more professional team in April 2026. While the group's default stack includes Microsoft PowerApps/Dataverse (which Rick dislikes and refuses to be pigeonholed into), he architected the current proposal/budget app using **Electron + React + TypeScript** interfacing with Dataverse ^[raw/articles/gemini-career-outlook-2026-10-16.md].

## Insourcing Initiative

NASA is actively executing a **workforce insourcing directive** to convert low-margin, cost-plus contractor positions to direct civil service hires (causing [[entities/amentum]] to project a 3% / ~$400M–$420M revenue headwind in FY2027) ^[raw/articles/gemini-career-outlook-2026-10-16.md]. Key implications:

- Rick **strongly opposes** working for NASA/government directly — both because of rigid federal bureaucracy/cold customer culture and because his $170K salary already hits the **2026 Huntsville GS-14 Step 10 ceiling ($170,207)**, where mandatory 4.4% FERS-FRAE deductions would cut his take-home pay (see [[queries/nasa-civil-service-gs-pay]]) ^[raw/articles/gemini-career-outlook-2026-10-16.md]
- Specialized software/GUI architects are harder for NASA to insource than generic administrative/staffing roles because the GS pay scale cannot compete with private defense rates ($185K+)
- **Remote work restriction:** Per **NPR 3600.2B § 6.1.6**, NASA prohibits remote work or telework from outside the United States and its territories (confirmed 2026-10-15)

## Current Project (2026)

Rick's new group (since April 2026) is building a **proposal and budget planning app** that:
- Centralizes proposal and budget data in one system
- Prevents errors from multiple spreadsheet versions circulating
- Eliminates duplicate entries that inaccurately exaggerate costs
- NASA stakeholders say it could have measurable **"six-figure" impact** (cost savings)
- **Tech stack:** Electron + React + TypeScript interfacing with Microsoft Dataverse via pacx
- Uses persistent PowerShell worker pattern for Dataverse CRUD (Option A) until IT grants Azure portal access
- Work env restricted: no Azure portal access, CodeApps not yet enabled
- This builds **transferable skills** (React + TypeScript + Dataverse + Electron) unlike pure PowerApps work

## Future Questions

- How does the FY2027 insourcing wave affect Rick's specific division under ESSCA II (~May 2027 start)?
- What is the outcome of the ~November 2026 annual raise cycle?

## Sources

- LinkedIn profile data ^[raw/articles/linkedin-ricksegrest-2026.md]
- User direct input | 2026-05-30
- Gemini Career Outlook export & user input | 2026-10-16 ^[raw/articles/gemini-career-outlook-2026-10-16.md]
