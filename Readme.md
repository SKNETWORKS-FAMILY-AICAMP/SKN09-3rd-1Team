# 👩🏻‍⚖️ SK Networks AI CAMP 9기 - 3rd 1Team: lawquick
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
### 팀명: Lawquick
- "가족법 문제 해결의 가장 빠른 길 - Lawquick"
- 빠르게, 정확하게, 따뜻하게 가족법 문제 해결에 도움.

<br>

### 팀원 소개

| [@김하늘](https://github.com/nini12091)                      | [@박유진](https://github.com/YUJINDL01)                       |  [@박주은](https://github.com/pprain1999)                       | [@유지은](https://github.com/yujitaeng)                       |
|---------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|---------------------------------------------------------------------|
| <img src="image/jitaeng.png" width="200" height="200">         | <img src="https://github.com/user-attachments/assets/c8ce1260-d6ca-4659-89c3-5d9f06847812" width="200" height="200" />| <img src="image/yoonjae.png" width="200" height="200">             |  ![yujitaeng](https://github.com/user-attachments/assets/7fdacbe3-b568-4c42-8758-d189ec522bc3)  |



<br>

----
# 2️⃣ **프로젝트 개요**
- **프로젝트 명**:  "lawquick"
- **프로젝트 소개**:
    
    "lawquick"는 이혼과 양육권 문제에 직면한 사람들이 법적 절차를 이해하고, 적절한 대응 전략을 수립할 수 있도록 돕는 **AI 기반 법률 상담 서비스**입니다. 이 서비스는 이혼 절차, 재산 분할, 양육권 및 양육비 청구 등 법적 문제를 다루며, AI는 사용자의 상황을 분석하여 맞춤형 법률 조언, 법적 대응 전략을 제시합니다. 또한, 이혼 소송과 양육권 분쟁에 관한 다양한 판례와 법률을 기반으로 사용자가 이해하기 쉬운 방식으로 정보를 제공합니다.
    
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
1. 판례/법률 기반 질의응답
    a. 구성
    
    | 항목 | 설명 |
    | --- | --- |
    | instruction | 사용자의 질문 또는 요청 |
    | input | 사용자의 질문을 바탕으로 검색된 관련 정보 (벡터 DB 결과) + 사용자 정보 |
    | output | instruction 과 input 을 바탕으로 생성된 모델의 최종 답변 |
    - 총 900개의 데이터쌍
    
    b. 생성방법
    
    - input-사용자 정보 생성
    
    ```python
    def generate_random_profiles(n=300):
        marital_statuses = ["기혼", "이혼", "별거", "사실혼"]
        divorce_stages = ["이혼 고려 중", "이혼 준비 중", "이혼 진행 중", "이미 이혼함"]
        property_ranges = ["1천만 원 미만", "1천만~5천만 원", "5천만~1억 원", "1억~5억 원", "5억 이상"]
        abuse_history = ["없음", "있음"]
    
        def generate_children():
            if random.random() < 0.2:
                return "비공개"
            num_children = random.randint(0, 5)
            if num_children == 0:
                return "없음"
            ages = sorted(random.sample(range(0, 41), num_children))
            age_str = ", ".join(f"{age}세" for age in ages)
            return f"{num_children}명 ({age_str})"
    
        profiles = []
        for _ in range(n):
            marriage_duration = str(random.randint(0, 50)) + "년" if random.random() > 0.2 else "비공개"
    
            profile = {
                "혼인 상태": random.choice(marital_statuses) if random.random() > 0.2 else "비공개",
                "혼인 기간": marriage_duration,
                "이혼 단계": random.choice(divorce_stages) if random.random() > 0.2 else "비공개",
                "자녀": generate_children(),
                "재산": random.choice(property_ranges) if random.random() > 0.2 else "비공개",
                "폭력": random.choice(abuse_history) if random.random() > 0.2 else "비공개"
            }
            profiles.append(profile)
        return profiles
    ```
    
    - instruction 생성
    
    ```python
    question_prompt = PromptTemplate.from_template("""
    당신은 이혼 전문 AI 상담사에게 조언을 구하고 싶은 일반 사용자입니다. 아래 사용자 상황은 현실에서 마주칠 수 있는 다양한 이혼 사례 중 하나입니다. 이 상황을 바탕으로 **현실적이고 구체적인 법률 상담 질문**을 3개 작성해 주세요.
    
    ※ 질문은 사용자가 직접 AI 상담사에게 하는 말투로 작성하며, 다음과 같은 다양한 주제를 포함할 수 있습니다:
    - 자녀 양육권 분쟁, 양육비 문제
    - 배우자의 외도, 폭력, 도박, 정신질환 등 이혼 사유
    - 사실혼, 동거, 재혼, 국제결혼, 동성혼 등 다양한 혼인 형태
    - 재산 분할, 위자료, 부동산 명의, 퇴직금, 연금, 채무
    - 이혼 절차, 협의이혼 vs 재판상 이혼
    - 이혼 후의 생활 안정, 주거권, 연금, 신혼부부 혜택
    - 법적 보호 제도(가정폭력, 임시 보호, 접근금지 등)
    - 황혼 이혼, 출산 직후 이혼, 단기간 혼인 후 이혼 등 다양한 이혼 시점과 그에 따른 법적 쟁점
    
    [사용자 상황]
    {profile}
    
    [질문]
    1.
    2.
    3.
    """)
    ```
    
    사용 모델: gpt-3.5-turbo
    
    - output 생성
    
    ```python
    structured_prompt = PromptTemplate.from_template("""
    당신은 가족법 전문 AI 상담사입니다. 아래 사용자 상황과 질문, 그리고 참고 문서를 바탕으로, **법적 근거가 명확하고 구조화된 상담 답변**을 작성해주세요.
    
    ※ 다음 사항을 반드시 지켜주세요:
    - 사용자 정보 중 '비공개'로 표시된 항목은 절대 활용하지 마세요.
    - 관련 법 조항이나 판례가 존재하지 않는다면 '해당 없음'으로 작성하되, 그 이유를 설명해 주세요.
    - 조언 항목은 단순한 일반론이 아니라, 사용자의 상황에 맞는 현실적이고 논리적인 설명과 전문적인 판단을 담아 주세요.
    - 사용자 입장에서 이해하기 쉽도록 핵심을 요약하고 구체적인 행동 제안도 포함해주세요.
    
    [사용자 상황]
    {profile}
    
    [질문]
    {question}
    
    [참고 문서 요약]
    {context}
    
    [답변 작성 형식]
    
    💬 답변:
    1️⃣ 관련 법 조항: (관련 조항이 있다면 조문 번호와 함께 간단한 설명 / 없다면 '해당 없음' + 이유 설명)
    
    2️⃣ 관련 판례 요약: (실제 존재하는 유사 판례의 번호 및 핵심 판시사항 / 없으면 '해당 없음' + 이유 설명)
    
    3️⃣ 사용자 상황에 맞춘 조언: (사용자의 상황을 고려한 법률적 분석, 판단 근거, 구체적 조언과 권장 행동 제시. 필요시 주의사항도 함께 안내)
    """)
    ```
    
    사용 모델: gpt-3.5-turbo

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
