# 👩🏻‍⚖️ SK Networks AI CAMP 9기 - 4th 1Team: LawQuick

- **주제:** AI 활용 애플리케이션 개발  
- **개발 기간:** 2025.04.21 ~ 2025.04.22  

---

## 📌 목차

<details>
<summary>목차 내용</summary>

### 01. 팀 소개  
### 02. 프로젝트 개요  
### 03. 기술 스택  
### 04. 시스템 구성도  
### 05. 요구사항 정의서 (캡처)  
### 06. 화면설계서 (캡처)  
### 07. WBS  
### 08. 테스트 계획 및 결과 보고서 (캡처)  
### 09. 수행결과(테스트/시연 페이지)  
### 10. 한 줄 회고  

</details>

---

## 01. 팀 소개

### ✅ 팀명: LawQuick  
가족법 문제 해결의 가장 빠른 길

### ✅ 팀원 소개

| [@김하늘](https://github.com/nini12091) | [@박유진](https://github.com/YUJINDL01) | [@박주은](https://github.com/pprain1999) | [@유지은](https://github.com/yujitaeng) |
|-----------------------------------------|----------------------------------------|------------------------------------------|------------------------------------------|
| <img src="https://github.com/user-attachments/assets/e7dd2863-b577-4385-a46c-7163efb0bfe4" width="200" height="200"> | <img src="https://github.com/user-attachments/assets/c8ce1260-d6ca-4659-89c3-5d9f06847812" width="200" height="200" /> | <img src="https://github.com/user-attachments/assets/c80b5b8d-4a42-4ed1-950f-b0ea5b078f51" width="200" height="200"> | <img src="https://github.com/user-attachments/assets/7fdacbe3-b568-4c42-8758-d189ec522bc3" width="200" height="200" /> |

---

## 02. 프로젝트 개요

### ✅ 프로젝트 명: LawQuick  
### ✅ 프로젝트 소개: 이혼 특화 AI 법률 상담 챗봇  

**LawQuick**은 이혼 분쟁을 겪는 사용자들이 법률 정보를 통해 자신의 상황을 이해하고 조언을 얻을 수 있도록 돕는 **AI 기반 가족법 상담 챗봇**입니다.

---

### ✅ 프로젝트 필요성

#### 📈 나홀로 소송 증가
![image (5)](https://github.com/user-attachments/assets/9278a929-ee80-4aa8-b479-7b1c45dd8b75)  
![image (6)](https://github.com/user-attachments/assets/5c91008a-dcb5-4d09-a6f6-0404a3573b4f)

출처: [https://www.mk.co.kr/news/society/9878764](https://www.mk.co.kr/news/society/9878764)

- 제대로 된 법률 서비스를 이용하려면 **높은 비용 부담**이 존재함  
- 비용 문제로 법률 전문가의 도움 없이 소송을 진행하는 **'나홀로 소송'** 사례 증가

#### 📚 법률 해석의 어려움

- 정보는 많지만, **자신의 사례에 어떤 법이 적용되는지 알기 어려움**  
- 판례나 조항의 해석이 어려워 **일반인의 이해에는 한계**

---

### ✅ 프로젝트 목표

#### 📈 법률 정보의 접근성 향상  
- 복잡한 법률 용어를 **쉽고 간결한 Q&A 형식의 정보 제공**

#### 👤 개인화된 법률 조언 제공  
- 단순 정보 나열이 아닌, **사용자 상황을 반영한 맞춤형 상담 응답**

#### 💸 법률 서비스 진입장벽 완화  
- **비용 부담 없이 초기 상담을 제공**하고, 사용자의 법적 고민을 가볍게 나눌 수 있는 창구 제공

---

## 03. 기술 스택

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

---

## 04. 시스템 구성도

> 시스템 아키텍처 및 데이터 흐름도 (예: 사용자 입력 → 벡터 검색 → LLM → 응답 반환)

![system-diagram](https://github.com/your-team/your-repo/assets/your-diagram-placeholder)

---

## 05. 요구사항 정의서

- 사용자 정보 입력, 상담 진행, 결과 제공 등 핵심 기능 요구사항 정리  
- REQ-LQ01 ~ REQ-LQ10 포함  
- 🖼️ 캡처 이미지 첨부 예정

---

## 06. 화면설계서

- info 페이지를 포함한 각 화면 별 와이어프레임 or 목업  
- 입력 UI, 상담 결과, 초기 화면 등  
- 🖼️ 캡처 이미지 첨부 예정

---

## 07. WBS (작업 분배표)

| 역할 | 팀원 | 담당 업무 |
|------|------|-----------|
| 데이터 수집/전처리 | 김하늘 | 판례/법령 수집, 파싱 |
| 벡터 DB 구축 | 박주은 | 임베딩 및 검색 구현 |
| 챗봇 개발 | 유지은 | Gradio UI, 응답 생성 |
| 프론트/폼 구현 | 박유진 | 사용자 입력 페이지, 유효성 검증 |

---

## 08. 테스트 계획 및 결과

- 주요 기능별 테스트 시나리오 작성  
- 정상 입력/비정상 입력 대응 여부 확인  
- 🖼️ 테스트 결과 캡처 포함 예정

---

## 09. 수행 결과

- 실제 구동 영상 or Gradio 시연 링크  
- 배포 환경 소개 및 사용 방법

---

## 10. 한 줄 회고

- ❤ **김하늘**  
  - 처음엔 막막했지만, 우리만의 결과물을 만든 경험이 소중했습니다.

- 💜 **박유진**  
  - 사용자 입장에서 고민하며 개발하는 것이 정말 중요하다는 걸 느꼈어요!

- 💙 **박주은**  
  - AI가 법률 서비스를 돕는 방법을 직접 구현하며 자신감이 생겼어요.

- 💚 **유지은**  
  - 팀원들과 협업하며 빠르게 MVP를 만드는 경험이 뜻깊었어요.

---
