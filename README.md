<div align="center">

# 하정민 · Jungmin Ha

**ML Engineer · AI 석사**

데이터 수집부터 모델 설계, 실서비스 배포까지<br>AI 개발 전 과정을 단독으로 수행하는 ML 엔지니어입니다.

<br>

[![Portfolio](https://img.shields.io/badge/🌐_포트폴리오-hazzyai.github.io-4361EE?style=for-the-badge)](https://hazzyai.github.io)
&nbsp;
[![Email](https://img.shields.io/badge/📧_이메일-gkckdals3@naver.com-555555?style=for-the-badge)](mailto:gkckdals3@naver.com)

<br>

| | | |
|:---:|:---|:---|
| 🔐 | **필상 (Pillsang)** | ML 엔지니어 — 피싱 탐지 AI 모델 설계 · 실서비스 배포 |
| 🎓 | **충남대학교 대학원** | 바이오AI융합학과 석사 (2023) · GPA 4.33/4.5 |
| 📋 | **국가 R&D 2회** | 딥테크 TIPS · 스케일업 TIPS |
| 🏆 | **수상 5회** | 교외 3관 · 교내 2관 |
| 📄 | **특허 등록 2건** | AI 관련 특허 2건 |

</div>

<br>

---

## 🔬 국가과제 연구

<br>

### 딥테크 TIPS — Cascade 멀티스테이지 피싱 탐지 연구

[![Private](https://img.shields.io/badge/🔒_Private-비공개_레포-red?style=flat-square)](.)
&nbsp;
![Status](https://img.shields.io/badge/Status-진행중-brightgreen?style=flat-square)
&nbsp;
`피싱 탐지` `Cascade` `멀티스테이지` `NLP 딥러닝` `경량화`

단일 모델의 한계를 극복하기 위해 **3단계 Cascade 구조**를 설계했습니다.
명확한 케이스는 앞 단계에서 저비용으로 처리하고, 판별이 어려운 케이스만 다음 단계로 전달해 정확도와 추론 속도를 동시에 개선합니다.

```
Stage 1 │ URL + HTML 특성 기반 경량 탐지   →  명확한 케이스 조기 처리
Stage 2 │ 보안 관점 취약점 분석            →  중간 난이도 케이스 처리
Stage 3 │ NLP 딥러닝 모델                  →  판별 어려운 케이스 최종 처리
```

<br>

### 스케일업 TIPS — Multimodal RAG 피싱 탐지 연구

[![Private](https://img.shields.io/badge/🔒_Private-비공개_레포-red?style=flat-square)](.)
&nbsp;
![Status](https://img.shields.io/badge/Status-진행중-brightgreen?style=flat-square)
&nbsp;
`Multimodal RAG` `Llama 3.1 70B` `QLoRA` `BGE-M3` `SigLIP` `PaddleOCR`

피싱 사이트 탐지를 위한 **4-Modality VectorDB 기반 RAG 시스템**을 설계·개발 중입니다.

```
URL 분석  ──┐
HTML 파싱 ──┤──▶  Multimodal VectorDB (Qdrant)  ──▶  Llama 3.1 70B QLoRA
OCR 텍스트 ─┤         BGE-M3 임베딩 / SigLIP
이미지 비전 ─┘         PaddleOCR
```

<br>

---

## 🚀 프로젝트

<br>

### 필상 AI Chrome 확장프로그램

[![GitHub](https://img.shields.io/badge/GitHub-hazzyAI/pillsang--chrome--extension-181717?style=flat-square&logo=github)](https://github.com/hazzyAI/pillsang-chrome-extension)
&nbsp;
![Chrome](https://img.shields.io/badge/Chrome_Web_Store-심사완료-4285F4?style=flat-square&logo=google-chrome&logoColor=white)
&nbsp;
`CatBoost ONNX` `Manifest V3` `온디바이스 추론` `Service Worker` `2단계 탐지`

AI 탐지 기능을 탑재한 Chrome 확장프로그램을 **기획부터 배포까지 단독 개발**했습니다.

- **1차 탐지**: 서버 DB API 조회 (화이트/블랙리스트 즉시 판별)
- **2차 탐지**: 미등록 URL → CatBoost ONNX 온디바이스 추론
- 탐지 결과 DB 적재 → 신규 URL 자동 리스트 편입 (피드백 루프 구성)
- 악성 확률에 따른 4단계 UI 표시 · 자동 알림 · 리디렉션 처리

<br>

### 싹다잡아 — 피싱 탐지 ML 모델 (실서비스 배포)

[![PlayStore](https://img.shields.io/badge/Google_Play-누적_50만+_다운로드-3DDC84?style=flat-square&logo=google-play&logoColor=white)](https://play.google.com/store/apps/details?id=com.ps.wb&hl=ko)
&nbsp;
`CatBoost` `ONNX Runtime` `Android 온디바이스` `추론 10ms 이하` `SHAP` `MLflow`

누적 다운로드 **50만+ 보안 앱**에 피싱 탐지 ML 모델을 **최초로 설계·탑재**했습니다.

- 논문 기반 특성 후보군 선정 → 180개 수치형 특성 구성 → Feature Selection으로 80개 압축
- CatBoost 모델 선정 및 파인튜닝 → ONNX 변환 → Python 출력값 정합성 검증
- HTML 수집 불가 환경을 위한 Fallback 구조 별도 설계
- Android 온디바이스 추론 구현 · **추론 시간 10ms 이하** 달성
- MLflow 실험 관리 · SHAP 기반 모델 해석

<br>

---

## 🏆 대회

<br>

### 🌐 교외대회

<br>

**🥉 AI 대학원 챌린지 with KT 믿:음** &nbsp;·&nbsp; 3위 · IITP 원장상 &nbsp;·&nbsp; KT · IITP · 2023

[![GitHub](https://img.shields.io/badge/GitHub-KT--AI--Competition-181717?style=flat-square&logo=github)](https://github.com/hazzyAI/KT-AI-Competition)
&nbsp;
`LLM 파인튜닝` `KT Mi:dm` `의료 AI` `대화형 진단` `데이터 증강` `크롤링`

KT Mi:dm LLM을 파인튜닝해 의료 접근성 문제를 해결하는 **대화형 진단 AI**를 개발했습니다.
공개 데이터가 없어 병원 사이트를 직접 크롤링 + LLM 기반 데이터 증강으로 학습 데이터를 구축했으며,
증상 입력 → 질병 후보 제시 → 추가 질문으로 진단을 세분화하는 구조를 설계했습니다.

<br>

**🥈 스마트축사 데이터 활용대회** &nbsp;·&nbsp; 우수상 &nbsp;·&nbsp; 과기부 · NIA · SK · 2022

[![GitHub](https://img.shields.io/badge/GitHub-SK--Competition-181717?style=flat-square&logo=github)](https://github.com/hazzyAI/SK-Competition)
&nbsp;
`Swin Transformer` `Instance Segmentation` `mmdetection` `Weighted mAP 0.97434`

YOLOv5 · Mask R-CNN · Swin Transformer 비교 실험 후 **Swin Transformer 최종 채택**,
한우 발정 탐지 모델을 개발해 **Weighted mAP 0.97434** 달성. → KSC 2023 학술발표로 이어짐

<br>

**🥇 바이오AI융합 해커톤** &nbsp;·&nbsp; 대상 · 1위 &nbsp;·&nbsp; DACON · 2022

[![GitHub](https://img.shields.io/badge/GitHub-BIOAI--Competition-181717?style=flat-square&logo=github)](https://github.com/hazzyAI/BIOAI-Competition)
&nbsp;
`BioPython` `Protein Feature Extraction` `CatBoost` `ESM-v2 대비 RMSE 54% 개선`

BERT 기반 단백질 언어모델(ESM-v2)과 BioPython 기반 도메인 특성 추출 방식을 비교 실험,
직접 추출한 특성이 대형 언어모델을 압도함을 증명. **ESM-v2(RMSE 4.37) 대비 RMSE 2.00866 달성 (54% 개선)**
→ AAiCON 2023 학술발표로 이어짐

<br>

---

### 🏫 교내대회

<br>

**🏆 바이오AI융합인재 특허 아이디어 대회** &nbsp;·&nbsp; 최우수상 &nbsp;·&nbsp; 충남대 · 2022

`DNN 기반 DTI 모델` `약물 청소율 예측` `특허 등록으로 연결`

DNN 기반 약물-표적 단백질 상호작용(DTI) 모델로 약물 청소율을 추정하는 시스템을 제안.
이후 **특허 제10-2730477호** 등록으로 이어짐

<br>

**🥈 바이오AI융합 경진대회** &nbsp;·&nbsp; 우수상 &nbsp;·&nbsp; 충남대 · 신테카바이오 · 2021

[![GitHub](https://img.shields.io/badge/GitHub-BIOAI2--Competition-181717?style=flat-square&logo=github)](https://github.com/hazzyAI/BIOAI2-Competition)
&nbsp;
`Xception Fine-tuning` `알츠하이머 예측` `유전자 발현` `CNN` `SOTA 대비 2% 개선`

유전체 발현 데이터를 256×256 이미지로 마스킹 처리한 비식별화 데이터로
사전학습된 **Xception 모델을 파인튜닝**해 알츠하이머 발병 분류 모델 구성.
기존 SOTA 대비 **Accuracy 2% 이상 개선** → 신테카바이오 인턴십으로 이어짐

<br>

---

## 📄 특허

<br>

| 구분 | 특허명 | 번호 | 등록일 |
|:----:|--------|------|:------:|
| ✅ 등록 | 인공신경망 기반의 약물-표적 단백질 상호작용 모델을 활용한 청소율 예측 시스템 | 제10-2730477호 | 2024.11 |
| ✅ 등록 | 스마트 금고 인증 방법 및 이를 이용한 시스템 | 공개특허 10-2023-0127426 | — |

<br>

---

## 💼 경력

<br>

**🔐 (주) 필상** &nbsp;·&nbsp; ML 엔지니어 · 연구원 &nbsp;·&nbsp; 재직중

피싱·악성 URL 탐지 AI 서비스 연구 및 개발. 누적 다운로드 50만+ 보안 앱(싹다잡아)에 피싱 탐지 ML 모델 최초 설계 및 Android 온디바이스 배포. AI 탐지 기능을 탑재한 Chrome 확장프로그램 단독 개발. 국가 R&D 과제(딥테크 · 스케일업 TIPS) 2건 병행 수행.

<br>

**🎓 충남대학교 산학협력단** &nbsp;·&nbsp; 연구원 &nbsp;·&nbsp; 2023.09 – 2024.01

단백질-단백질 수소 결합 거리 예측 연구 및 학술논문 작성 (AAiCON 2023, KDBC 2022). 신약개발 AI 관련 특허 명세서 작성 (특허 제10-2730477호 등록). 스마트축사 발정 탐지 모델 연구 (KSC 2023 발표). 연구 성과 기반 사업계획서 작성 참여.

<br>

**🔬 신테카바이오(주)** &nbsp;·&nbsp; 인턴 &nbsp;·&nbsp; 2022.03 – 2022.05

바이오AI융합 경진대회 수상 성과를 기반으로 알츠하이머 발병 예측 모델 고도화 연구. 유전자 발현 데이터를 256×256 이미지로 마스킹 처리 후 사전학습된 Xception 모델을 파인튜닝해 기존 모델 대비 성능 개선.

<br>

---

## 🛠️ 기술스택

<br>

**ML / 경량화**

![CatBoost](https://img.shields.io/badge/CatBoost-FFD700?style=flat-square)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-FF6B6B?style=flat-square)

**DL / CV**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![mmdetection](https://img.shields.io/badge/mmdetection-FF4500?style=flat-square)

**LLM / RAG**

![Llama](https://img.shields.io/badge/Llama_3.1_70B_QLoRA-blueviolet?style=flat-square)
![BGE-M3](https://img.shields.io/badge/BGE--M3-4B0082?style=flat-square)
![SigLIP](https://img.shields.io/badge/SigLIP-1A73E8?style=flat-square)
![PaddleOCR](https://img.shields.io/badge/PaddleOCR-0062B1?style=flat-square)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)

**배포 / 서비스**

![Android](https://img.shields.io/badge/Android_온디바이스-3DDC84?style=flat-square&logo=android&logoColor=white)
![Chrome](https://img.shields.io/badge/Chrome_Extension_MV3-4285F4?style=flat-square&logo=google-chrome&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

**자격증**

![TOEIC](https://img.shields.io/badge/TOEIC_Speaking-IH-blue?style=flat-square)
![자격증](https://img.shields.io/badge/통신선로산업기사-취득-green?style=flat-square)
