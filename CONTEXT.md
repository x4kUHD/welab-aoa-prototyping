# Project Context

Background for the research project this repo's prototypes support. For agent coding rules, see `AGENT.md`.

## Current Feature: Asset Tracking

This is the feature currently being prototyped in this repo, part of the PMS's **Monitor** module (see 3M Framework below).

- **Owners:** Eric, Marleigh, Reese, Bihan
- **Fields per asset:**
  - Life expectancy tracking (remaining years)
  - Location of the asset
  - Manufacturer
  - Initial cost and accrual (accrued/depreciated) cost
  - Document holder — attach manuals/instructions per asset

## Executive Summary

- **Project Title:** Strategic Facility Management and Community-Driven Approach to Resilience Hub Design within the Archdiocese of Atlanta (Part I: Georgia Tech)
- **Authors/Team:** Georgia Tech WE Lab (Eunhwa Yang, Ph.D., Ibrahim Bilau, Ph.D., James Holder II, Josie Chang, Ruby Kim, Rayeed Zaman, Jeff Ross-Bain)
- **Date:** July 2026
- **Problem Statement:** Faith-based institutions manage millions of square feet of complex physical assets (worship space, schools, offices) under conditions of limited capital, aging building infrastructure, and heavy volunteer dependency. FM research traditionally ignores this sector, leaving institutions trapped in a reactive maintenance culture with informal knowledge retention and fragmented data.

## Key Frameworks

### 1. Four Core FM Domains (Phase I)

1. **Sustainability & Energy Stewardship** — Managing high Energy Use Intensity (EUI) caused by intermittent/surge occupancy patterns.
2. **Operations & Maintenance (O&M)** — Shifting away from reactive, volunteer-dependent repairs without CMMS coverage.
3. **Business & Governance Processes** — Linking dispersed, informal operational data with parish finance councils and clergy leadership.
4. **Life-Cycle Decision-Making & Heritage** — Balancing long-term capital asset preservation against aging infrastructure and deferred maintenance.

### 2. The 3M Framework (Phase III)

- **Monitor** — Systematically tracking utility usage, asset appraisals, and active facility risk/condition backlogs.
- **Manage** — Operationalizing task tracking, inline work orders, priority level assignments, and changelogs.
- **Money** — Framing facility conditions in direct financial metrics (spend by utility, monthly cost estimates, valuation, recapitalization reserves) for governance/finance council action.

## Empirical Research: Pilot Parishes (Phase II)

### St. Anthony of Padua (Atlanta, West End)

- **Profile:** Urban, historic campus (founded 1903; sanctuary built 1924)
- **Operations:** Volunteer-run, no formal work order system, aging MEP/boiler systems, high reliance on institutional memory
- **Benchmarking:** Source EUI of 52 kBtu/ft²/yr (vs. median 58 kBtu/ft²/yr); Site EUI of 30 kBtu/ft²/yr

### St. Joseph (Marietta, GA)

- **Profile:** Suburban campus (~8 acres, 5 buildings including a K–8 school, total 107,882 sq ft)
- **Operations:** Dedicated facilities manager, structured governance, security infrastructure (109 cameras), proactive O&M capacity
- **Benchmarking:** Source EUI of 79 kBtu/ft²/yr (vs. median 58 kBtu/ft²/yr); Site EUI of 30 kBtu/ft²/yr

## Key Deliverables & System Architecture (Phase III)

### Primary Deliverable: Parish Management System (PMS)

- **Tech Stack & Security:** Web application featuring Auth0 secure authentication with role-based access control. (Note: this prototyping repo does not use this stack — see `AGENT.md`.)
- **Core Modules & Functionality:**
  - **Dashboard** — Card-based UI designed to lower cognitive load for low-tech/volunteer users. Features inline editing for parish and building metadata.
  - **Utilities Tracking** — Upload and account assignment for Electricity, Gas, Water, and Waste by specific building.
  - **Appraisal Entry** — Text-parsing interface for uploading building appraisals and structural valuations directly into the risk/backlog engine.
  - **Active Risks & Backlog Registry** — Building-level division of maintenance tasks with priority status tagging (Overdue, Due Soon, Addressed).
  - **Finances View** — Automated breakdown of expenses by utility type and by individual building to translate facility risks into finance-council-ready presentations.
  - **History & Audit Log** — Sortable changelog tracking task modifications, status updates, and deletions to preserve institutional memory.

### Alternative Deliverable: Excel-Based FM Toolkit

- **Components:** Google Form/Sheet connected to an Excel Action Tracker dashboard, a Condition-Based Asset Inventory (CBI), and a Budget Tracker.
- **Positioning:** Offline/low-cost fallback for low-capacity parishes, though prone to spreadsheet link failure compared to the unified web-based PMS.

## Research Takeaways & Strategic Future Roadmap

- **Diagnostic Boundary:** The current tools successfully transition parishes from reactive management to diagnostic organization.
- **The Predictive Gap:** Existing tools do not yet provide predictive analytics (e.g., forecasting equipment failure timing, financial degradation modeling, automated risk prioritization) due to cross-sectional data limits.
- **Future PMS Roadmap:** Usability testing, cross-parish portfolio analytics, PDF reporting export, and building predictive algorithms via longitudinal utility/maintenance datasets.
