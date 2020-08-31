# kaggle_titanic
practicing basic of ML with kaggle titanic 

> "경기도 빅데이터 전문가 과정" 프로젝트 -> 타이타닉 생존자 데이터로 ML 실습

## 목차

### 1. 데이터 준비 및 탐색 / Preparing dataset
### 2. 데이터 전처리 방법 & 선택 이유 / Feature engineering & Feature selection 
    1) 데이터 전처리 후 유의미한 feature 선택하기
    2) dataset 다시 만들기
### 3. 모델 적용 프로세스 및 결과 / 3개의 기본 모델 선택 (SVC, KNN, 의사결정나무)
    1) KNN 모델 
    2) SVC 모델 
    3) 의사결정나무
    4) XGBOOST
    5) Random Forest
### 4. 모델 간 성능비교 / Predict on test data & Check the result with metrics
    1) KNN 모델, SVC모델, 의사결정나무, XGBOOST, Random Forest
    
## +Review

### 데이터 전처리의 중요성
- 결측치 처리가 관건임 : 중앙값, 평균값, 최빈값, 혹은 ML로 예측 등 적절한 방법을 활용해야 함
- domain knowledge 의 중요성 : 예를들어 타이타닉 배의 구조를 알고 있어서 cabin의 위치 등을 파악 할 수 있다면 정확도를 높일 수 있을 것임. 
- feature 균형 맞추기 : 데이터셋에서 feature들 간 스케일 불균형 정규화(Z-score Normalization), 원핫인코딩 등을 활용하면 더 좋은 결과 얻을 수 있을 거라 예상됨
- 탈락 시킨 다른 feature도 잘 활용할 수 있을 것 같음 : 예를들어 name의 경우 정규식을 이용해 호칭만 추출해서 활용 가능할 것.


### ML 모델 셀렉션
- 같은 데이터를 활용해도 모델 별로 정확도가 다름.
- 여러가지 모델을 테스트해보고 가장 높은 정확도를 보이는 것으로 선택하는 것이 좋음
- confusion matrix , roc_curve로 모델 별 detail을 확인하기도 가능

### 기타
- ML의 전반적인 프로세스를 이해할 수 있었음.
- 통계적 지식의 중요성 : 정확한 분석을 위해 통계적 지식을 적용할 필요성을 느낌.
- 팀워크와 의사소통의 중요성:
<br>
    우리팀은 모두 코딩 초보였기 때문에 충분히 의사사통하고 역할을 고르게 분담하기로 함
    feature eng 부터 ML test까지 한 파트 씩 담당해서 분업함
    정기적으로 결과물을 확인하고 피드백 함
    --> 빠른 시간에 모두 이해할 수 있는 결과를 도출할 수 있었음.
