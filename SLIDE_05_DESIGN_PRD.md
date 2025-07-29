# [PRD] Redesign for Slide 05: The GRI Answer Engine

- **Document Version**: 1.0
- **Context**: This slide follows the "Automated Materiality Engine" (Slide 04). The audience now understands **HOW** we assess materiality. The next logical question is, "So what? How do you turn that assessment into an actual report?" This slide must answer that question.
- **Key Insight**: Based on the provided source code (`README.md`, `answer_service.py`, `gri_data_fixed_corrected.jsonl`), our core technological advantage is not just using a generic AI, but using a **specifically fine-tuned language model (`KoAlpaca-Polyglot-5.8B`)** on our own **GRI-standard dataset**. We also use a sophisticated **structured prompting** method.

## 1. Strategic Goal

To showcase our deep technical expertise in AI-powered report generation. We must move beyond a simple "AI writes the report" claim and explain **WHY** our AI is uniquely qualified for this task. The slide must build immense technical credibility and seamlessly transition into a live product demo.

## 2. Core Narrative: "A Specialist AI, Not a Generalist"

The central story is that we have built an "AI Specialist" – an expert in GRI reporting – not just a generic text generator. This is achieved through deliberate model selection, specific training (fine-tuning), and a rigorous process.

## 3. Functional & Visual Requirements

The slide should be structured in three distinct sections to tell this story.

### Section 1: The Making of an Expert AI (The "Model")

-   **Objective**: Explain how our AI model was created and why it's special.
-   **Visual Concept**: An "AI Model Factory" or "Training Lab" diagram.
-   **Required Elements**:
    1.  **Inputs**:
        -   An icon/logo representing a powerful base model: `EleutherAI/polyglot-ko-5.8b`.
        -   An icon representing our proprietary training data: `GRI Training Dataset` (our `.jsonl` file).
    2.  **Process**:
        -   A central visual element representing the **"Fine-Tuning Process"**.
    3.  **Output**:
        -   The final, specialized model: **`KoAlpaca-GRI Specialist Model`**. This should look more refined and intelligent than the base model.
-   **Key Message (to be displayed as a headline for this section)**: "We Don't Use a Generic AI; We Trained a GRI Specialist."

### Section 2: The 3-Step Answer Generation Process (The "Process")

-   **Objective**: Show the step-by-step process of how the assessment results from Slide 04 are converted into a report draft.
-   **Visual Concept**: A process flow diagram that starts with the output from the previous slide.
-   **Required Steps**:
    1.  **Step 1: Contextual Prompting**
        -   **Description**: "User answers and GRI standards are combined into a structured, intelligent prompt for our AI."
        -   **Visual Aid**: A simplified visual representation of the structured prompt from `answer_service.py`.
    2.  **Step 2: AI Draft Generation**
        -   **Description**: "Our GRI Specialist Model generates a professional, compliant paragraph based on the prompt."
        -   **Visual Aid**: The prompt from Step 1 flows into our `KoAlpaca-GRI` model icon, and a polished text draft emerges.
    3.  **Step 3: Human-in-the-Loop (Review & Approve)**
        -   **Description**: "Users review, edit, and give final approval, turning the AI draft into an official corporate asset."
        -   **Visual Aid**: An icon of a person reviewing the text and clicking an "Approve" button.

### Section 3: Transparency & Demo Pivot (The "Reality Check")

-   **Objective**: To be transparent about our current capabilities and limitations, and to create a perfect transition to the live demo.
-   **Visual Concept**: A clean, concise information box at the bottom of the slide.
-   **Required Content**:
    -   **`Framework Focus`**: State that we are optimized for **GRI Standards**. Explain *why* (global standard, structured, ideal for AI).
    -   **`Current Limitations`**: Clearly state that other standards like `ESRS` or `SASB` are not yet supported. Explain *why* (they require separate, dedicated fine-tuning). Mention this is on the roadmap.
    -   **`Call to Action / The Pivot`**: A clear, forward-looking statement: **"Now, let's see this engine in action. (Live Demo)"**

## 4. Creative Freedom

The specific layout, iconography, animations, and overall aesthetic are up to your creative judgment. The goal is to make this complex technical information feel accessible, impressive, and professional. Please ensure the final design is visually consistent with the "Automated Materiality Engine" slide.

## 5. Final Deliverables

1.  The complete, redesigned HTML code for `slides/05-solution-overview.html` (or a more appropriately named file like `05-answer-engine.html`).
2.  Any necessary additions or modifications to `/assets/common.css`.
