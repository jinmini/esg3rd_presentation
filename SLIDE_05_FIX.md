# [PRD] New Slide 05: GRI Answer Engine Deep Dive

- **Document Version**: 1.0
- **Date**: 2023-10-27
- **Target Slide**: `05-gri-answer-engine.html` (New)
- **Action**: Create a new slide, replacing the previous "Solution Overview". All subsequent slides must be renumbered.

## 1. Goal & Strategic Purpose

The purpose of this new slide is to provide a **technical deep dive into our core AI technology**, the "GRI Answer Engine". It must move beyond a simple feature list and establish **deep technical credibility** with the audience.

The key messages to convey are:
1.  **We built a specialist AI, not a generic one.**
2.  **Our AI is trained on high-quality, relevant data.**
3.  **Our AI generates reports through a transparent and reliable process.**

## 2. Content & Data Requirements

This slide must accurately incorporate the following technical details.

### 2.1. The AI Model: "KoAlpaca-GRI"
- **Base Model**: `beomi/KoAlpaca-Polyglot-5.8B` (A powerful Korean-based model).
- **Fine-Tuning**: Utilized a proprietary dataset focused on GRI Standards.
- **Resulting Model**: `KoAlpaca-GRI`, a specialist model for ESG reporting.

### 2.2. The Benchmark & Philosophy
- Our model is benchmarked against the **energy 'utilization' strategies** of market leaders, not just 'production'.
- **Key Role Models**: Doosan Fuel Cell, Hyundai Motor (Hydrogen), LS ELECTRIC, Hanwha Energy, Bloom Energy. This shows our focus on advanced ESG topics like RE100, hydrogen economy, and VPP.

### 2.3. The 3-Step Generation Process
1.  **Structured Prompting**: Intelligently combines user data with GRI standards.
2.  **AI Draft Generation**: The `KoAlpaca-GRI` model generates a compliant draft.
3.  **Human-in-the-Loop**: The user reviews, edits, and provides final approval.

### 2.4. Training Results & Architecture (Critical Data)
This data should be presented visually, perhaps in a compact, professional-looking "Tech Spec" box.
- **Final Training Loss**: 0.0753
- **Best Eval Loss**: 0.2509
- **LoRA Adapter Size**: 28MB
- **Trainable Parameters**: ~1.2M
- **Key LoRA Config**: `r=16`, `lora_alpha=32`, `target_modules=query_key_value`
- **Key Takeaway**: "A lightweight yet powerful LoRA adapter was created, enabling the base model to be optimized for specific ESG tasks without retraining the entire 5.8B parameters."

## 3. Visual & Layout Requirements

### 3.1. Overall Structure
The slide should have a clear, hierarchical layout, likely a **two-part or three-part structure** to present the information without overwhelming the audience.

### 3.2. Key Visual Components
- **Component 1: The "AI Factory" Diagram**
  - A visual flow showing: `Base Model (polyglot-ko)` → `Fine-Tuning (GRI Dataset)` → `Specialist Model (KoAlpaca-GRI)`.
  - The "Fine-Tuning" step should be highlighted as our core intellectual property.

- **Component 2: The 3-Step Process Diagram**
  - Visually represent the "Prompting → AI Generation → Human Review" flow.

- **Component 3: The "Tech Spec" Box**
  - A clean, data-dense box to display the training results and architecture details from section 2.4. This adds a layer of technical proof.

### 3.3. Image Integration
- The slide must incorporate **three images** (1876x864px). Use placeholders for now.
  - **Image 1**: To be placed near the "AI Factory" diagram. It should visually represent the benchmark companies (e.g., a collage of their logos or representative technologies).
  - **Image 2**: To be placed next to the "Structured Prompting" step. It should visualize what a structured prompt looks like.
  - **Image 3**: To be placed next to the "AI Draft Generation" step. It should be a screenshot of an actual AI-generated report snippet.

## 4. Technical Implementation & Refactoring

