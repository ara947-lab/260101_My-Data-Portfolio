# 📊 My Data Analysis Portfolio  
**Lee Ara | Data Analyst**

> 이탈은 결과가 아니라 과정이며,  
> 분석의 역할은 이탈을 설명하는 것이 아니라  
> **‘언제 개입해야 하는가’를 앞당기는 것**이다.

운영 관점에서 실제로 실행 가능한  
**개입 시점을 정의하고, 의사결정으로 연결하는 데이터 분석**을 목표로 합니다.

---

## 🔗 Live Demo & Links

- 🌐 Interactive Portfolio (GitHub Pages)  
  👉 https://ara947-lab.github.io/260101_My-Data-Portfolio/
- 📈 Olist Seller Risk Dashboard (Streamlit)  
  👉 https://olist-analysis.streamlit.app/
- 🎮 TFT Analysis Dashboard (Streamlit)  
  👉 https://tft-dashboard.streamlit.app/

---

## 🧠 Projects Overview

### 1️⃣ Olist 이커머스 판매자 이탈 리스크 모니터링 (Advanced Project)

**한 줄 요약**  
> 초기 6개월 행동 데이터를 기반으로  
> *이탈 직전이 아닌, 개입 가능한 시점*을 식별하는 운영형 리스크 모니터링 시스템

#### 📌 문제 정의
- 1년 내 판매자 이탈률 **82% 이상**
- 기존 분석은 “왜 이탈했는가”에 머물러 있었음
- 운영에서 활용 가능한 **개입 시점 기준 부재**

#### 🔍 분석 접근
- 초기 6개월 주문/활동 패턴 기반 Feature Engineering
- 데이터 전처리 최적화로 **용량 98% 감소**
- 이탈 여부가 아닌 **회복 가능성 중심 Risk Stage 정의**

#### 🧩 Risk Segmentation
| Stage | 기준 | 해석 |
|------|------|------|
| Recoverable | 주문 ≥ 4건 | 구조적 지원 시 회복 가능 |
| Low Active | 주문 2~3건 | 활동 약화 단계 |
| Almost Churn | 주문 ≤ 1건 | 이탈 임박 |

#### 📊 핵심 인사이트
- 리뷰 평점은 원인이 아니라 **결과**
- **배송 지연 4일 초과 시** 긍정 리뷰 비율 급락
- 이탈은 갑작스러운 이벤트가 아닌 **행동 감소의 누적 결과**

#### 🛠 활용 관점 (Operational View)
- Risk Stage별 **Seller ID 리스트 직접 매핑**
- 즉시 개입 대상 명확화 (알림, 쿠폰, 가이드 발송)

#### 🧪 성과 지표
- 데이터 용량 감소: **98%**
- 모델 Recall: **86%**
- 운영 적용 가능 대상 명확화

#### 🛠 Tech Stack
`Python · Pandas · Streamlit · Chart.js`

---

### 2️⃣ TFT 시즌3 메타 변동성 및 조합 승률 분석 (Basic Project)

**한 줄 요약**  
> 시너지보다 **챔피언 단일 파워가 메타를 지배하는 구조적 문제**를 데이터로 검증한 분석

#### 📌 분석 목적
- “이 조합이 센 이유”를 감각이 아닌 데이터로 설명
- 픽률·승률·Top4 비율 기반 메타 구조 해석

#### 🔍 분석 결과
- 상위 조합의 **70~80%가 특정 챔피언(케일, 피즈, 카이사 등)에 집중**
- 시너지 효과보다 **스킬 계수·구조가 승률을 좌우**
- 저픽 고승 챔피언(숨은 OP) 식별

#### 🛠 Data-driven Balance Proposal
- Miss Fortune: 광역 스킬 계수 하향 제안
- Chrono: 1단계 공격속도 증가폭 완화
- Star Guardian: 시너지 요구치 완화 제안

#### 🛠 Tech Stack
`Python · Pandas · Visualization · Streamlit`

---

## 📁 Repository Structure

📦 260101_My-Data-Portfolio
┣ 📂 olist_dashboard # Olist 판매자 이탈 분석 코드
┣ 📂 tft_analysis # TFT 메타 분석 코드
┣ 📜 index.html # 인터랙티브 포트폴리오 메인 페이지
┗ 📜 README.md
