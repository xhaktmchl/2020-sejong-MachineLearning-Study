# 데이터 전처리 
정의: 데이터의 품질을 올리는 것

# 저처리 기법
- 실수화
- 정제
- 통합
- 축소(데이터 수 줄이기(samplig) ,차원축소)
- 변환( 정규화, 구간화)
- 균형 



# 데이터 실수화
이용: dictVectorizer

# 데이터 변환
필요성: 데이터 간의 차이가 크면 패턴인식의 정확도 떨어짐
종류:
- 표준화
- 정규화 
(보통은 표준화<정규화 유용)
이용: 
- countVectorizer
- tfidVectorizer

# 데이터 정제
결측치 none, np.nan
결측치를 없애거나 평균,중앙,최빈값으로 채운다
이용: imputer ,fillna,dropna()

# 데이터 통합
: 여러 가지 데이터 통합
이용: pd.merge

# 데이터 불균형

