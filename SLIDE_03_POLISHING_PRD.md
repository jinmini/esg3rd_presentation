# [PRD] Polishing Slide 03 (`03-market-opportunity.html`)

- **Document Version**: 1.0
- **Context**: The workflow-centric design of this slide is strategically sound. We now need to refine the visual details to maximize its clarity and narrative impact.
- **Strategic Goal**: To visually reinforce the logical connections between the identified problem (the "Golden Path"), our capabilities, and the resulting benefits.

## 1. Key Areas for Improvement

1.  **"Golden Path" Badge Placement**: The current placement inside one box is misleading. It should represent the *connection* between the two key steps.
2.  **Visual Flow**: The connection between the top workflow and the middle capabilities section is not explicit enough.
3.  **Readability**: The key pain points and solutions in the bottom "Before/After" section could be more scannable.

## 2. Specific Requirements for `03-market-opportunity.html`

### Task 1: Reposition and Redesign the "Golden Path" Badge

-   **Objective**: To clarify that the "Golden Path" refers to the entire process from assessment to drafting.
-   **Action**:
    1.  Move the "GOLDEN PATH" badge so it is positioned **above and between** the "중요성 평가" and "보고서 초안" boxes.
    2.  **(Creative Freedom for Claude)** Consider adding a new visual element, like a glowing **arch or bracket** that spans over both boxes, and place the badge on top of this arch. This will visually group them as a single, critical process that we solve.

### Task 2: Strengthen the Visual Connection Between Sections

-   **Objective**: To visually guide the audience's eyes from the workflow to our specific solutions.
-   **Action**:
    1.  Draw thin, subtle lines connecting the highlighted workflow steps ("중요성 평가", "보고서 초안") to the corresponding capability cards below ("간소화된 중요성 평가", "GenAI 보고서 초안").
    2.  This will make the relationship "We solve *this step* with *this capability*" immediately obvious.

### Task 3: Enhance Readability in the "Before/After" Section

-   **Objective**: To make the key takeaways in the comparison lists instantly scannable.
-   **Action**:
    1.  In the "기존 방식의 한계" list, wrap the key pain points in `<strong>` tags. Examples: `<strong>2-3주 소요</strong>`, `<strong>고가의 컨설팅 의존</strong>`, `<strong>연결 단절</strong>`.
    2.  In the "우리의 혁신적 접근" list, do the same for the key benefits. Examples: `<strong>연결된 워크플로우</strong>`, `<strong>비용 절감</strong>`, `<strong>직접 보고서로 연결</strong>`.

## 3. Final Deliverables

1.  The complete, updated HTML code for `slides/03-market-opportunity.html`.
2.  Any new CSS classes added to `/assets/common.css` to support these refinements.