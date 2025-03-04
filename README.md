# 7th-ML-1team
# 개발,데이터 직군 면접 질문 추천시스템

## 폴더 구조
┣ 📂 1 data #직군 별 면접 질문 및 질문 유형 엑셀 파일

┣ 📂 2 modeling # 면접 질문을 올바른 직군으로 분류하는 분류 모델 코드 

┗ 📂 3 preprocessing_code # 면접 질문 데이터를 벡터화하고 백번역으로 증강시킨 코드 

## 📃 기획 계기
면접 질문들은 여러 사이트에 분산되어 있어 정보 획득에 불편함이 있고 어떤 질문이 중요한 질문인지 판단하기 힘들다. 이에 면접 질문 데이터를 모아 하나의 앱에서 제공하고 비슷한 질문의 빈도수를 이용해 중요도를 평가하여 빈도수가 높은 질문을 상대적으로 중요한 질문으로 제공하도록한다.

### 데이터 크롤링
GitHub 레포지토리 활용
- https://github.com/devham76/tech-interview-study
- https://github.com/WooVictory/Ready-For-Tech-Interview
- https://github.com/brave-people/brave-tech-interview
- https://github.com/gyoogle/tech-interview-for-developer
- https://github.com/4z7l/tech_interview.zip
- https://github.com/JaeYeopHan/Interview_Question_for_Beginner
- https://github.com/zzsza/Datascience-Interview-Questions
- https://github.com/dhkdn9192/data_engineer_career
- https://github.com/boost-devs/ai-tech-interview
- https://github.com/WeareSoft/tech-interview
- https://github.com/baeharam/Must-Know-About-Fronten


### 데이터 전처리
- KoNLPy를 사용하여 토큰화 진행 후 TF=IDF벡터화
- 백번역 기법을 활용하여 원문의 의미를 유지하면서 단어, 어미등만 달라지도록 하여 데이터를 증강


### 모델링 과정
- 코사인 유사도를 이용한 텍스트 간 유사도를 기반으로 분류
- SVM, RandomForest, XGBoost 모델을 사용하고 그리드서치 및 베이지안 최적화로 하이퍼 파라미터를 튜닝



