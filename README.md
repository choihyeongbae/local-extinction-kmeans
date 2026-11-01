# 지방소멸위험 데이터 기반의 K-means 군집 분석 PBL

2026 SW·AI 교과융합 수업 자료(통합사회 · 공통수학2 · 정보)의 **Google Colab 실습 노트북**과 **CSV 데이터**입니다.  
경상북도 22개 시·군과 전국 229개 시·군·구의 인구 데이터를 분석하며, **표준화가 K-means 군집 결과를 어떻게 바꾸는지**를 두 점 사이의 거리 개념으로 탐구합니다.

## 차시별 노트북 (클릭하면 Colab에서 바로 열림)

| 차시 | 학습 주제 | 연계 교과 | 학생용 | 교사용 |
|---|---|---|---|---|
| 1차시 | CSV 데이터 분석으로 살펴보는 경북 시·군의 인구 구조 | 통합사회 + 정보 | [학생용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/student/lesson1_student.ipynb) | [교사용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/teacher/lesson1_teacher.ipynb) |
| 2차시 | 표준화와 K-means를 활용한 경북 시·군 군집 분석 | 공통수학2 + 정보 | [학생용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/student/lesson2_student.ipynb) | [교사용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/teacher/lesson2_teacher.ipynb) |
| 3차시 | 전국 시·군·구 군집 분석과 지역 맞춤형 인구 정책 제안 | 통합사회 + 정보 | [학생용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/student/lesson3_student.ipynb) | [교사용 열기](https://colab.research.google.com/github/choihyeongbae/local-extinction-kmeans/blob/main/notebooks/teacher/lesson3_teacher.ipynb) |

- **학생용**: 핵심 코드에 빈칸(`___`)이 있고, 모둠활동지 질문에 답을 적는 칸이 있습니다.
- **교사용**: 빈칸이 채워진 완성 코드, 실행 결과, 모범답안이 포함되어 있습니다.
- Colab에서 열린 노트북은 **[파일] → [Drive에 사본 저장]** 후 사용하세요.
- 데이터는 노트북 안에서 이 저장소의 주소로 바로 불러오므로 파일을 따로 업로드할 필요가 없습니다.

## 데이터 (`data/`)

| 파일 | 내용 | 열 |
|---|---|---|
| `gyeongbuk_2025.csv` | 경상북도 22개 시·군 | 시군, 연도, 총인구, 청년여성인구, 고령인구 |
| `korea_2025.csv` | 전국 17개 시도, 229개 시·군·구 | 시도, 시군구, 연도, 총인구, 청년여성인구, 고령인구 |

- 청년여성인구: 20~39세 여성 인구(명), 고령인구: 65세 이상 인구(명)
- 지방소멸위험지수 = 청년여성인구 ÷ 고령인구 (0.5 미만이면 소멸위험지역)
- 자료: 한국고용정보원(KEIS) 지방소멸위험지수 데이터(2025년)를 수업용으로 가공

## 실행 환경
Google Colab(Python 3), pandas, numpy, scikit-learn, matplotlib, koreanize-matplotlib(그래프 한글 표시, 노트북 첫 셀에서 설치)

---
개발: 포항여자고등학교 정보교사 최형배 (2026)
