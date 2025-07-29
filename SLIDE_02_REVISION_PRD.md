# [PRD] Complete Redesign for Slide 02: From "Executive Summary" to "Team & Roles"

- **Document Version**: 1.0
- **Context**: Our presentation has pivoted from a business pitch to a story of a student project's "journey, learning, and vision." The current "Executive Summary" slide (02) is a remnant of the old business pitch narrative and feels out of place.
- **Strategic Goal**: To replace the summary with a "Team & Roles" slide. This will build credibility, add a human element to the presentation, and showcase the diverse skill set that made this project possible.

## 1. Task: Complete Overhaul of `02-executive-summary.html`

### 1.1. File Operation

-   **Rename** `slides/02-executive-summary.html` to **`slides/02-team-and-roles.html`**.

### 1.2. New Content & Design Requirements

-   **Main Title**: "Our Team: The Architects of ESG GenAI" or "우리의 여정을 함께한 팀"
-   **Subtitle**: "각자의 전문성으로 AI 기반 ESG 솔루션의 초석을 다졌습니다."
-   **Design Concept**: A clean, professional layout featuring four distinct profile cards, one for each team member.

### 1.3. Profile Card Structure (Repeat for all 4 members)

-   Each card should contain:
    1.  A placeholder for a **profile picture or an avatar icon** at the top.
    2.  The team member's **Name/Initial** (e.g., "A").
    3.  The team member's **Role** (e.g., "AI Engineer"), styled prominently.
    4.  A concise, one or two-sentence description of their **Key Contribution**, paired with a relevant icon.

### 1.4. Specific Content for Each Team Member

-   **Team Member A**:
    -   **Role**: AI Engineer
    -   **Icon**: `fas fa-robot`
    -   **Contribution**: "Built the core AI engine for report generation, from selecting and fine-tuning the HuggingFace model to deploying the API."

-   **Team Member B**:
    -   **Role**: Data Engineer
    -   **Icon**: `fas fa-database`
    -   **Contribution**: "Constructed the high-quality, GRI-compliant training dataset that serves as the brain of our specialized AI model."

-   **Team Member C**:
    -   **Role**: Frontend Developer
    -   **Icon**: `fas fa-desktop`
    -   **Contribution**: "Translated the complex workflow of ESG practitioners into an intuitive UI and an interactive dashboard, crafting the user experience."

-   **Team Member F**:
    -   **Role**: Backend & DevOps
    -   **Icon**: `fas fa-cogs`
    -   **Contribution**: "Developed the Materiality Assessment API and engineered the robust infrastructure (DevOps) for stable service operation."

## 2. Final Deliverables

1.  The complete, redesigned HTML code for the new `slides/02-team-and-roles.html`.
2.  Any necessary CSS additions to `common.css` to support the new profile card layout.
3.  Confirmation that the navigation links in `01-title.html` and `03-market-opportunity.html` are updated to point to this new slide.