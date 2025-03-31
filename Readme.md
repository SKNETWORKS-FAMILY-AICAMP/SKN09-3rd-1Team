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

## ✅ **팀원 소개**

| [@김하늘](https://github.com/nini12091)                      | [@박유진](https://github.com/YUJINDL01)                       |  [@박주은](https://github.com/pprain1999)                       | [@유지은](https://github.com/yujitaeng)                       |
|---------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|
| <img src="https://github.com/user-attachments/assets/e7dd2863-b577-4385-a46c-7163efb0bfe4" width="200" height="200">         | <img src="https://github.com/user-attachments/assets/c8ce1260-d6ca-4659-89c3-5d9f06847812" width="200" height="200" />| <img src="https://github.com/user-attachments/assets/c80b5b8d-4a42-4ed1-950f-b0ea5b078f51" width="200" height="200">             |  <img src="https://github.com/user-attachments/assets/7fdacbe3-b568-4c42-8758-d189ec522bc3" width="200" height="200" />|

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

## ✅ **프로젝트 목표**

### 📈 **법률 정보의 접근성 향상**
    
* 복잡한 법률 용어를 **쉽고 간결한 Q&A 형식의 정보 제공**
    
### 👤 **개인화된 법률 조언 제공**
    
* 단순 정보 나열이 아닌, **사용자 상황을 반영한 맞춤형 상담 응답**
    
### 💸 **법률 서비스 진입장벽 완화**
    
* **비용 부담 없이 초기 상담을 제공**하고, 사용자의 법적 고민을 가볍게 나눌 수 있는 창구 제공
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
# 3️⃣ **시스템 아키텍처 및 처리 흐름**

## ✅ 시스템 아키텍처

LawQuick은 **RAG(Retrieval-Augmented Generation)** 기반 구조로 설계됨.  

📌 구성 요소  
- **FAISS 벡터 DB**: 의미 기반 문서 검색  
- **OpenChat 기반 파인튜닝 LLM**: 정형화된 응답 생성  
- **GPT 모델 (보조적 역할)**: 응답 품질 보완

![시스템 플로우](https://github.com/user-attachments/assets/ee51656a-52aa-40d4-bdb2-cd75248111ae)

## ✅ 시스템 플로우

📌 구성 요소  
1. **질문 입력**  
   사용자가 자연어로 질문을 입력

2. **문서 검색**  
   FAISS를 통해 의미 유사도가 높은 판례 및 법령 문서 검색

3. **프롬프트 구성**  
   검색된 문서와 질문을 결합하여 하나의 입력 프롬프트로 생성

4. **모델 응답 생성**  
   파인튜닝된 LLM이 구조화된 답변을 생성

5. **후처리 (선택적)**  
   응답 품질이 부족한 경우 GPT를 통해 보완

6. **학습 활용 (점선 영역)**  
   GPT가 생성한 고품질 응답은 추후 파인튜닝 데이터로 재활용 가능


![시스템 아키텍처](https://github.com/user-attachments/assets/fcbd8bc8-1102-4568-8008-39fc45cf8b51)

> **전체 구조 요약:**  
> 사용자 질문 → 문서 검색 → 프롬프트 구성 → 모델 응답 생성

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



## ✅ 문서 구성 및 벡터화

### 🧾 문서 결합 방식

- 하나의 문서에 **판례 내용 + 참조 조문**을 함께 연결하여 구성
- `LangChain`의 `Document` 형식으로 변환  
  → 사건번호, 선고일자, 사건명, 참조조문 등의 **메타데이터** 포함
- 각 문서는 실제 판례에서 **어떤 법률 조항이 적용되었는지**를 확인할 수 있는 구조로 설계



### ✂️ 문서 분할 및 벡터화

| 항목 | 설명 |
|------|------|
| 문서 분할 방식 | `RecursiveCharacterTextSplitter` 사용, **600자 기준**으로 분할 |
| 임베딩 모델 | `OpenAI text-embedding-3-large` |
| 벡터 DB | `FAISS` 기반 벡터 데이터베이스 생성 |
| 용도 | `RAG 기반 검색` 및 `파인튜닝 학습 데이터 생성`에 활용 |



### 📌 구조적 특징

- 단순 요약 문서가 아닌, **법률 적용 구조까지 포함된 통합 문서**
- 각 문서는 **사례 + 근거법령**을 함께 포함  
  → 질문자의 상황에 맞춰 **정확하고 신뢰도 높은 문맥 검색 가능**
- 그대로 **질의응답 학습 데이터(instruction-input-output)**로도 사용 가능



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

- [**📂 DB 연동 구현 코드 (Google Drive)**](https://drive.google.com/drive/folders/10jCckp9hGfIuIjyjUmA1QuvJqft6pvbR)
- [**🧠 파인튜닝 모델 (Hugging Face)**](https://huggingface.co/skyss/skn-3rd/tree/main)

## ✅ **DB 연동 구현 내용**

**구현 내용 요약**
* DB 연동 용으로 `Langchain`의 `Document` 개체로 변환된 판례+법령 데이터
* `RecursiveCharacterTextSplitter`를 활용해 600자를 기준으로 문서 분할(chunk)
* `OpenAI Embedding` 모델로 벡터화
* `FAISS` 기반 Vector DB로 저장하여 RAG 검색 시스템에 최종 연동

---

# 8️⃣ 모델 선정 이유

## 🧠 사용된 LLM: [`openchat/openchat-3.5-0106`](https://huggingface.co/openchat/openchat-3.5-0106)

## ✅ **모델 선정 기준**
* **정해진 출력 형식을 유지할 것**
* **적은 자원으로 빠른 응답이 가능할 것**
* **소량의 데이터로도 파인튜닝이 가능할 것**

OpenChat: 법률 상담과 같이 **정형화된 응답**, **근거 중심 추론**, **빠른 응답 시간**이 필요한 작업에 적합한 오픈소스 LLM.

## ✅ **OpenChat의 특징과 장점**

* **출력 형식 제어 용이**  
  → 답변 포맷을 일관되게 유지할 수 있어 구조화된 응답에 적합함

* **경량화 구조**  
  → 추론 속도가 빠르고, 적은 자원으로 실행 가능함
  
* **C-RLFT 학습 방식**  
  → 명시적 선호 레이블 없이도 학습 가능 → 파인튜닝에 효율적임


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
# 9️⃣ 테스트 계획 및 결과 보고서
[**👨‍🔬 테스트 계획 및 결과 보고서**](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN09-3rd-1Team/blob/main/test_result/%EB%AA%A8%EB%8D%B8%20%ED%8F%89%EA%B0%80%20%EB%B3%B4%EA%B3%A0%EC%84%9C.pdf)

## 🧪 평가 방식

모델 응답은 총 **30개 질문, 6개 항목, 100점 만점** 기준으로 평가함:

### ✅ LLM 기반 가사법 상담 응답 평가 기준

#### 📌 1. 응답 속도 (최대 10점)

#### 📌 2. 법적 근거 제공 (최대 30점)

**🔹 법 조항 제시 (최대 15점)**  

**🔹 판례 제시 (최대 15점)**  

#### 📌 3. 사용자 맞춤 조언 제공 (최대 25점)

#### 📌 4. 입력 반영 정확도 (최대 15점)

#### 📌 5. 출력 형식 일관성 (최대 10점)

#### 📌 6. 질문 품질 (최대 10점)


## 📊 테스트 결과

| 항목 | 결과 |
|------|------|
| 📎 평균 점수 | **86.9점** |
| 🎯 90점 이상 응답 비율 | **10%** |
| 🧠 응답 일관성 | 매우 높음 (같은 질문 반복에도 구조·논리 유지) |
| 📘 강점 | 위자료, 재산분할, 양육비 관련 강제집행 설명 |
| 🔁 모델 안정성 | 질문 다양성에도 출력 구조 안정적으로 유지 |

## ✅ 테스트 결론

- **📚 법적 근거 제공력**  
  : 민법 및 가사소송법 조문, 대법원 판례 등을 구조화하여 **정확하고 구체적으로 인용**함  
- **💡 사용자 맞춤형 조언**  
  : 질문자의 혼인 기간, 자녀 유무, 재산 상황 등 **입력 정보를 반영한 전략적 안내** 제공  
- **📋 응답 형식 일관성**  
  : `1️⃣ 법 조항 → 2️⃣ 판례 → 3️⃣ 해석 → 4️⃣ 조언`의 **단계형 구조 유지**, 시각적 가독성 우수  

또한 동일 질문에 대해 **논리 흐름과 정보 일관성을 유지**하며,  
실제 법률 상담 상황에서 요구되는 **명확성, 실용성, 신뢰성** 모두 충족
<br>

---

# 🔟 **진행 과정 중 프로젝트 개선 노력**

📌  **개선 전 문제점**

![image (7)](https://github.com/user-attachments/assets/11c26a95-07ad-4c80-8137-a06419d568e2)

- 응답의 형식이 구조화 되지 않음
- 제공되는 연관 판례의 관련성이 떨어짐
- 프롬프트 메세지가 응답에 그대로 출력되는 문제
- 법률적인 판단 근거가 부족해 신뢰성이 떨어짐
- 사용자가 요청한 법령, 판례를 제대로 인용하지 못함

## ✅ 1. 프롬프트 최적화

| 전략 | 설명 |
| --- | --- |
| 🧾 응답 형식 구조화 | `1️⃣ 법적 해석`, `2️⃣ 맞춤 전략` 등 고정된 섹션 구조로 일관성 확보 |
| 🧠 질문 유형별 포맷 분기 | 조문/판례 요약, 상황 상담 등 질문 목적에 따라 응답 형식 분리 |
| 🛡 이상 응답 제어 | 사건 요약 시 전략 미포함, 반복/비논리적 응답은 자동으로 GPT 전환 |
| 🔄 GPT 보완 로직 | 파인튜닝 응답이 미흡할 경우 GPT가 필요한 부분만 자연스럽게 보완 |
| 🔍 사례 기반 응답 유도 | GPT가 실제 판례·사례를 인용하도록 유도하여 신뢰도 향상 |

📌 예시 이미지

- 질문 유형별 답변 포맷 분리 후 법령 본문 제공 응답 예시
    
![image (8)](https://github.com/user-attachments/assets/d45bee98-2bbe-4ade-bcda-0406fc481349)

    
- 실제 판례를 인용하도록 유도한 뒤 판례 요약 응답 예시
    
![image (9)](https://github.com/user-attachments/assets/a7839b48-7f41-493f-9eb8-ef88dc867f8b)

    



## ✅ 2. 기능 개선

| 항목 | 설명 |
| --- | --- |
| 🔗 문서 유사도 필터링 | FAISS + Embedding 기반으로 질문과 무관한 문서 제거 |
| 🧠 하이브리드 응답 구조 | 파인튜닝 응답 초안 + GPT 보완을 통해 전문성 및 자연어 품질 확보 |



## ✅ 3. 성능 최적화

| 항목 | 설명 |
| --- | --- |
| 🚀 응답 속도 개선 | GPT 기반 필터링 → 벡터 유사도 기반 선필터링 구조로 병목 해소 |
| 💡 GPT 호출 최소화 | 파인튜닝 응답이 충분할 경우 GPT 호출 생략 → 속도 및 비용 최적화 |
| 🧠 QLoRA 경량 파인튜닝 | A40 환경에서 QLoRA + 4bit 압축 기반 저비용 고효율 튜닝 수행 |
| 📈 응답 품질 평가 | 조문 해설, 맞춤 전략, 상황 반영 등 기준으로 응답 품질 지속 개선 |



## ✅ 4. 시스템 안정화

| 항목 | 설명 |
| --- | --- |
| 🧼 반복/오류 응답 감지 | 반복되거나 부정확한 응답은 자동으로 후처리 로직 적용 |



## ✅ 5. 사용자 경험 개선 (UI/UX)

| 항목 | 설명 |
| --- | --- |
| 💬 Gradio 기반 대화 UI | 누구나 쉽게 이용 가능한 대화형 상담 시스템 구성 |
| 📝 사용자 정보 입력 폼 | 항목별 ‘비공개 처리’ 옵션 포함하여 정보 보호 및 입력 편의성 향상 |
| 🗂 채팅 히스토리 기반 응답 | 사용자 질문 흐름 유지 → 문맥 이해 기반 자연스러운 대화 제공 |

📌 예시 이미지

- 사용자 정보 입력
    
![image (10)](https://github.com/user-attachments/assets/350be3b4-0918-4e95-aab6-53398a481538)

    
- 채팅 흐름 개선
    
![image (11)](https://github.com/user-attachments/assets/3af4be5d-cbad-4ae2-8762-1b178ca471f9)

---

# *️⃣ **수행 결과**

### ✅ 최종 결과 GIF
![최종-결과-화면-gif](https://github.com/user-attachments/assets/0177453f-084d-4b77-b322-9f5cb51793f3)

<br>

### ✅ 사용자 화면
![사용자 화면](https://github.com/user-attachments/assets/548a31c0-dfe2-44be-b5bc-80bda8c0d4e2)



### ✅ 질의응답 화면
![결과 1(파인튜닝만)](https://github.com/user-attachments/assets/455e7bb4-24c0-4690-b401-9cb1de9a68a0)
![결과 2(파인튜닝만)](https://github.com/user-attachments/assets/d47a8ba0-1761-49a4-8a98-0ad77de4d07f)
![결과 3(파인튜닝만)](https://github.com/user-attachments/assets/64ba7522-8fc0-46e8-a000-4f8adb7a43f9)

<br>

---


# 🤖 결과 정리 및 향후 계획

## ✅ 프로젝트 요약
LawQuick은 이혼 및 가사법 상담에 특화된  
문서 기반 질의응답 시스템입니다. 핵심 구성은 다음과 같습니다.

- 실제 상담 사례와 법령 데이터를 활용한 도메인 특화 Q&A
- 정형화된 응답 포맷과 법적 근거 중심의 답변 설계, 사용자 입력 반영
- RAG 기반 문서 검색, LLM 파인튜닝 결합

## 🎯 기대 효과
- 법률 상담에서 요구되는 **정확성, 신뢰성, 실용성**을 갖춘 답변 제공
- **일반 사용자도 이해할 수 있는 구조화된 응답** 구현
- 실제 법률 서비스로의 **확장 가능성을 지닌 기술 구조 확보**


## 🔧 향후 개선 방향

| 항목 | 내용 |
|------|------|
| 🔄 법률 지식 확장 | 최신 법령 및 신규 판례 반영을 위한 지속적 데이터 업데이트 |
| ⚡ 응답 속도 최적화 | 실시간 상담 환경을 위한 처리 경량화 및 속도 개선 |
| 🎯 프롬프트 구조 개선 | 다양한 질문 유형 대응을 위한 템플릿 정교화 |
| 📥 사용자 피드백 반영 | 실제 사용자 경험을 반영한 응답 품질 보완 체계 도입 |


<br>

---

# ✳️ **한 줄 회고**

- ❤ 김하늘
   - 조문, 조언, 법률 정보가 구분되지 않거나 응답 형식이 일관되지 않는 문제가 발생해, 데이터를 항목별로 구조화하고 표현을 통일한 뒤 파인튜닝을 진행했습니다. 이후 출력 예시를 프롬프트에 포함시키는 방식으로 개선하면서 응답 품질이 안정되었고, 데이터 구성과 프롬프트 설계가 모델 성능에 결정적인 영향을 미친다는 점을 직접 경험할 수 있었습니다.
- 💜박유진
   - 파인튜닝 데이터를 직접 생성하면서, **모델이 학습 과정에서 '패턴'을 인식한다는 의미**는 단순한 문장 구조나 표현 방식뿐 아니라, **인풋과 아웃풋 등 필요한 정보가 항상 일정한 방식으로 제공되어야 한다는 것**임을 확실히 깨달을 수 있었습니다.
- 💙박주은
   - 이미 학습된 LLM을 특정 도메인에 맞춰 재학습하는 파인튜닝의 성능을 직접 일반 GPT 모델과 비교하며 확인함으로써 개념을 제대로 이해할 수 있었습니다. 또한, 파인튜닝 모델의 응답을 GPT로 후처리하는 하이브리드 응답 구조를 처음 접하고, 그 성능까지 확인할 수 있어 흥미로운 경험이었습니다.
- 💚유지은
   - 파인튜닝으로 모델의 정확성을 만들고 프롬프트로 그것을 더 세부적으로 조율을 할 수 있다는 것을 느꼈고 어느 하나도 빠져선 안될 중요한 부분들이라는 것을 깨달았습니다. LLM기반으로 사용자 케이스의 유사성을 따져가며 답변을 주는 모델을 만드는 과정이 험난했으나 과정을 익혀갈 수 있어 좋았습니다.

<br>
