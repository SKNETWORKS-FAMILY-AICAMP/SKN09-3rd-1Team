# 👩🏻‍⚖️ SK Networks AI CAMP 9기 - 3rd 1Team: ooo
- **개발 기간:** 2025.03.18 ~ 2025.03.31

---

# 📌 목차  
1. [팀 소개](#1️⃣-팀-소개)  
2. [프로젝트 개요](#2️⃣-프로젝트-개요)  
3. [기술 스택](#3️⃣-기술-스택)  
4. [시스템 아키텍처](#4️⃣-시스템-아키텍쳐)
5. [WBS](#5️⃣-wbs)  
6. [요구사항 명세서](#6️⃣-요구사항-명세서)  
7. [데이터 수집 및 처리](#7️⃣-데이터-수집-및-처리)  
8. [테스트 계획 및 결과 보고서](#8️⃣-테스트-계획-및-결과-보고서)  
9. [진행 과정 중 프로젝트 개선 노력](#9️⃣-진행-과정-중-프로젝트-개선-노력)  
10. [수행 결과](#🔟-수행-결과)
11. [한 줄 회고](#*️⃣-한-줄-회고)


<br>

----

# 1️⃣ **팀 소개**
### 팀명, '근육빵빵'이란?
- "근육 빵빵, 회원 이탈률 00명"
- **'헬스장 회원 이탈률 00명으로 만들고, 유지중인 회원들에게 근육을 빵빵하게 만들겠다'** 는 중의적인 의미를 담고 있습니다.

<br>

### 팀원 소개

| [@김하늘](https://github.com/nini12091)                      | [@박주은](https://github.com/pprain1999)                       | [@박유진](https://github.com/YUJINDL01)                       | [@유지은](https://github.com/yujitaeng)                       |
|---------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|
| <img src="image/jitaeng.png" width="200" height="200">         | <img src="image/gwangwoon.png" width="200" height="200">            | <img src="image/yoonjae.png" width="200" height="200">             |  ![yujitaeng](https://github.com/user-attachments/assets/7fdacbe3-b568-4c42-8758-d189ec522bc3)  |



<br>

----
# 2️⃣ **프로젝트 개요**
- **프로젝트 명**:  "___"
- **프로젝트 소개**:
    
    " ___"는 이혼과 양육권 문제에 직면한 사람들이 법적 절차를 이해하고, 적절한 대응 전략을 수립할 수 있도록 돕는 **AI 기반 법률 상담 서비스**입니다. 이 서비스는 이혼 절차, 재산 분할, 양육권 및 양육비 청구 등 법적 문제를 다루며, AI는 사용자의 상황을 분석하여 맞춤형 법률 조언, 법적 대응 전략을 제시합니다. 또한, 이혼 소송과 양육권 분쟁에 관한 다양한 판례와 법률을 기반으로 사용자가 이해하기 쉬운 방식으로 정보를 제공합니다.
    
- **프로젝트 필요성(배경)**:
    
    이혼 및 양육권 문제는 **법적, 감정적, 재정적 요소가 복잡하게 얽혀 있어** 일반인이 법률 절차를 이해하고 대응하는 데 어려움을 겪는 경우가 많습니다.
    
    1. **법률 정보 접근성 부족**
        - 변호사를 직접 찾아 상담받기 어려운 경우가 많고, 인터넷상의 정보는 신뢰도가 낮거나 최신 법률을 반영하지 못할 수 있음.
    2. **개별 상황에 대한 맞춤형 조언 부족**
        - 동일한 법률 조항이라도 개별 사건에 따라 적용 방식이 달라질 수 있음.
        - 기존 검색 기반 서비스는 일반적인 정보를 제공할 뿐, 사용자의 구체적인 상황에 맞는 해결책을 제시하지 못함.
    3. **법률 상담 비용 부담**
        - 초기 상담만으로도 상당한 비용이 발생하며, 경제적 부담 때문에 법적 조치를 포기하는 사례가 많음.
    
    본 프로젝트는 **AI 기반 법률 Q&A 챗봇을 개발하여, 이러한 문제를 해결하고 보다 많은 사람들이 법적 조언을 받을 수 있도록 지원**하는 것을 목표로 합니다.
    
- **프로젝트 목표**:
    1. **이혼 및 양육권 관련 법률 Q&A 지원**: 이혼 및 양육권 문제에 대해 사용자가 법적 대응을 쉽게 이해하고 실행할 수 있도록 돕습니다.
    2. **맞춤형 법률 상담 제공**: 사용자의 구체적인 상황에 맞춘 상담을 통해, 이혼과 양육권 문제에 대한 최적의 대응책을 제공합니다.
    3. **법적 절차의 자동화 및 효율성 증대**: 이혼 및 양육권 분쟁에 있어 사용자들이 빠르고 효율적으로 법적 절차를 진행할 수 있도록 지원합니다.


<br>

----

# 3️⃣ **기술 스택**
<br>

| 카테고리 | 기술 스택 |
|----------|-------------------------------------------|
| **LLM 모델** | ![OpenChat](https://img.shields.io/badge/OpenChat-F4A300?style=for-the-badge&logo=OpenAI&logoColor=white) ![KoGPT2](https://img.shields.io/badge/KoGPT2-4C7FEF?style=for-the-badge&logo=Kakao&logoColor=white) ![Gemma](https://img.shields.io/badge/Gemma-1F99F2?style=for-the-badge&logo=HuggingFace&logoColor=white) |
| **백엔드** | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-005F73?style=for-the-badge&logo=LangChain&logoColor=white) |
| **데이터베이스** | ![FAISS](https://img.shields.io/badge/FAISS-009688?style=for-the-badge&logo=FAISS&logoColor=white) |
| **임베딩** | ![OpenAI Embeddings](https://img.shields.io/badge/OpenAI%20Embeddings-8C9E90?style=for-the-badge&logo=OpenAI&logoColor=white) |
| **클라우드 환경** | ![Runpod](https://img.shields.io/badge/RunPod-FF4500?style=for-the-badge&logo=RunPod&logoColor=white) |
| **딥러닝 프레임워크** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white) ![Hugging Face Transformers](https://img.shields.io/badge/Hugging%20Face%20Transformers-FFCC00?style=for-the-badge&logo=HuggingFace&logoColor=white) ![LoRA](https://img.shields.io/badge/LoRA-FF4500?style=for-the-badge&logo=HuggingFace&logoColor=white) |
| **협업 및 문서화** | ![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white) |
| **UI & 대시보드** | ![Gradio](https://img.shields.io/badge/Gradio-008000?style=for-the-badge&logo=Gradio&logoColor=white) |
| **형상 관리** | ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white) |


<br>

----

# 4️⃣ **시스템 아키텍쳐**



<br>

----

# 5️⃣ **WBS**



<br>

----

# 6️⃣ **요구사항 명세서**



<br>

----

# 7️⃣ **데이터 수집 및 처리**
<!--  1. 어디서 무엇을 수집 했는 지
2. 어떤 방식으로 수집 했는 지
3. 어떤 것을 전처리 하였는 지
4. 데이터들을 어떻게 합쳤는 지 -->


<br>

----

# 8️⃣ **테스트 계획 및 결과 보고서**
<!-- 기입 
- [참고 링크 1](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN08-3rd-2Team), [참고 링크 2](https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN08-3rd-1Team),
- **!!여기서 키포인트는 프로젝트 초반에 세운 가설을, 어떻게 발전하고 구현했는지 기입 필요!!!**
- 테스트 계획 및 결과 보고서 (캡쳐+git upload) / DB 연동 구현 코드 (링크만) -->

### 1. FAISS 전처리
<!-- 기입 -->

<br>

### 2. RAG
<!-- 기입 -->

<br>

### 3. langchain+FAISS필요한 이유
<!-- 기입 -->

<br>

### 4. 프롬프트 작성
<!-- 기입 -->

<br>

### 5. Fine-tuning
<!-- 기입 -->

<br>

### 5-1. 파인튜닝 필요성
<!-- 기입 -->

<br>

### 6. 출력 결과
<!-- 기입 | 모델 별 답변 비교 & 검증, 가설 검증 
     아래 이미지는 참고용! 다 기입하고 나선 지울 것!!  -->
![image2](https://github.com/user-attachments/assets/fa473d56-3f61-46c2-8754-485fac215f6d)


<br>

----

# 9️⃣ **진행 과정 중 프로젝트 개선 노력**
<!-- 기입 
1. **기능 개선**: 프로그램의 기능을 개선한 부분 (예: 사용자 피드백을 반영하여 기능 추가)
2. **성능 최적화**: 성능을 개선한 부분 (예: 데이터 처리 속도 개선, 서버 응답 시간 단축 등)
3. **버그 수정**: 발생한 버그를 어떻게 해결했는지, 수정한 과정
4. **사용자 경험 개선**: UI/UX 개선 내용 (예: 인터페이스 개선, 접근성 향상 등) -->


<br>

----

# 🔟 **수행 결과**

### 1. 메인페이지
<!-- 기입 -->

<br>

### 2. 사용자 입력 단계
<!-- 기입 -->

<br>

### 3. AI 봇 작동하는 모습
<!-- 기입 -->

<br>

### 4. 사용자 즉각 응답
<!-- 기입 -->

<br>

### 5. 최종 행동 GIF
<!-- 기입 -->

<br>

----

# *️⃣ **한 줄 회고**

- ❤김하늘
   - <!-- 기입 -->
- 💜박유진
   - <!-- 기입 -->
- 💙박주은
   - <!-- 기입 -->
- 💚유지은
   - <!-- 기입 -->


<br>

----
