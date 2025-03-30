# 👩🏻‍⚖️ SK Networks AI CAMP 9기 - 3rd 1Team: LawQuick
- **주제:** LLM을 연동한 내외부 문서 기반 질의 응답 시스템
- **개발 기간:** 2025.03.28 ~ 2025.03.31
---
# 📌 목차

<details>
<summary>목차 내용</summary>

### 1. [팀 소개](#0️⃣-팀-소개)  
### 2. [프로젝트 개요](#1️⃣-프로젝트-개요)  
### 3. [기술 스택](#2️⃣-기술-스택)  
### 4. [시스템 아키텍처](#3️⃣-시스템-아키텍쳐)  
### 5. [WBS](#4️⃣-wbs)  
### 6. [요구사항 명세서](#5️⃣-요구사항-명세서)  
### 7. [수집한 데이터 및 전처리 요약](#6️⃣-수집한-데이터-및-전처리-요약)  
### 8. [DB 연동 구현 코드](#7️⃣-db-연동-구현-코드)  
### 9. [모델 선정 이유](#8️⃣-모델-선정-이유)  
### 10. [테스트 계획 및 결과 보고서](#9️⃣-테스트-계획-및-결과-보고서)  
### 11. [진행 과정 중 프로젝트 개선 노력](#🔟-진행-과정-중-프로젝트-개선-노력)  
### 12. [수행 결과](#*️⃣-수행-결과)  
### 13. [한 줄 회고](#✳️-한-줄-회고)  

</details>

----
# 0️⃣ **팀 소개**
## ✅ **팀명: LawQuick**
- 가족법 문제 해결의 가장 빠른 길
- 빠르게, 정확하게, 따뜻하게 가족법 문제 해결

<br>

## ✅ **팀원 소개**

