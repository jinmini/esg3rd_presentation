# [PRD] Polishing the Title Slide (`01-title.html`)

- **Document Version**: 1.0
- **Context**: The presentation structure is complete. We are now in the final polishing phase to maximize the delivery and impact of each slide. We will start with the first impression: the title slide.
- **Strategic Goal**: To transform the static title slide into a more dynamic, perfectly aligned, and visually impactful introduction that reflects the presentation's new theme of "journey and learning."

## 1. Key Areas for Improvement

1.  **Alignment**: The three keyword icons and their text are not perfectly visually aligned.
2.  **Emphasis**: The key subtitle "도전, 학습, 그리고 미래 비전" lacks visual emphasis.
3.  **Dynamics**: The slide is too static and could benefit from subtle animations to increase engagement.

## 2. Specific Requirements for `01-title.html`

### Task 1: Refine Icon Section Layout

-   **Objective**: To achieve perfect visual alignment for the three keyword sections.
-   **Action**:
    1.  Wrap each of the three keyword sections (icon + Korean title + English subtitle) in its own `div` container with a class like `.keyword-item`.
    2.  Use a flexbox container for these three items and apply styles to ensure they are perfectly top-aligned (`align-items: flex-start`), solving the subtle misalignment.

### Task 2: Enhance the Main Subtitle

-   **Objective**: To give more visual weight to our presentation's core theme.
-   **Action**:
    1.  In the subtitle `AI 기반 ESG 보고 자동화 플랫폼 개발 여정: 도전, 학습, 그리고 미래 비전`, apply the existing `.highlight` class or a similar emphasis style to the keywords **"도전, 학습, 그리고 미래 비전"**.
    2.  Consider adding subtle decorative elements around this line to make it stand out as a key theme.

### Task 3: Implement Subtle Entry Animations

-   **Objective**: To make the slide feel more professional and engaging upon loading.
-   **Action**: Use CSS to apply gentle `fade-in-up` animations to the elements in a specific sequence:
    1.  **First**: The `accent-line` should animate (e.g., width from 0 to 100%), followed by the main title "ESG GenAI" fading in.
    2.  **Second**: The subtitles fade in.
    3.  **Third**: The three `.keyword-item` containers fade in sequentially with a slight delay between each (a staggered effect).
-   **Note**: The animations should be quick and professional, not distracting. A duration of 0.5s to 0.8s is ideal.

## 3. Final Deliverables

1.  The complete, updated HTML code for `slides/01-title.html`.
2.  Any new CSS classes or animations added to `/assets/common.css` to support these changes.