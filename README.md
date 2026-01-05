# 📚 AI 독해력 트레이너 (Reading Comprehension Trainer)

OpenAI **GPT-4o-mini**를 활용하여 사용자 맞춤형 독해 퀴즈를 생성하고, 문해력을 과학적으로 훈련하는 **Streamlit** 웹 애플리케이션입니다.

## 🌟 주요 기능 (Features)

- **🔗 URL 자동 분석**: 뉴스 기사, 블로그 등 웹페이지 URL만 입력하면 본문을 자동으로 추출하여 분석합니다.
- **📝 맞춤형 퀴즈 생성**: 사용자가 선택한 난이도(초/중/고/성인)에 맞춰 5가지 유형의 독해 문항을 출제합니다.
  1. **주제 찾기**: 글의 핵심 요지를 파악하는 능력 훈련
  2. **어휘 선택**: 문맥에 맞는 적절한 어휘 판단
  3. **빈칸 추론**: 논리적 흐름과 접속사 파악
  4. **내용 일치**: 사실 관계(Fact Check) 확인
  5. **비교 분석**: 관련된 외부 지문과의 비교/대조 능력
- **📊 즉각적인 피드백**: 채점 결과와 함께 상세한 해설, 그리고 취약 유행에 따른 맞춤형 학습 조언을 제공합니다.

## 🛠 기술 스택 (Tech Stack)

- **Frontend**: Streamlit (Python)
- **AI/LLM**: OpenAI GPT-4o-mini API
- **Web Scraping**: Trafilatura
- **Deployment**: Streamlit Community Cloud

## 🚀 설치 및 실행 (Installation)

### 1. 환경 설정

`python-dotenv` 등 필수 라이브러리를 설치합니다.

```bash
pip install -r requirements.txt
```

### 2. API Key 설정

`.env.example` 파일을 복사하여 `.env` 파일을 생성하고, OpenAI API Key를 입력하세요.
(Streamlit Cloud 배포 시에는 `Secrets` 기능을 사용합니다.)

```bash
# .env 파일 예시
OPENAI_API_KEY=sk-your-openai-api-key-here
```

### 3. 앱 실행

```bash
streamlit run app.py
```

## 📂 프로젝트 구조 (Structure)

```
📦 smart-reading-trainer
 ┣ 📜 app.py              # 메인 애플리케이션 코드
 ┣ 📜 requirements.txt    # 의존성 패키지 목록
 ┣ 📜 .env                # 환경 변수 (로컬 실행용)
 ┗ 📜 README.md           # 프로젝트 설명서
```

---
Developed using Streamlit & OpenAI API.
