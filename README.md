# 📘 Data Analysis Intro

---

### 📌 데이터 분석(Data Analysis)
데이터 분석은 원시 데이터(raw data)를 활용해 **패턴·흐름·관계**를 발견하고  
이를 통해 **의사결정 품질 개선**과 **비즈니스 성장 전략 수립**을 가능하게 하는 과정이다.

---

### 📌 ETL (Extract · Transform · Load)

![etl](https://github.com/user-attachments/assets/9411f790-a378-47ba-abf2-250f050982c3)

ETL은 데이터를 분석 가능한 구조로 만들기 위해  
**추출(Extract) → 변환(Transform) → 적재(Load)** 의 과정을 거친다.

#### ▫ Extract (추출)
- DB, Logs, API 등 다양한 소스에서 원본 데이터 수집

#### ▫ Transform (변환)
- 정제, 결측치 처리, 포맷 변환, 스키마 통합 등 가공 과정 수행

#### ▫ Load (적재)
- 데이터 웨어하우스 또는 분석 플랫폼에 저장

---

### 📌 확률변수 (Random Variable)
확률변수는 시행(trial)의 결과에 따라 값이 결정되는 변수이며  
머신러닝, 통계, 딥러닝의 핵심 기반 개념이다.

#### ▫ 특징
- 확률변수는 **대문자(X, Y)** 로 표현
- 값들은 집합 형태로 구성됨  
  예: Y = { y₁, y₂, y₃ }
- 각 y₁, y₂, y₃은 **확률변수값(value)**

![random-variable](https://github.com/user-attachments/assets/3ff2bbff-cfab-4f1c-9f2e-9f2f98498a89)

---

### 📌 정규분포 (Normal Distribution)
정규분포는 많은 자연·사회 데이터가 따르는 대표적인 분포이며,  
여러 비정규분포도 극한에서는 정규분포에 수렴한다.

![normal1](https://github.com/user-attachments/assets/ce3f3d56-c1af-46fc-a896-410b19c320d1)
![normal2](https://github.com/user-attachments/assets/28d1b39f-69b7-4b61-96cb-2649ddcc9b00)

#### ▫ 확률밀도함수(PDF)
![pdf1](https://github.com/user-attachments/assets/f2637fe9-5436-4922-87a1-133972646d72)
![pdf2](https://github.com/user-attachments/assets/d07bf86e-579f-48ae-83f4-aff1fb93c337)

---

## 1️⃣ Numpy

Numpy는 머신러닝·데이터 분석 환경에서  
데이터 **추출 / 가공 / 변환**을 위해 가장 먼저 익혀야 하는 기반 라이브러리이다.

### ▫ ndarray
- N차원 배열 구조  
- 파이썬 리스트보다 빠르고 연산 최적화됨

### ▫ astype()
- 배열 요소의 **데이터 타입 변경**
- 대량 데이터 처리 시 메모리 절약 가능

### ▫ axis
- 배열의 연산 방향을 나타내는 **축 개념**

<img width="1045" height="276" alt="numpy2" src="https://github.com/user-attachments/assets/c7f16abb-ee59-49b4-b4c9-ba0151faca9a" />

### ▫ 주요 초기화 함수
- `arange()` : 범위 기반 연속값 생성  
- `zeros()` : 0으로 초기화  
- `ones()` : 1으로 초기화  

---

## 2️⃣ Pandas

Pandas는 **표(테이블) 형태의 2차원 데이터**를 처리하기 위한 필수 데이터 분석 라이브러리이다.

### ▫ Pandas 구성요소
- **DataFrame** : 행·열로 구성된 구조  
- **Series** : 1차원 데이터  
- **Index** : 행 번호(고유값)  

### ▫ 주요 기능
- `DataFrame()` : 다양한 자료구조를 DataFrame으로 변환  
- `read_csv()` : CSV 파일 로드  
- `head()` : 상위 N행 미리보기  

---

## 3️⃣ 2023 행복지수 데이터 분석  
### (GDP · Social Support)

GDP와 사회적 지지는 **행복지수와 직접적인 상관관계**를 가진다.

<img width="577" height="569" alt="happiness_report_2023" src="https://github.com/user-attachments/assets/72095f52-9be0-49e8-9241-7469bcdc504f" />

### ▫ 분석 요약
- 두 지표(GDP & Social Support)가 모두 높을수록 **행복지수가 안정적**  
- 둘 중 하나라도 낮으면 **행복 수준 격차 증가**  

---

## 4️⃣ Visualization (시각화)

데이터의 **분포·패턴·상관관계·이상치**를 파악하기 위해 시각화를 사용한다.

<img width="919" height="228" alt="visual01" src="https://github.com/user-attachments/assets/68fcf8ef-9d02-498a-a23a-bef1adc6f755" />

### ▫ 대표 시각화 종류
- Bar Chart  
- Pie Chart  
- Line Chart  
- Violin Plot  
- Scatter Plot  
- Histogram  
- KDE Plot  

---

## 5️⃣ RFM 분석 (Recency · Frequency · Monetary)

RFM 분석은 고객의 구매 행동을 **정량적으로 평가하여 그룹화**하는 대표적인 고객 분석 기법이다.

### ▫ RFM 정의
- **Recency** : 얼마나 최근에 구매했는가  
- **Frequency** : 얼마나 자주 구매했는가  
- **Monetary** : 얼마나 많은 금액을 썼는가  

---

## 6️⃣ 이커머스 A기업의 RFM 분석

### ▫ 고객 데이터 구성
- Year_Birth → Age 변환 가능  
- MntWines, MntFruits 등 카테고리 소비 정보  
- 매장/웹 구매 횟수, 웹 방문 횟수  
- 캠페인 참여 정보(Cmp1~Response): 전반적으로 응답률 낮음  
- ID 컬럼은 분석에 직접 사용되지 않음  

### ▫ 분석 중 발견된 특징
- Z_CostContact, Z_Revenue 변수 설명 부족  
- 캠페인 관련 변수 전체적으로 응답률이 낮은 편  

---


