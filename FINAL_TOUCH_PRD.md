# [PRD] Final Touches for Slides 01 and 09

- **Document Version**: 1.0
- **Context**: The core narrative of our presentation has evolved from a business pitch to a story of "learning, limitations, and vision." We need to ensure the very first and very last slides align perfectly with this new, more authentic narrative.

## Task 1: Refine the Title Slide (`01-title.html`)

- **Objective**: To set the right expectation from the very beginning, hinting at the journey of learning and discovery.
- **Requirements**:
  1.  **Update the Subtitle**:
      -   **Current**: `<p class="body-large text-muted mb-20">AI 기반 ESG 보고 자동화 플랫폼</p>`
      -   **New**: Replace the current subtitle with a two-line version that frames the presentation as a journey.
          ```html
          <p class="body-large text-muted mb-20">
              AI 기반 ESG 보고 자동화 플랫폼 개발 여정: <br>
              <span class="highlight">도전, 학습, 그리고 미래 비전</span>
          </p>
          ```
  2.  **Update the Footer**:
      -   Change the slide number from `1/12` to `1/9`.

## Task 2: Refine the Q&A Slide (`09-qa.html`)

- **Objective**: To pivot the Q&A session away from a business/investment context towards a technical and academic discussion, maintaining the authenticity of our new narrative.
- **Requirements**:
  1.  **Update the "Thank You" Message**:
      -   Change the focus from `MVP 성과와 향후 비전` (MVP achievements and future vision) to a phrase like `개발 과정에서의 학습과 미래에 대한 제언` (learnings from the development process and proposals for the future).
  2.  **Completely Overhaul the "Welcomed Questions" Section**:
      -   **Change the title** from "환영하는 질문 주제" to **"함께 논의하고 싶은 주제 (Topics for Discussion)"**.
      -   **Replace the old topics** (Business Value, ROI, etc.) with the following new topics that encourage a reflective discussion:
          -   **Topic 1: Technical Challenges & Solutions**: "We welcome in-depth discussions on the technical/data limitations we faced and our proposed solutions."
          -   **Topic 2: The Future of ESG x AI**: "We would love to share ideas on how AI can further contribute to ESG reporting and strategy."
          -   **Topic 3: Learnings from the Project**: "Any questions about our technical and domain-specific learning process are welcome."
  3.  **(Optional but recommended)** Update the large Q&A graphic's sub-message to align with the new tone (e.g., "Let's talk about technical challenges and future visions").

## Final Deliverables

1.  The updated HTML code for `slides/01-title.html`.
2.  The updated HTML code for `slides/09-qa.html`.