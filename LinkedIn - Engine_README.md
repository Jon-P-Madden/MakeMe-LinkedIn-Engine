# Make Me! LinkedIn Optimization Engine

**Make Me! LinkedIn Optimization Engine** is an AI-assisted profile optimization tool that turns a LinkedIn profile into a recruiter-searchable positioning page.

Part of the **Make Me!** career tools suite - built by a Senior Technical Program Manager to solve real job search problems with practical AI-assisted workflows.

Most LinkedIn advice is generic. This engine aligns searchability, credibility, and positioning.

No installation. No backend. No friction.

![Make Me! LinkedIn Optimization Engine](Screenshot.png)

---

## What This Demonstrates

- Product design for a public professional profile, not just a resume rewrite
- AI-assisted LinkedIn diagnosis and profile improvement
- Recruiter-search keyword strategy connected to target roles
- Structured output for headline, About, experience, skills, and Featured sections
- Resume-to-LinkedIn consistency thinking across the Make Me suite
- Browser-first prototype architecture with local saved output

---

## The Problem

LinkedIn profiles often fail for two different audiences at the same time. Recruiters cannot find them because the right keywords are missing, and humans cannot quickly understand them because the profile does not tell a clear story.

Generic LinkedIn advice usually says to "optimize your headline" or "add keywords," but it rarely connects profile content to the user's actual resume, target roles, credibility signals, and recruiter search behavior.

---

## The Solution

The engine helps users turn a static profile into a clearer positioning page:

1. Captures the current LinkedIn profile, resume/background, target roles, and desired positioning
2. Reviews the profile for searchability, credibility, proof, and consistency
3. Recommends recruiter-search keywords and title positioning
4. Generates improved headline and About section content
5. Guides experience, skills, Featured, and Open to Work improvements
6. Produces a LinkedIn optimization package the user can review and apply manually

The workflow is designed to help a profile read better to people and surface better in recruiter searches.

---

## Design Constraints (Intentional)

- Single-file browser prototype for portability and easy review
- No backend required for the current prototype
- Runtime API key input instead of stored secrets
- Browser `localStorage` persistence for saved LinkedIn packages
- Browser-first workflow for user-controlled review and editing
- Output designed for manual LinkedIn updates rather than automated account changes
- Profile guidance aligned with resume and application positioning

---

## Features

### Profile Intake

- Current LinkedIn profile intake
- Resume or career background input
- Target role and industry context
- Desired positioning and search direction
- Job description context when available

### AI Diagnosis

- Recruiter searchability review
- Credibility and proof review
- Keyword alignment analysis
- Resume-to-LinkedIn consistency notes
- Profile completeness guidance

### Profile Optimization

- LinkedIn headline options
- About section draft
- Experience section rewrite guidance
- Skills recommendations
- Featured section ideas
- Open to Work title recommendations

### Save / Export

- Saved LinkedIn optimization packages
- Downloadable text output in the prototype
- Local browser persistence
- Reviewable recommendations before the user updates LinkedIn manually

---

## Architecture

```text
User Browser
  |
  v
LinkedIn Optimization UI
  |
  +--> Profile, resume, and target-role intake
  |
  +--> localStorage saved LinkedIn packages
  |
  +--> Profile diagnosis and optimization workflow
  |       |
  |       v
  |   Runtime-selected AI provider/model
  |
  v
Headline options, About draft, skills strategy, Featured ideas, and search keywords
```

The engine operates as a browser-first prototype. It captures profile and target-role context, uses local browser storage for saved packages, routes analysis through a runtime-selected AI provider, and returns structured recommendations the user can apply to LinkedIn manually.

---

## Setup

1. Clone or download the repository.
2. Open `app/engines/linkedin-profile.html` in a browser.
3. Enter an API key for the selected AI provider when prompted by the app.
4. Paste or summarize the current LinkedIn profile and target direction.
5. Generate the profile diagnosis and optimization package.
6. Review the recommendations and manually apply selected updates to LinkedIn.

**No installation. No build step. No server.**

---

## Known Limitations

- Client-side API calls are prototype-oriented and may depend on provider browser policies.
- `localStorage` is browser-local and does not sync across devices.
- The prototype does not automatically update LinkedIn.
- Generated profile copy should be reviewed and personalized before publishing.
- AI output parsing and validation can be hardened in future versions.
- There is no backend, database, authentication, or cloud sync in the current prototype.

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript
- Browser `localStorage`
- Runtime AI provider/API key input
- No backend
- No database
- No build tooling required for the prototype

---

## Roadmap

- Add stronger resume-to-LinkedIn consistency checks
- Improve recruiter keyword recommendations by role family
- Add saved version comparison
- Expand export/report formats
- Support richer profile diagnostics
- Integrate with Recruiter Outreach messaging context once that engine is built

---

## Part of the Make Me! Suite

| Engine | Tool | Purpose |
|--------|------|---------|
| Engine 1 | **Make Me! Resume Positioning Engine** | Build a strategically positioned resume from raw career history |
| Engine 2 | **Make Me! Application Engine** | Analyze job postings, tailor application materials, generate cover letters, and track applications |
| Engine 3 | **Make Me! LinkedIn Optimization Engine** | Optimize LinkedIn profiles for recruiter searchability and credibility |
| Engine 4 | **Make Me! Interview Prep Engine** | Planned engine for interview questions, STAR stories, and role-specific prep |
| Engine 5 | **Make Me! Salary Negotiation Engine** | Planned engine for compensation strategy, counteroffers, and negotiation messaging |
| Engine 6 | **Make Me! Recruiter Outreach Engine** | Planned engine for recruiter, referral, and networking outreach |

---

## Why This Exists

LinkedIn is not just an online resume. It is a search surface, credibility layer, and first impression all at once.

This engine exists because job seekers need more than generic profile tips. They need a way to connect their resume story, target roles, keywords, proof points, and recruiter discovery strategy into one coherent profile. The LinkedIn Optimization Engine helps make that connection practical.

- **Profile design** - treats LinkedIn as search surface, credibility layer, and story page
- **AI as interpreter** - model output used to connect resume context to recruiter search behavior
- **Workflow thinking** - diagnosis, rewrite guidance, skills, Featured strategy, and keywords in one flow
- **Constraint-driven architecture** - browser-first, local-first, and portable

---

## License

MIT — use it, fork it, adapt it.

---

*Built by Jonathan Madden*
*[LinkedIn](https://linkedin.com/in/jonathan-p-madden) - [github.com/Jon-P-Madden](https://github.com/Jon-P-Madden)*
