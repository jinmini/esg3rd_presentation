# [PRD] Revise Slide 05: GRI Answer Engine Deep Dive (v1.1)

- **Document Version**: 1.1
- **Target Slide**: `05-gri-answer-engine.html`
- **Action**: **Complete redesign** of the existing slide based on critical feedback. The previous attempt was insufficient.

## 1. Goal & Strategic Purpose (REVISED - CRITICAL)

The previous version failed to convey the core story. The **primary goal is to clearly communicate our unique philosophy and methodology.**

- **Key Story to Emphasize**: We consciously pivoted from benchmarking traditional "energy production" companies (like Korea Midland Power) to forward-thinking **"energy utilization" leaders (like Doosan Fuel Cell, LS ELECTRIC, Hyundai Motor)**. This strategic choice is what makes our AI a true specialist. **This narrative MUST be explicitly stated in the slide's text.**

## 2. Layout & Visual Requirements (REVISED - CRITICAL)

The current vertical layout is long and confusing. We must switch to a **"Two-Column Layout"**.

- **Left Column (The "Why & How" - 40% of width)**: This column tells the story.
  1.  **Title**: "GRI Answer Engine"
  2.  **"Our Philosophy" Section (New Text)**: Add a dedicated text block at the top stating: _"우리는 '에너지 생산'을 넘어 **'에너지 활용'**에 집중합니다. 한국중부발전 모델이 아닌, **두산퓨얼셀, LS ELECTRIC** 등 미래 에너지 리더들의 ESG 전략을 AI에 학습시켰습니다."_
  3.  **3-Step Process**: Below the philosophy, display the 3-step process (Prompting → Generation → Review) in a compact, vertical list with icons.
  4.  **"Tech Spec" Box**: At the bottom of this column, place the tech spec box with the training data.

- **Right Column (The "What" - 60% of width)**: This column provides the visual proof.
  1.  **"AI Factory" Diagram**: Place the AI Factory diagram (Base Model → Fine-Tuning → Specialist Model) at the top of this column.
  2.  **Image Gallery**: Below the diagram, create a clean grid to display the three required images (use placeholders). Each image MUST have a clear title:
      - **Image 1 Title**: "Our Benchmarks"
      - **Image 2 Title**: "Structured Prompt Example"
      - **Image 3 Title**: "AI-Generated Draft"

## 3. Technical Implementation (REVISED - CRITICAL)

The previous attempt failed to meet the coding standards.
- **Code Cleanup is Mandatory**:
  - **Remove ALL inline styles (`style="..."`)**. Use utility classes or component classes in `common.css`.
  - **Remove the `<script>` and `<style>` tags from the HTML file**. All CSS must go into `common.css`. All JavaScript logic (like animations) must be placed in a temporary `<script>` tag but clearly marked with a `// TODO: Move to common.js in Phase 2` comment.
- **Create New CSS Components**: Create robust, reusable classes in `common.css` for the new layout elements (e.g., `.two-column-layout`, `.left-pane`, `.right-pane`, `.image-gallery`, `.image-gallery-item`).

## 4. Acceptance Criteria (REVISED)

- [ ] The slide is redesigned with the **two-column layout**.
- [ ] The **"Our Philosophy" text** explaining the benchmark shift is prominently visible.
- [ ] The **three images** are correctly placed with titles in the right-hand column gallery.
- [ ] **All inline styles are removed**.
- [ ] The `<style>` block is removed, and its content is integrated into `common.css`.