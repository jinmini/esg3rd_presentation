# [PRD] Polishing Slide 04 (`04-materiality-engine.html`)

- **Document Version**: 1.0
- **Context**: The current version of this slide contains all the right information but suffers from layout issues, most critically requiring the user to scroll. A presentation slide must fit on a single screen.
- **Strategic Goal**: To redesign the layout to fit everything on one screen, create a stronger visual hierarchy that emphasizes the core "engine," and refine the design of the process diagram itself.

## 1. Key Areas for Improvement

1.  **Layout & Spacing**: The slide does not fit on one screen. The "Input" and "Benefits" sections take up too much vertical space.
2.  **Diagram Design**: The 5-step process boxes are misaligned and lack a cohesive, professional design.
3.  **Visual Hierarchy**: The core "engine" diagram is not treated as the main "hero" element of the slide.

## 2. Specific Requirements for a Complete Redesign

### Task 1: Consolidate Layout to a Single Screen

-   **Objective**: To eliminate the need for scrolling by repositioning ancillary information.
-   **Action**:
    1.  **Reposition the "Input" section**: Instead of large horizontal boxes at the top, change it to a **compact vertical list of small icons and labels** in the **top-left corner** of the slide.
    2.  **Reposition the "Benefits" section**: Instead of large horizontal boxes at the bottom, change it to a **compact vertical list of small icons and labels** in the **bottom-right corner** of the slide.
    3.  This will free up the entire central area of the slide for the main diagram.

### Task 2: Redesign the "Automated Engine" Process Diagram

-   **Objective**: To create a professional, clear, and visually appealing process flow diagram.
-   **Action**:
    1.  Place the 5-step process diagram horizontally in the now-empty central space.
    2.  **Unified Box Design**: Redesign all five process boxes to have a **consistent size, style, and centered alignment** for icons and text.
    3.  **Highlight the Core Step**: Make the **"Scoring" (점수 산정) box visually distinct** (e.g., with a different background color or a glowing border `box-shadow`) to emphasize its importance. Keep the `⭐ ESRS COMPLIANT` badge prominent.
    4.  **Clear Connectors**: Use clean, bold arrows between the boxes to clearly show the left-to-right process flow.

### Task 3: Re-organize Supporting Information

-   **Objective**: To logically place the remaining content blocks around the main diagram.
-   **Action**:
    1.  Place the yellow **"ESRS 표준 준수 점수 산정"** info box directly **below** the 5-step diagram. It should feel like a footnote or detailed explanation for the "Scoring" step.
    2.  Place the green **"최종 산출물: Double Materiality Matrix"** info box directly **below** the ESRS info box, positioning it as the final, ultimate output of the entire process.

## 3. Final Deliverables

1.  The complete, redesigned HTML code for `slides/04-materiality-engine.html` that fits on a single screen.
2.  Any necessary CSS additions or modifications to `common.css` to support this new, compact, and refined layout.