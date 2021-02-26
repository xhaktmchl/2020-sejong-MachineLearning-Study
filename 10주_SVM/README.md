# 서포트 벡터 머신(SVM)
## 개념
- 지도학습 모델
- 분류,회귀 모두 사용(분류>회귀)

## svm 학습방향
- margin의 최대화( 결정 경계로부터 데이터의 거리가 최대)

## 용어
- 결정경계(hyperplane)
- - 클래스를 분류하는 기준
- 서포트 벡터
- - 결정경계에서 가장 가까이에 있는 각 클랙스의 데이터
- 마진
- - 서포트 벡터 간의 거리

## 장점
- 서포트 벡터를 기준으로 결정경계를 결정짓기 때문에 outlier 에 영향을 거의 않받음


10.2주차
# hard margin svm  //  soft margin svm
- hard margin svm : 에러가 없는 선형분류
- soft margin svm : 에러가 존재해서 선형분류불가능 할 때 사용하는 선형분류


## 에러의 허용 정도
- C가 크면, 에러 허용 않함, 마진 감소(오버피팅)
- C가 작으면, 에러 허용 증가, 마진 증가(underfitting)

## svm 종류
- 1)선형 SVM
- - Hard margin svm/  soft margin svm
- 2) 비선형 svm
- - kernel svm

## 비선형 svm
- kernel을 통해 차원을 증가시킨다음 분류 가능
### 커널 선정법 
- 실험적으로 선정
- 커널의 종류(
- - RBF 커널,
- - sigmoid 커널, 
- - low degree polynomial 커널

# 다중 분류 svm(multi classification)
##  하나-나머지OVR(One-vs-Rest)
- 이항분류 값이 가장 큰 값을 그룹으로 할당
## 하나-하나 OVO(one-vs-one)
- n개의 분류기로 나누어 가장 많이 할당된 그룹으로 할당(voting 방식)
