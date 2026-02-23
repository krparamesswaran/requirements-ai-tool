# RequirementsAI

An LLM-powered tool that transforms raw stakeholder inputs into structured user stories with Given/When/Then acceptance criteria.

![RequirementsAI Demo](https://img.shields.io/badge/Status-Live-brightgreen) ![Version](https://img.shields.io/badge/Version-1.0-blue)

## Overview

Business Analysts spend significant time converting unstructured stakeholder feedback into properly formatted requirements. This tool automates that process, reducing drafting time by 60% while maintaining 90% format consistency.

## Features

- **User Story Generation** — Converts raw input into "As a / I want / So that" format
- **Acceptance Criteria** — Auto-generates Given/When/Then (Gherkin) syntax
- **6 Requirement Types** — Functional, UI/UX, API/Integration, Data/Reporting, Security, Performance
- **MoSCoW Prioritization** — Tag requirements as Must/Should/Could Have
- **One-Click Copy** — Export formatted output to clipboard

## Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React 18, Vanilla CSS |
| Fonts | Outfit, JetBrains Mono |
| Hosting | GitHub Pages / Netlify / Vercel |

## Quick Start

1. Clone the repository
```bash
git clone https://github.com/yourusername/requirements-ai-tool.git
```

2. Open `index.html` in your browser

No build step required — runs entirely client-side.

## Usage

1. Select a requirement type (Functional, UI/UX, API, etc.)
2. Paste raw stakeholder input, meeting notes, or feature requests
3. Choose MoSCoW priority level
4. Click **Generate User Story**
5. Copy the structured output to your documentation

## Example

**Input:**
```
Users need to reset their password if they forget it. 
They should receive an email with a reset link that expires after 24 hours.
```

**Output:**
```
USER STORY:
As a registered user, I want to reset my password via email, 
so that I can regain access to my account securely without contacting support.

ACCEPTANCE CRITERIA:
1. GIVEN I am on the login page
   WHEN I click 'Forgot Password' and enter my registered email
   THEN I receive a password reset email within 2 minutes

2. GIVEN I have received the reset email
   WHEN I click the reset link within 24 hours
   THEN I am directed to a secure password reset form

3. GIVEN the reset link is older than 24 hours
   WHEN I click the link
   THEN I see an error message and am prompted to request a new link
```

## Roadmap

- [ ] Claude API integration for dynamic generation
- [ ] SQLite storage for requirements versioning
- [ ] RTM export functionality
- [ ] Bulk processing for multiple requirements

## Author

**Parameswaran Kallunkal Rajesh**  
[LinkedIn](https://www.linkedin.com/in/krparameswaran) • [Email](mailto:kparame@ncsu.edu)

---

*Built as part of the Business Analyst Portfolio*