| [@김하늘](https://github.com/nini12091)                      | [@박유진](https://github.com/YUJINDL01)                       |  [@박주은](https://github.com/pprain1999)                       | [@유지은](https://github.com/yujitaeng)                       |
|---------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|
| <img src="https://github.com/user-attachments/assets/e7dd2863-b577-4385-a46c-7163efb0bfe4" width="200" height="200">         | <img src="https://github.com/user-attachments/assets/c8ce1260-d6ca-4659-89c3-5d9f06847812" width="200" height="200" />| <img src="image/yoonjae.png" width="200" height="200">             |  <img src="https://github.com/user-attachments/assets/7fdacbe3-b568-4c42-8758-d189ec522bc3" width="200" height="200" />|

<br>

----
# 1️⃣ **프로젝트 개요**
## ✅ **프로젝트 명: LawQuick**
## ✅ **프로젝트 소개: 이혼 특화 AI 법률 상담 챗봇**

**LawQuick**은 이혼 분쟁을 겪는 사용자들이 법률 정보를 통해 자신의 상황을 이해하고 조언을 얻을 수 있도록 돕는 **AI 기반 가족법 상담 챗봇**

## ✅ **프로젝트 필요성**


### 📈 나홀로 소송 증가
![image (5)](https://github.com/user-attachments/assets/9278a929-ee80-4aa8-b479-7b1c45dd8b75)

![image (6)](https://github.com/user-attachments/assets/5c91008a-dcb5-4d09-a6f6-0404a3573b4f)

출처: [https://www.mk.co.kr/news/society/9878764](https://www.mk.co.kr/news/society/9878764)

- 제대로 된 법률 서비스를 이용하려면 **높은 비용 부담**이 존재함
- 비용 문제로 법률 전문가의 도움 없이 소송을 진행하는 **'나홀로 소송'** 사례 증가

### 📚 법률 해석의 어려움

- 정보는 많지만, **자신의 사례에 어떤 법이 적용되는지 알기 어려움**
- 판례나 조항의 해석이 어려워 **일반인의 이해에는 한계**

### 💸 상담 비용과 대응 계획 수립의 장벽

- **초기 상담 비용**으로 인해 아예 접근조차 하지 못하는 사례 존재
- 전문가와의 상담이 필요한 시점 판단 어려움

## ✅ **프로젝트 목표**

1. **법률 정보의 접근성 향상**
    
    → 복잡한 법률 용어를 **쉽고 간결한 Q&A 형식의 정보 제공**
    
2. **개인화된 법률 조언 제공**
    
    → 단순 정보 나열이 아닌, **사용자 상황을 반영한 맞춤형 상담 응답**
    
3. **법률 서비스 진입장벽 완화**
    
    → **비용 부담 없이 초기 상담을 제공**하고, 사용자의 법적 고민을 가볍게 나눌 수 있는 창구 제공
    
4. **심리적 안정감 제공**
    
    → 법률 문제를 **다른 사람에게 말하기 어려운 상황에서도, 익명성과 편안함 속에서 자신의 상황을 털어놓을 수 있는 공간 제공**

<br>

----

# 2️⃣ **기술 스택**
<br>

| 카테고리 | 기술 스택 |
|----------|-------------------------------------------|
| **사용 언어** | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white) |
| **LLM** | ![OpenChat](https://img.shields.io/badge/OpenChat-FFB000?style=for-the-badge&logo=OpenAI&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-005F73?style=for-the-badge&logo=Chainlink&logoColor=white) |
| **벡터 데이터베이스** | ![FAISS](https://img.shields.io/badge/FAISS-009688?style=for-the-badge&logo=Apache&logoColor=white) |
| **임베딩 모델** | ![OpenAI Embeddings](https://img.shields.io/badge/OpenAI%20Embeddings-8C9E90?style=for-the-badge&logo=OpenAI&logoColor=white) |
| **실행 환경** | ![RunPod](https://img.shields.io/badge/RunPod-FF4500?style=for-the-badge&logo=Render&logoColor=white) |
| **모델 튜닝/학습 프레임워크** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white) ![Transformers](https://img.shields.io/badge/Transformers-FFCC00?style=for-the-badge&logo=HuggingFace&logoColor=black) ![LoRA](https://img.shields.io/badge/LoRA-F76D57?style=for-the-badge&logo=HuggingFace&logoColor=white) |
| **인터페이스(UI)** | ![Gradio](https://img.shields.io/badge/Gradio-20B673?style=for-the-badge&logo=Gradio&logoColor=white) |
| **형상 관리 및 협업** | ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white) ![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=Google%20Drive&logoColor=white) |


<br>

----

# 3️⃣ **시스템 아키텍쳐**
## **✅ 시스템 아키텍쳐**
![시스템플로우](https://github.com/user-attachments/assets/ee51656a-52aa-40d4-bdb2-cd75248111ae)

## **✅ 시스템 플로우**
![시스템아키텍처](https://github.com/user-attachments/assets/fcbd8bc8-1102-4568-8008-39fc45cf8b51)

<br>

----

# 4️⃣ **WBS**
프로젝트 기간: 2025-03-18 ~ 2025-03-31
![스크린샷 2025-03-28 172115](https://github.com/user-attachments/assets/38893b7d-fcdf-4a7e-b4ed-ebbcec791a12)

<br>

----

# 5️⃣ **요구사항 명세서**

![image (1)](https://github.com/user-attachments/assets/a28fb2c7-aa58-4d99-bd0a-0c0f1c6cda3f)

<br>

----
# 6️⃣ 수집한 데이터 및 전처리 요약

## ✅ **판례 데이터**

- **출처**: 국가법령정보센터 Open API
- **수집 방식**: “이혼” 관련 키워드 약 60여 개를 활용하여 다양한 이혼 사례에 대한 판례 크롤링
- **전처리 과정**:
    - `판례내용`이 없는 항목 제거
    - 구조가 깨졌거나 필드 누락된 항목 필터링
    - 중첩 필드(`판례내용`) 구조 정리 및 일관화
    - 한국어 불용어 처리
- **최종 확보량**: **5,549건**

### 📦 판례 데이터 구조

| 필드명 | 설명 | 데이터 타입 |
| --- | --- | --- |
| 판례일련번호 | 판례 고유 식별자 | `string` |
| 사건명 | 사건의 명칭 | `string` |
| 사건번호 | 법원 사건 번호 | `string` |
| 선고일자 | 판결 선고 일자  | `string` |
| 법원명 | 판결을 내린 법원 | `string` |
| 사건종류명 | 사건 유형 (형사, 민사 등) | `string` |
| 사건종류코드 | 사건 종류 코드 | `string` |
| 판결유형 | 판결 방식 (판결, 결정 등) | `string` |
| 선고 | 선고 여부 | `string` |
| 판시사항 | 판결에서 다룬 주요 쟁점 | `string` |
| 판결요지 | 판결 요약 | `string`  |
| 참조조문 | 인용된 법 조문 | `string` |
| 참조판례 | 인용된 판례 | `string` |
| 판례내용 | 판결 상세 정보  | `object` |

### 🔹 판례내용 하위 필드

| 하위 필드명 | 설명 | 데이터 타입 |
| --- | --- | --- |
| 피고인 | 피고인 정보 | `string` |
| 상고인 | 상고 제기자 정보 | `string` |
| 변호인 | 변호인 이름 및 소속 | `string` |
| 원심판결 | 원심 판결 내용 | `string` |
| 주문 | 대법원의 판결 결과 | `string` |
| 이유 | 판결 이유 설명 | `string` |

## ✅ **법률 데이터**

- **출처**: [국가법령정보센터](https://www.law.go.kr/) PDF 문서
- **수집 방식**: “이혼” 관련 법률 PDF 수집 → 텍스트 추출 → JSON 구조화
- **전처리 과정**:
    - 조항을 `조항번호`, `조항제목`, `조항내용`으로 분리
    - 본문 내 항목(①②③…)을 자동으로 `제1항`, `제2항` 등으로 구조화
    - 한글 불용어 처리
- **최종 확보량**: **70개 법률 / 5,819개 조항**

### 📚 법률 데이터 구조

| 필드명 | 설명 | 데이터 타입 |
| --- | --- | --- |
| 법률명 | 해당 조항이 속한 법률명 | `string` |
| 조항번호 | 조문 번호 | `string` |
| 조항제목 | 조문 제목 또는 주제 | `string` |
| 조항내용 | 각 항의 조문 내용 | `object` |

### 🔸 조항내용 하위 구조

| Key | 설명 | 데이터 타입 |
| --- | --- | --- |
| 조항 번호 | 조항의 각 항 내용 | `string` |

## ✅ **파인튜닝 학습용 Q&A 데이터**

- **목적**: 법률 문서 기반 챗봇을 학습시키기 위한 질의응답 데이터 자동 생성

- **데이터 생성 방식**:
  * 판례 및 법령 문서를 **내용 단위로 분할(chunking)**  
    → 한 문서가 너무 길 경우, 500자 내외로 잘라서 다루기 쉽게 처리    
  * 각 chunk 내용을 바탕으로 자연어 질문 3개 자동 생성 (LLM 사용)  
  * 생성된 질문에 대해 RAG 기반으로 문서 검색 및 응답 생성  
  * `instruction`, `input`, `output` 형식으로 정리하여 저장

- **데이터 구조**:

| 항목 | 설명 |
|------|------|
| `instruction` | 문서 기반으로 생성된 질문 |
| `input` | 질문과 관련된 문서 내용 (RAG 검색 결과) |
| `output` | 질문에 대한 GPT 응답 결과 |

- **최종 확보량**: 총 **200개 질의응답 쌍**
----
# 7️⃣ **DB 연동 구현 코드**

**➡️ DB 연동 구현 코드(링크)** <br>
**➡️ [fine tuning 모델](https://huggingface.co/skyss/skn-3rd/tree/main)**

---

# 8️⃣ 모델 선정 이유

## 🧠 사용된 LLM: [`openchat/openchat-3.5-0106`](https://huggingface.co/openchat/openchat-3.5-0106)

OpenChat은 법률 상담과 같이 **정형화된 응답**, **근거 중심 추론**, **빠른 응답 시간**이 필요한 작업에 적합한 오픈소스 LLM임.

## ✅ **OpenChat의 특징과 장점**

* **C-RLFT 학습 방식**  
  → 명시적 선호 레이블 없이도 학습 가능 → 파인튜닝에 효율적임

* **경량화 구조**  
  → 추론 속도가 빠르고, 적은 자원으로 실행 가능함

* **출력 형식 제어 용이**  
  → 답변 포맷을 일관되게 유지할 수 있어 구조화된 응답에 적합함

* **문맥 반영 성능 우수**  
  → 검색 기반 문서(RAG)와 결합 시, 문맥을 안정적으로 활용함

* **오픈소스 접근 가능성**  
  → 커스터마이징 및 배포가 자유로움 (Apache 2.0 라이선스)

## 📌 선택 이유 요약

* 정형화된 법률 상담 포맷에 맞는 출력 제어가 쉬움  
* 추론 속도와 리소스 효율성이 뛰어남  
* 파인튜닝 및 실시간 응답 시스템 적용에 실용적임

## 📚 모델 정보

* **제작자**: Guan Wang et al.  
* **논문**: [OpenChat: Advancing Open-source Language Models with Mixed-Quality Data](https://arxiv.org/abs/2309.11235)  
* **라이선스**: Apache 2.0  
* **모델 페이지**: [HuggingFace 링크](https://huggingface.co/openchat/openchat-3.5-0106)

----

# 9️⃣ **테스트 계획 및 결과 보고서**

(결과 이미지)
<br>

(결과 해설)

일반 모델은 인 것에 비해~ 최종 모델은 ~~~하다 

지금 최종 모델은 몇 점인데 향후 ~를 한다면 어떻게 될 것인지 등등

<br>

----

# 🔟 **진행 과정 중 프로젝트 개선 노력**

## ✅ **1. 기능 개선**

- **질문 유형 자동 분류**  
  사용자의 질문을 *일반 상담 / 법령 조문 설명 / 판례 요약*으로 자동 분류하여 적절한 응답 포맷을 적용함

- **문서 기반 상담 제공**  
  단순한 답변이 아닌, 관련 법령·판례 원문을 함께 출력하여 신뢰도를 높임

- **문서 유사도 필터링 도입**  
  FAISS + OpenAI 임베딩 기반 유사도 필터링으로 무관한 문서 제거 및 의미 중심의 문서 검색 구현

- **하이브리드 응답 구조 적용**  
  파인튜닝 모델이 생성한 초안에 대해 GPT가 후처리하여 보다 명확하고 전문적인 답변 제공

## ✅ **2. 성능 최적화**

- **벡터 기반 문서 필터링 전환**  
  GPT 기반 필터링 대신 임베딩 유사도 필터링 적용 → 응답 속도 향상 및 리소스 절감

- **GPT 호출 최소화 전략 적용**  
  파인튜닝 모델의 응답 품질이 충분할 경우 GPT 보완 생략 → 처리 시간 및 API 비용 절감

- **QLoRA 기반 학습 효율화**  
  QLoRA + 4bit 양자화를 통해 학습 리소스를 줄이면서도 성능 저하 없이 파인튜닝 가능하도록 구성

## ✅ **3. 버그 및 품질 개선**

- **반복 또는 비논리 응답 자동 교체**  
  파인튜닝 모델 응답 중 반복 또는 이상 문장이 감지되면 GPT 단독 응답으로 자동 대체

- **함수 정의 오류 복구**  
  `extract_single_answer`, `filter_relevant_docs` 등 누락되거나 오류가 발생한 함수들을 신속히 재정의하여 안정성 확보

- **조문 설명 전략 제거 처리**  
  법률 조문 설명 응답에 전략적 조언이 포함되지 않도록 GPT 프롬프트를 명확히 설정

## ✅ **4. 사용자 경험 개선 (UI/UX)**

- **Gradio 기반 대화형 UI 구현**  
  별도 설치 없이 웹에서 바로 사용 가능한 직관적 인터페이스 구성

- **2열 사용자 정보 입력 폼 제공**  
  항목별 '비공개' 옵션을 포함하여 민감 정보를 보호하면서도 간편하게 입력 가능하도록 구성

- **응답 출처 시각화**  
  응답의 출처가 파인튜닝(🟢)인지 GPT 보완(🟠)인지 구분 가능하도록 시각적 표시 도입

- **대화 이력 유지 기능**  
  이전 질문 및 응답을 보존하여, 연속된 상담 흐름과 맥락을 자연스럽게 이어감

----

# *️⃣ **수행 결과**

![결과-화면-_1_ (1)](https://github.com/user-attachments/assets/26fbbda5-0928-479c-bb96-5e5daad506bb)

<br>

----

# ✳️ **한 줄 회고**

- ❤김하늘
   - <!-- 기입 -->
- 💜박유진
   - 파인튜닝 데이터를 직접 생성하면서, **모델이 학습 과정에서 '패턴'을 인식한다는 의미**는 단순한 문장 구조나 표현 방식뿐 아니라, **인풋과 아웃풋 등 필요한 정보가 항상 일정한 방식으로 제공되어야 한다는 것**임을 확실히 깨달을 수 있었습니다.
- 💙박주은
   - <!-- 기입 -->
- 💚유지은
   - 파인튜닝으로 모델의 정확성을 만들고 프롬프트로 그것을 더 세부적으로 조율을 할 수 있다는 것을 느꼈고 어느 하나도 빠져선 안될 중요한 부분들이라는 것을 깨달았습니다. LLM기반으로 사용자 케이스의 유사성을 따져가며 답변을 주는 모델을 만드는 과정이 험난했으나 과정을 익혀갈 수 있어 좋았습니다.

<br>
