<div align="center">

# <img width="256" height="256" alt="image" src="https://github.com/user-attachments/assets/b6636962-edf9-4a57-bd70-6c66ad81749e" />
### 띠링 (Ddiring)

### 어르신과 가족을 잇는 AI 기반 일상 돌봄 연결 서비스

> '띠링'은 알림음을 연상시키는 이름으로,<br/>
> 어르신의 안부가 알림처럼 가족에게 따뜻하게 전해진다는 의미를 담았습니다.

<p>
  <img src="https://img.shields.io/badge/Java-17-007396?logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring%20Boot-3.5-6DB33F?logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/React%20Native-0.81-61DAFB?logo=react&logoColor=white">
  <img src="https://img.shields.io/badge/Expo-54-000020?logo=expo&logoColor=white">
  <img src="https://img.shields.io/badge/FastAPI-LangGraph-009688?logo=fastapi&logoColor=white">
  <img src="https://img.shields.io/badge/Claude-Haiku%20%7C%20Sonnet-D97757?logo=anthropic&logoColor=white">
  <img src="https://img.shields.io/badge/AWS-EC2%20%7C%20S3%20%7C%20RDS-FF9900?logo=amazonaws&logoColor=white">
</p>

**캡스톤디자인 07분반 5조**

</div>

---


https://github.com/user-attachments/assets/46f2f5ea-1b64-4e9d-aad3-23928141f5a5



## 🌿 우리가 풀고자 한 문제

독거노인이 증가하면서, 멀리 사는 보호자 가족이 어르신의 일상 안부를 **매일** 확인하기는 점점 어려워지고 있습니다. 기존 방식에는 분명한 한계가 있습니다.

- 📞 **전화·메신저** — 보호자의 능동적 노력에 전적으로 의존하고, 기록이 누적되지 않습니다.
- 📡 **활동 감지 센서** — 물리적 움직임만 측정할 뿐, 정서·건강 상태는 파악하지 못합니다.
- 🚨 **응급 호출 버튼** — 사후 대응 중심이라, 일상적 변화의 점진적 추적이 어렵습니다.

또한 매일 똑같은 안부 질문이 반복되면 어르신은 피로감을 느끼고, 보호자는 단편적인 "잘 지내" 응답만으로 미묘한 변화를 포착하기 어렵습니다.

## 💡 띠링의 해결 방식

**띠링**은 어르신의 일상(약 복용·식사·기분·활동·안전 등)을 매일 **체크리스트(설문)** 형태로 가볍게 확인하고, 그 결과를 보호자가 한눈에 모니터링할 수 있게 합니다.

| | |
|---|---|
| 🤖 **개인화된 안부 경험** | AI가 어르신 프로필·최근 응답을 반영해 기계적인 질문을 따뜻한 발화로 변환하고, TTS 음성까지 제공해 디지털 취약 계층의 사용 장벽을 낮춥니다. |
| 📊 **데이터 기반 돌봄** | 일일 응답을 누적·집계해 일일 요약·주간 패턴 리포트를 만들고, 위험 신호(연속 약 복용 누락·우울감 지속 등)를 감지해 보호자에게 알림을 보냅니다. |
| 💝 **가족 간 정서적 연결** | 일일 사진 공유, 초대코드 기반 가족방, 출석 체크로 단순 모니터링을 넘어선 정서적 교류 채널을 제공합니다. |

---

## 🗂 레포지토리

| 레포지토리 | 파트 | 핵심 스택 |
|---|---|---|
| [**SERVER**](https://github.com/ddiring-team/SERVER) | Backend | Java 17, Spring Boot 3.5, Spring Security(JWT), JPA, MySQL |
| [**FRONT**](https://github.com/ddiring-team/FRONT) | Frontend | React Native 0.81, Expo 54, React 19, TypeScript |
| [**AI**](https://github.com/ddiring-team/AI) | AI | Python 3.11, FastAPI, LangChain, LangGraph |

---

## 🏗 시스템 아키텍처

<img width="1690" height="931" alt="image" src="https://github.com/user-attachments/assets/ab1f5e65-a07b-477b-805e-34faf2020745" />


---

## 🧰 기술 스택

### Backend ([SERVER](https://github.com/ddiring-team/SERVER))
`Java 17` · `Spring Boot 3.5` · `Spring Security (JWT, HS512)` · `Spring Data JPA` · `Spring Cache (Caffeine)` · `MySQL (AWS RDS)` · `Kakao OAuth2` · `Firebase Admin SDK (FCM)` · `AWS S3` · `Swagger`

### Frontend ([FRONT](https://github.com/ddiring-team/FRONT))
`React Native 0.81` · `Expo 54` · `React 19` · `TypeScript 5.9` · `expo-secure-store` · `@react-native-firebase/messaging` · `expo-image-picker`

### AI ([AI](https://github.com/ddiring-team/AI))
`Python 3.11` · `FastAPI` · `LangChain` · `LangGraph` · `Anthropic Claude (Haiku 4.5 / Sonnet 4.6)` · `OpenAI TTS` · `LangSmith` · `Pydantic`

### Infra / DevOps
`AWS EC2` · `AWS ECR` · `AWS S3` · `AWS RDS` · `Docker / Docker Compose` · `GitHub Actions (CI/CD)`

> AI 그래프는 호출 빈도·비용에 따라 모델을 분리 운영합니다. 고빈도·단순 작업(질문 변환·위험 문구·일일 요약)은 **Claude Haiku 4.5**, 추론 품질이 중요한 주간 패턴 분석은 **Claude Sonnet 4.6** 으로 처리합니다.

---

## 👥 팀 구성

| 이름 | 역할 | 담당 |
|---|---|---|
| 김현수 | **Frontend** | React Native 앱 ([FRONT](https://github.com/ddiring-team/FRONT)) |
| 박성제 | **Backend** | Spring Boot 서버 ([SERVER](https://github.com/ddiring-team/SERVER)) |
| 이현택 | **AI** | FastAPI · LangGraph ([AI](https://github.com/ddiring-team/AI)) |

**협업 전략** — Organization 내 파트별 레포지토리를 분리 운영하고, Gitflow(`이슈 → 브랜치 → PR → 코드 리뷰 → merge`)로 개발합니다. merge된 코드는 GitHub Actions를 통해 ECR 빌드 후 EC2에 자동 배포됩니다.

---

## 🔗 링크

| 구분 | 링크 |
|---|---|
| 📑 API 명세서 (Swagger) | https://api.ddiringapp.com/swagger-ui/index.html |
| 📝 Notion | https://app.notion.com/p/30e3059d1a8a80f98df4f6f67e004ee0 |
| 🎨 Figma (Wireframe) | [바로가기](https://www.figma.com/design/djRijsyJIo9uOndvldJHoW/) |

<div align="center">

---

🔔 *어르신의 안부가 알림처럼, 가족에게 따뜻하게.*

</div>
