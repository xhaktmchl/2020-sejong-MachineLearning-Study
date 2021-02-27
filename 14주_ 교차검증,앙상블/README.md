＃ 교차검증
##  파이프라인(pipeline)
- 개념: 전처리,학습, 검증을 한번에 묶을 수 있는 함수
- sklearn 라이브러리에 있음


## 모델 성능 평가
### 홀드아웃 교차검증(Holdout cross validation)
- 개념: training set에서 validation set을 따로 만들어 파라미터 학습에 사용하고 test set은 성능 추정에만 사용
- 단점: validation set 에 따라 모델의 성능의 편차가 심함
### k 겹 교차검증(K fold cross valiation)
- 개념: validation set에 따른 모델 성능의 편차를 보완하기 위해 training set을 k개로 나눈 다음 k번의 홀드아웃 교차검증을 통해 validation set에 대한 모델 성능의 평균을 구하는 것


## 모델 성능 최적화
### 과대적합(over fitting)
- 
### 과소적합(under fitting) 

### 과대적합 해결
- 1) 학습 데이터 보충
- 2) 모델규제(regularization) 늘림



////////////////////////////////////////////////////
# 앙상블

## 종류
- 다수결 투표
- 배깅
- 부스팅

## 다수결 투표(Majority Voting)
- 개념: 여러개의 모델중 결과값이 가장 많이 나온 것으로 분류

## 배깅(bagging)
- 개념: 같은 종류의 모델을 다른 학습 데이터를 가지고 여러 번 사용해  예측
- 부트스트랩(bootstrap) : (학습 데이터의 중복을 허용)
- 대표적 예) 
-  - 랜덤 포레스트 : DT를 여러번 사용 함 

## 부스팅(boosting)
- 개념: 학습 중 잘못 분류된 데이터의 50%를 학습에 재사용
- 예) AdaBoost: 잘못 분류된 데이터에 가중치를 부여해서 다시 학습




