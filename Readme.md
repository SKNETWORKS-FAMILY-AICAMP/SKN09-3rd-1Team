# 👩🏻‍⚖️ SK Networks AI CAMP 9기 - 3rd 1Team: lawquick
- **개발 기간:** 2025.03.28 ~ 2025.03.31

---

# 📌 목차  
1. [팀 소개](#0️⃣-팀-소개)  
2. [프로젝트 개요](#1️⃣-프로젝트-개요)  
3. [기술 스택](#2️⃣-기술-스택)  
4. [시스템 아키텍처](#3️⃣-시스템-아키텍쳐)
5. [WBS](#4️⃣-wbs)  
6. [요구사항 명세서](#5️⃣-요구사항-명세서)  
7. [수집한 데이터 및 전처리 요약](#6️⃣-수집한-데이터-및-전처리-요약)
8. [DB 연동 구현 코드](#7️⃣-db-연동-구현-코드)
9. [모델 선정 이유](#8️⃣-모델-선정-이유)
10. [테스트 계획 및 결과 보고서](#9️⃣-테스트-계획-및-결과-보고서)
11. [진행 과정 중 프로젝트 개선 노력](#🔟-진행-과정-중-프로젝트-개선-노력)
12. [수행 결과](#*️⃣-수행-결과)
13. [한 줄 회고](#✳️-한-줄-회고)



<br>

----
# 0️⃣ **팀 소개**
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
# 1️⃣ **프로젝트 개요**
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

# 2️⃣ **기술 스택**
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

# 3️⃣ **시스템 아키텍쳐**

**시스템 플로우**
![image (4)](https://github.com/user-attachments/assets/59ce312d-b3fc-4e0a-aa96-b596cc64715b)


**시스템 아키텍쳐**
![image (3)](https://github.com/user-attachments/assets/03d1a3f3-1244-47e2-8fb5-aac3b7c88aa5)


<br>

----

# 4️⃣ **WBS**

![image (2)](https://github.com/user-attachments/assets/536ced4d-471e-4691-a8f8-13cbf73cc2b5)


<br>

----

# 5️⃣ **요구사항 명세서**


![image (1)](https://github.com/user-attachments/assets/a28fb2c7-aa58-4d99-bd0a-0c0f1c6cda3f)



<br>

----

# 6️⃣ **수집한 데이터 및 전처리 요약**
<!--  1. 어디서 무엇을 수집 했는 지
2. 어떤 방식으로 수집 했는 지
3. 어떤 것을 전처리 하였는 지
4. 데이터들을 어떻게 합쳤는 지 -->

## **1. RAG- 판례 데이터, 법률 데이터**

### 1-1 판례 데이터, 법률 데이터 수집

### **데이터 수집**

- **판례 데이터**

```python
# 이혼 관련 크롤링 키워드 
keywords = [
    "이혼 청구", "협의 이혼", "재판상 이혼", "이혼 소송", 
    "이혼 사유", "이혼 조정", "이혼 판결", "이혼 위자료", 
    "이혼 후 재산 분할", "이혼 관련 법률", "이혼 재산 분할", 
    "부부 공동재산", "특유재산 분리", "혼인 중 재산 형성 기여도", 
    "재산 분할 비율", "위자료와 재산 분할 차이", "퇴직금 재산 분할", 
    "부동산 재산 분할", "사업체 재산 분할", "채무 분할", "이혼 후 양육권", 
    "양육권 소송", "양육비 청구", "양육권 변경", "양육비 지급 의무", "친권자 변경", 
    "비양육 부모 면접교섭권", "양육비 미지급 제재", "아이 거주지 변경"
    "이혼", "배우자의 부정행위", "불륜으로 인한 이혼", "가정폭력 이혼", "배우자의 폭력", "경제적 폭력 (생활비 미지급)",
    "유책 배우자의 이혼 청구 가능 여부", "정신질환으로 인한 이혼", "배우자의 도박 중독", "배우자의 알코올 중독",
    "배우자의 마약 중독", "국제결혼 이혼", "외국인 배우자 이혼", "국내/해외 이혼 절차 차이", "다문화 가정 이혼",
    "국제 양육권 분쟁", "외국인 배우자 강제 출국", "혼인 무효 및 취소", "혼인 무효 소송", "강제 결혼 취소",
    "허위 혼인신고 취소", "근친혼 이혼", "배우자의 이중결혼(중혼)", "속임수 결혼(사기 혼인)", "미성년자 혼인 무효",
    "이혼 후 성 변경", "이혼 후 재혼 문제", "이혼 후 재산 명의 변경", "이혼 후 아이 성 변경",
    "이혼 후 양육비 지급 분쟁", "이혼 후 부모 면접권", "이혼 후 주거 문제"
]
```

국가법령정보센터(https://www.law.go.kr/) OPENAPI 이용해 “이혼” 관련 키워드로 판례 데이터 크롤링 진행 

- **법률 데이터**

```python
# pdf 파일 json 형식으로 전처리하여 저장
def save_as_json(all_texts, output_dir):
    """
    모든 PDF 내용을 하나의 JSON 파일로 저장
    {'파일 이름': 텍스트 내용} 형식
    """
    json_path = os.path.join(output_dir, 'law_data.json')
    
    with open(json_path, 'w', encoding='utf-8') as f:
        json.dump(all_texts, f, ensure_ascii=False, indent=2)
    
    return json_path
```

국가법령정보센터(https://www.law.go.kr/) 에서 “이혼” 으로 검색된 법률 데이터 (pdf 문서) 크롤링 진행 

## 1-2 RAG용 데이터로 가공(전처리)

- **판례 데이터**

```python
import json

# 1. JSON 파일 열기
with open("./data/filtered_case_data.json", "r", encoding="utf-8") as f:
    data = json.load(f)

# 2. 판례내용이 비어있는 항목과 비어있지 않은 항목 나누기
non_empty_case_contents = [case for case in data if case.get("판례내용")]

# 3. 새 파일로 저장
with open("./data/filtered_case_data_non_empty.json", "w", encoding="utf-8") as f:
    json.dump(non_empty_case_contents, f, ensure_ascii=False, indent=2)

# 4. 확인 출력
print(f"전체 판례 수: {len(data)}")
print(f"판례내용이 비어있지 않은 항목 수: {len(non_empty_case_contents)}")
print("✅ filtered_case_data_non_empty.json 파일 저장 완료!")
```

```python
# 데이터 구조
[
  {
    "판례일련번호": "599601",
    "사건명": "정보통신망이용촉진및정보보호등에관한법률위반(정보통신망침해등)",
    "사건번호": "2021도5555",
    "선고일자": "2024-11-14",
    "법원명": "대법원",
    "사건종류명": "형사",
    "사건종류코드": "400102",
    "판결유형": "판결",
    "선고": "선고",
    "판시사항": "구 정보통신망 이용촉진 및 정보보호 등에 관한 법률 제48조 제1항에서 금지하는 (...) 판단하는 기준",
    "판결요지": "None",
    "참조조문": "구 정보통신망 이용촉진 및 정보보호 등에 관한 법률(2024. 1. 23. 법률 제20069호로 개정되기 전의 것) 제48조 제1항, 제71조 제1항 제9호(현행 제71조 제1항 제11호 참조)",
    "참조판례": "대법원 2005. 11. 25. 선고 2005도870 판결(공2006상, 71), 대법원 2021. 6. 24. 선고 2020도17860 판결",
    "판례내용": {
      "피고인": "피고인",
      "상고인": "검사",
      "변호인": "법무법인 서한 담당변호사 김건하 외 1인",
      "원심판결": "수원지법 2021. 4. 22. 선고 2020노4076 판결",
      "주문": "원심판결 중 무죄 부분을 파기하고, 이 부분 사건을 수원지방법원에 환송한다.",
      "이유": "상고이유를 판단한다.  (...) 주문과 같이 판결한다.대법관 이숙연(재판장) 이흥구 오석준(주심) 엄상필"
    }
  },
```

![스크린샷 2025-03-27 153413](https://github.com/user-attachments/assets/4aeefb9f-21d4-43f0-bd1e-a69d6e237413)


판례 내용이 비어있는 데이터들 제거.

- **법률 데이터**

```python
# 항목 분리 함수 정의
def split_articles(text):
    matches = list(re.finditer(r'(①|②|③|④|⑤|⑥|⑦|⑧|⑨|⑩)', text))
    if not matches:
        return {"제1항": text.strip()}

    result = {}
    for i in range(len(matches)):
        start = matches[i].start()
        end = matches[i + 1].start() if i + 1 < len(matches) else len(text)
        content = text[start + 1:end].strip()
        result[f"제{i + 1}항"] = content
    return result
```

```python
# 데이터 구조
{
    "가사소송법": [
        {
            "법률명": "가사소송법",
            "조항번호": "제1조",
            "조항제목": "목적",
            "조항내용": {
                "제1항": "이 법은 인격의 존엄과 남녀 평등을 기본으로 하고 가정의 평화 및 친족 간에 서로 돕는 미풍양속을 보존 하고 발전시키기 위하여 가사(家事)에 관한 소송(訴訟)과 비송(非訟) 및 조정(調停)에 대한 절차의 특례를 규정함을 목적으로 한다. [전문개정 2010. 3. 31.]"
            }
        },
        ...
}        
```

법률 조문별로 항목을 분할하여 저장.

![스크린샷 2025-03-28 101536](https://github.com/user-attachments/assets/658bfdf2-f925-45fd-8028-431f497d80f9)


# 2. 파인튜닝- 훈련용 Q&A 데이터


1. 판례/법률 기반 질의응답
   
    1. 구성
    
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
    

![스크린샷 2025-03-28 100406](https://github.com/user-attachments/assets/7a41dab6-50d0-46bf-9943-8d588cd5d0fe)

<br>

----
# 7️⃣ **DB 연동 구현 코드**

**➡️ DB 연동 구현 코드(링크)**


<br>

----
# 8️⃣ **모델 선정 이유**

### **사용된 LLM: openchat/openchat-3.5-0106**

**OpenChat 특징**

- C-RLFT 기법을 사용하여 학습되어 명시적인 선호 레이블 없이도 효과적으로 학습할 수 있도록 도움 (파인튜닝에 용이)
- 적은 매개변수로도 높은 성능을 제공

**법률 데이터셋에 대한 Fine-tuning**이 용이하며, 모델의 **경량화** 덕분에 **빠른 응답 시간**과 **높은 처리 성능**을 제공하는 OpenChat모델을 사용하여 **법률 상담 서비스의 효율성을 극대화하고, 복잡한 법률 문제에 대한 실시간 지원을 기대**

```
@article{wang2023openchat,
  title={OpenChat: Advancing Open-source Language Models with Mixed-Quality Data},
  author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang},
  journal={arXiv preprint arXiv:2309.11235},
  year={2023}
}
```

<br>

----




# 9️⃣ **테스트 계획 및 결과 보고서**

(결과 이미지)

(결과 해설)

일반 모델은 인 것에 비해~ 최종 모델은 ~~~하다 

지금 최종 모델은 몇 점인데 향후 ~를 한다면 어떻게 될 것인지 등등

<br>

----


# 🔟 **진행 과정 중 프로젝트 개선 노력**
<br>

----

# *️⃣ **수행 결과**

시연페이지 구성 화면 (스크롤 gif)
시연페이지 테스트 화면 캡처 이미지

<br>

----

# ✳️ **한 줄 회고**

- ❤김하늘
   - <!-- 기입 -->
- 💜박유진
   - 파인튜닝 데이터를 직접 생성하면서, **모델이 학습 과정에서 '패턴'을 인식한다는 의미**는 단순한 문장 구조나 표현 방식뿐 아니라, **정답과 필요한 정보가 항상 일정한 방식으로 제공되어야 한다는 것**임을 확실히 깨달을 수 있었습니다.
- 💙박주은
   - <!-- 기입 -->
- 💚유지은
   - <!-- 기입 -->


<br>

----