- **New File Creation**: Create a new file named `05-gri-answer-engine.html`.
- **Renumbering**: All subsequent slides (`06`, `07`, etc.) must be renumbered (`07`, `08`, etc.). All navigation links and footer page numbers across the entire project must be updated to reflect the new slide count.
- **CSS Integration**: All custom CSS required for this new slide **must be integrated into `common.css`**. Create new, reusable component classes (e.g., `.tech-spec-box`, `.ai-factory-step`).
- **No Inline Styles or `<style>` tags**: The final HTML must be clean of all inline `style` attributes and `<style>` blocks.
- **JavaScript**: Any interactive elements (like hover effects) must have their logic placed in a `<script>` tag for now. This will be migrated to `common.js` in Phase 2.

## GRI 프레임워크에 맞는 모델 훈련 Data set

한국중부발전 사업 영역
1, 발전사업 --> 화력, 복합, 태양광, 풍력, 연료전지 등 발전소 운영
2. 신재생에너지 --> 태양광, 풍력, 연료전지, 수소혼소 등 확대 추진
3. 설비 운영/관리 --> 발전설비 정비, 고도화, 설비 투자, 유지 관리
4. 수출 사업 --> 해외 발전소 운영 및 O%M(운영/정비 서비스) 제공
데이터 셋 방향성
한국중부발전처럼 “신재생에너지를 생산만 하는 기업"이 아니라”이 아니라,  이제는 신재생에너지를 ‘어떻게 활용할지’에 집중하는 기업이 벤치마킹 타깃이 되어야 합니다.
이 관점에서 두산퓨얼셀, LS ELECTRIC, Bloom Energy, 현대차(수소 부문) 등은 활용 중심 ESG 전략’ 모델 구축과 보고서 구성의 롤모델이 될 수 있습니다.
두산퓨얼셀(연료전지 기반 분산형 발전 및 수소경제 핵심 기술)
2. 현대자동차(수소차 생산 외에도 **수소 저장·이송·활용 에너지 전환체계 구축 중)
“RE100 + 수소 활용” ESG 보고서에 반영
3. LS ELECTRIC (스마트그리드, 에너지저장장치(ESS), VPP(가상발전소) 기술 개발 )
중소기업/건물/도시단위 에너지 활용 최적화 시스템 
GRI 기준에서 Scope 3, 고객 가치 확장 중심
4. 한화에너지 ( 자체 태양광 발전 + 에너지저장장치(ESS) + 데이터 기반 운영)
전력 생산 → 저장 → 수요지 공급까지 일괄 운영
5. Bloom Energy (고체산화물연료전지 글로벌 선두 in 미국)
분산형 전력 + 수소 전환 솔루션 중심 보고서 구조 
 ESG 관점에서 활용 지표 명확

## 최종 훈련 결과

훈련 환료 상태: 완료됨
총 훈련 스텝: 7,602 스텝
훈련 에포크: 3 에포크
최고 성능 지표: 0.2509765625(eval_loss)
최종 손실: 0.0753(훈련 손실)
모델 아키텍쳐
모델 : "beomi/KoAlpaca-Polyglot-5.8B"
vram: 최소 6기가 필요
숨겨진 레이어 크기: 4,096
어텐션 헤드: 16개
숨겨진 레이어:28개
최대 위치 임베딩:2,048
어휘 크기:30,080
LoRA 어댑터 결과물
어댑터 크기:28MB
LoRA설정
r:16(랭크)
lora_alpha:32
lora_dropout:0.05
타겟 모듈: query_key_value
훈련 가능한 파라미터: 약 1.2M개
훈련 진행 과정
1에포크: 손실 9.8984 -->0.2605(eval_loss: 0.2509765625)
2에포크: 손실 0.1598(eval_loss:0.258544921875)
3에포크:: 손실 0.0753(eval_loss:0.3056640625)
한국어와 다국어 처리를 위한 LoRA 어댑터가 생성되었고, 최종 모델은 원본 KoAlpaca-Polyglot-5.8B 모델에 LoRA 어댑터를 적용하여 특정 테스크에 최적호된 형태로 사용 가능