# [PRD] Redesign for Presentation Finale (Slides 06-08)

- **Document Version**: 1.0
- **Context**: We have successfully established the problem and demonstrated our core solution (Materiality Engine & Answer Engine). Now, we need to craft a powerful closing sequence that builds maximum credibility and leads to our final "Ask."
- **Strategic Goal**: To streamline the final part of the presentation by consolidating slides, removing redundancy, and creating a compelling three-act structure: **Proof → Vision → Ask**.

---

## 1. Overview of Changes

This refactoring involves a significant restructuring of the presentation's latter half.

**Slides to be Deleted:**
-   `06-key-features.html`
-   `07-technology-architecture.html`

**Slides to be Kept & Re-ordered:**
-   `08-project-milestones.html` → becomes the new **`06-proven-execution.html`**
-   `09-roadmap.html` → becomes the new **`07-roadmap.html`**
-   `10-resource-requests.html` → becomes the new **`08-the-ask.html`**
-   `11-qa.html` → becomes the new **`09-qa.html`**

The total number of slides will be reduced to 9 (+ Q&A).

---

## 2. Task 1: Create the New Consolidated Slide `06-proven-execution.html`

**Objective**: To merge the core messages of three slides (Key Features, Tech Architecture, Project Milestones) into one powerful slide that proves our ability to execute.

### 2.1. File Operations

1.  **Delete** `slides/06-key-features.html` and `slides/07-technology-architecture.html`.
2.  **Rename** `slides/08-project-milestones.html` to `slides/06-proven-execution.html`.

### 2.2. Content & Design Requirements for the New `06-proven-execution.html`

-   **Main Title**: "증명된 실행력과 기술 기반 (Proven Execution & Technology Foundation)"
-   **Core Visual**: A timeline representing our key project milestones (content from the original `08-project-milestones.html`).
-   **Integration Requirement 1 (Value Proof)**:
    -   For each milestone on the timeline, integrate the most impactful results from the old `06-key-features.html`.
    -   Instead of just "MVP Launched," it should be "MVP Launched," followed by a key KPI like **"Result: 90% reduction in report drafting time."** This directly connects our actions to tangible value.
-   **Integration Requirement 2 (Technology Proof)**:
    -   Below the timeline, include a **highly simplified version** of the technology architecture from the old `07-technology-architecture.html`.
    -   This should not be a complex diagram. A clean, 4-block visual (`Frontend`, `Backend API`, `AI Core`, `Database`) is sufficient to convey technical solidity without overwhelming the audience.
-   **Overall Narrative**: The slide must tell this story: "Based on this **solid technology foundation**, we have achieved these **concrete milestones**, which have resulted in this **proven value**."

---

## 3. Task 2: Re-number and Verify Subsequent Slides

**Objective**: To ensure the rest of the presentation reflects the new structure and maintains a logical flow.

### 3.1. File Renaming

1.  Rename `slides/09-roadmap.html` to **`slides/07-roadmap.html`**.
2.  Rename `slides/10-resource-requests.html` to **`slides/08-the-ask.html`**.
3.  Rename `slides/11-qa.html` to **`slides/09-qa.html`**.

### 3.2. Content Verification & Link Updates

-   For each of the renamed slides (`07`, `08`, `09`), please verify and update the following:
    -   **Footer**: The slide number must be updated (e.g., "7/9", "8/9").
    -   **Navigation Component (`.slide-nav`)**: The `href` links for "Previous" and "Next" buttons must be updated to point to the correct new filenames.
    -   **JavaScript Navigation**: Any hardcoded links within `<script>` tags must also be updated. (Note: This will be fully resolved in Phase 2, but for now, please update the static links).

---

## 4. Final Deliverables

1.  The complete HTML code for the newly designed **`slides/06-proven-execution.html`**.
2.  Confirmation that the renaming and link/content updates for slides 07, 08, and 09 have been completed.
3.  (Optional but helpful) A list of the final, updated filenames for the entire presentation.