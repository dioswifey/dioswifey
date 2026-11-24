## Sohyun Kim · 김소현

**AI/AX Engineer · AI Product Manager**

기획서 작성부터 시스템 최적화까지 다룰 수 있는 AI 엔지니어를 지향합니다.
LLM 오케스트레이션과 RAG 기반 에이전트를 설계·구현하고, PRD·TRD 문서로 개발 요구사항을 직접 정의합니다.

> I build LLM-orchestrated agents end to end — from PRD/TRD authoring through system optimization.

---

### Core Engineering
데이터 · 백엔드 · 머신러닝 · 딥러닝 · 웹 서비스 · 생성형 AI

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Featured Projects

### 🎯 [headhunterAI](https://github.com/dioswifey/headhunterAI) — 사내문서 기반 AI 면접 시스템

`LangGraph` `Ollama` `RAG` `FastAPI` `PostgreSQL` `Redis` `Chroma` `Docker`

그 회사의 **사내문서를 근거로** 면접 질문을 생성하고, 음성 면접을 진행하고, 평가 리포트까지 만듭니다.
핵심 난점은 "근거로는 쓰되 기밀은 새지 않아야 한다"였고, 마스킹 18규칙(데이터 층)과 생성 질문
검사 관문(출력 층)의 **2층 방어**로 풀었습니다.

- **컴파일 그래프 3개** — 질문 생성 / 면접 루프(checkpointer) / 평가. 에이전트 모듈 29개, Python 약 10k LOC
- **점수·합불은 LLM이 판정하지 않습니다** — 그래프 상태에 점수 필드를 아예 두지 않아 경계를 구조로 강제
- **품질을 수치로 관리했습니다** — 지표 M-31~M-44 정의, 하드 제약(대외비 누출) 0건, 평균 ≥4.0 **그리고**
  95% CI 하한 ≥3.7, 부트스트랩·Wilson 구간, 회귀 허용 폭까지 기준선으로 고정
- **지원자 데이터를 외부 API로 보내지 않습니다** — Ollama 자체 호스팅이 기본 경로
- 테스트 9개 + 품질 측정 스크립트 14개

### 📊 [Mercari-priceprediction](https://github.com/dioswifey/Mercari-priceprediction) — 중고거래 가격 예측

`scikit-learn` `LightGBM` `SciPy` `pandas`

148만 건의 상품 데이터에서 상품명·설명글·카테고리·브랜드로 판매가를 예측했습니다.
**RMSLE 0.49220 → 0.41778 (15.1% 개선).**

- **개선의 원천을 분리했습니다** — 인코딩 교체와 n-gram 확장이 섞여 있던 개선을 ablation으로 나눠,
  실제 기여가 인코딩 쪽임을 실측
- **FM-FTRL을 직접 구현했습니다** — `wordbatch` 설치가 불가능한 환경에서 FTRL-proximal + FM 2차항을
  NumPy/SciPy로 벡터화 구현, 합성 데이터 스모크 테스트 후 적용
- **leakage를 숨기지 않고 측정했습니다** — 영향이 미미함을 수치로 확인하고 근거를 문서에 기록
- 실패한 전략(단계적 잔차 LGBM)도 실패로 남겨 뒀습니다
- 노트북에 출력이 저장돼 있어 **실행 없이 GitHub에서 바로 결과를 볼 수 있습니다**

---

### AI & Automation
AI 애플리케이션 · 에이전트 설계 및 개발

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Chroma](https://img.shields.io/badge/Chroma-FF6F61?style=flat-square)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)

LLM 오케스트레이션 · RAG(검색증강생성) · Tool Calling · 프롬프트 엔지니어링
LLM 품질 평가(LLM-as-judge) · 데이터 처리·검색 · 서비스 개발 워크플로우 자동화

### Bilingual Competency
미국 뉴욕주립대 심리학 학사 · 경제학 부전공

영어로 적혀있는 최신 글로벌 AI 기술을 빠른 속도로 흡수하고 적용합니다.
해외 논문과 기술 문서를 빠른 시간 안에 검토·분석해 구현으로 연결합니다.

---

### Other Work

**내부 자산 운용 자동화** — 한국투자증권 API 연동 Trading Agent
시장 데이터 수집부터 주문 실행까지의 워크플로우 자동화

**보상형 미니게임 기획** — E-commerce 고객 참여 솔루션
마켓컬리 '마이컬리팜' 벤치마킹, 쿠폰 발현 로직 설계 및 구매 전환 구조 제안

---

### Currently

- 생성형 AI · 에이전트 시스템을 실제 비즈니스 문제에 적용하는 일에 집중하고 있습니다
- CFA Level I 응시 예정 (2027년 5월)

### Contact

[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:lsk99013@gmail.com)
