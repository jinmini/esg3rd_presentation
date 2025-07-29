# [PRD] Redesign for Presentation Finale (v2): Learnings & Vision

- **Document Version**: 2.0
- **Context**: We are pivoting the presentation's finale. Instead of a business-oriented "Roadmap & ROI," we will adopt a more reflective and forward-looking approach suitable for a student/demo project.
- **Strategic Goal**: To conclude the presentation by demonstrating the deep learnings gained from the project, being transparent about its limitations, and proposing a thoughtful vision for future improvements. This showcases maturity, critical thinking, and technical insight over a premature business plan.

---

## 1. Overview of Changes

This PRD replaces the previous plan for slides 07 and 08. The core structure will be a two-act finale: **"Reflection on Limitations" → "Vision for Enhancements"**.

**Slides to be Redesigned:**
-   `07-roadmap.html` → becomes the new **`07-learnings-and-limitations.html`**
-   `08-the-ask.html` → becomes the new **`08-future-vision.html`**

**Slides to be Updated:**
-   `06-proven-execution.html`: Navigation must point to the new `07-learnings-and-limitations.html`.
-   `09-qa.html`: Navigation must point from the new `08-future-vision.html`.

---

## 2. Task 1: Redesign Slide 07 as "Learnings & Limitations"

**Objective**: To honestly reflect on the realistic challenges encountered during the project, thereby showcasing a deep understanding of the problem domain.

### 2.1. File Operation

-   **Rename** `slides/07-roadmap.html` to **`slides/07-learnings-and-limitations.html`**.

### 2.2. Content & Design Requirements

-   **Main Title**: "프로젝트를 통해 마주한 현실적 과제 (Learnings & Current Limitations)"
-   **Design Concept**: A "research note," "whiteboard," or "blueprint" theme. It should feel like a transparent look into our development process, not a polished marketing slide.
-   **Core Content**: The slide must be structured around three key limitations we faced. For each, describe the problem and what we learned from it.

    1.  **Limitation 1: Data Accessibility**
        -   **Icon**: A visual representing inaccessible or incomplete data (e.g., `fas fa-file-excel` with a lock icon).
        -   **Problem Statement**: "Lacked access to real-time, quantitative corporate data (e.g., energy usage, waste volume). Our analysis was thus focused on qualitative, publicly available text data."
        -   **Key Learning**: "We learned that building a robust, reliable data pipeline for quantitative metrics is the absolute prerequisite for a truly comprehensive ESG reporting tool."

    2.  **Limitation 2: Process Integration**
        -   **Icon**: A broken link or chain (`fas fa-link-slash`).
        -   **Problem Statement**: "The data flow between the 'Materiality Assessment' (Slide 04) and the 'GRI Answer Engine' (Slide 05) is not yet fully automated."
        -   **Key Learning**: "We realized the critical importance of a standardized data schema to create a seamless user experience between different analytical modules."

    3.  **Limitation 3: Computational Constraints**
        -   **Icon**: A visual for high server load or processing power (e.g., `fas fa-microchip` with a heat symbol).
        -   **Problem Statement**: "Fine-tuning and serving a large language model like KoAlpaca-5.8B locally required significant GPU resources and time, posing a scalability challenge."
        -   **Key Learning**: "We understood the necessity of MLOps infrastructure, cloud-based serving, and model optimization techniques (like quantization/distillation) for a viable commercial service."

---

## 3. Task 2: Redesign Slide 08 as "Future Vision"

**Objective**: To demonstrate foresight by proposing specific, intelligent solutions to the limitations identified in the previous slide.

### 3.1. File Operation

-   **Rename** `slides/08-the-ask.html` to **`slides/08-future-vision.html`**.

### 3.2. Content & Design Requirements

-   **Main Title**: "더 나은 ESG 보고 지원을 위한 제언 (Future Enhancements & Vision)"
-   **Design Concept**: A bright, forward-looking, "blueprint" or "mind-map" theme. It should feel optimistic and innovative, showing ideas branching out.
-   **Core Content**: Structure the slide around three key enhancements that directly address the limitations from slide 07.

    1.  **Enhancement 1: Real-time Data Integration Dashboard**
        -   **Icon**: A dashboard icon (`fas fa-tachometer-alt`).
        -   **Proposed Solution**: "Develop a dashboard that integrates with corporate systems (like ERP) to collect and analyze quantitative data in real-time, dramatically improving assessment accuracy."
        -   *(This directly solves the "Data Accessibility" limitation.)*

    2.  **Enhancement 2: End-to-End Automated Workflow**
        -   **Icon**: Interconnected gears (`fas fa-cogs`).
        -   **Proposed Solution**: "Create a seamless, one-click workflow where a prioritized issue from the materiality assessment automatically generates the corresponding GRI report draft."
        -   *(This directly solves the "Process Integration" limitation.)*

    3.  **Enhancement 3: Lightweight, Domain-Specific Models**
        -   **Icon**: A feather or lightning bolt icon (`fas fa-feather-alt`).
        -   **Proposed Solution**: "Develop smaller, highly specialized models (via distillation/quantization) for each reporting standard (GRI, ESRS, etc.) to ensure faster, more cost-effective, and scalable AI performance."
        -   *(This directly solves the "Computational Constraints" limitation.)*

---

## 4. Final Deliverables

1.  The complete HTML code for the newly designed **`slides/07-learnings-and-limitations.html`**.
2.  The complete HTML code for the newly designed **`slides/08-future-vision.html`**.
3.  Confirmation that all navigation links and footers in slides `06`, `07`, `08`, and `09` are correctly updated to reflect the new structure.