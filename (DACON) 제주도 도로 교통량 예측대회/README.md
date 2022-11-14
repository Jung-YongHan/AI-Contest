제주도 도로 교통량 예측대회
---
두번째 경진대회

10% 이내에 드는 성적을 달성.

무엇보다 EDA부분에서 시간을 많이 들인 대회

1. EDA-  
train데이터와 test데이터 간의 관계 파악이 매우 중요함.  
train데이터 내에 test데이터가 포함되어 있는 피쳐가 많아서 대부분 Label/OneHotEncoding 고려.(categorical features)  
피쳐들의 unique/target과의 상관관계를 통하여 Label/OneHotEncoding을 하였음.  
수치형 데이터인 위경도는 선형모델 성능 향상을 위해 MinMaxScaling을 해주었음.

2. PreProcessing-  
한 피쳐를 바꾸면서 성능을 비교할 때 마다 버전을 만들어 주었음. 인코딩이 추가됨에 따라 성능이 점점 높아지는 것을 볼 수 있음.

3. Modeling-  
LGBM, RF, EXT 세 가지 모델을 사용하여 가중치보팅을 통해 예측해주었음. 빅데이터였고 모델 성능 평가하는데에 시간이 너무 오래걸려서 많은 예측을 하지 못한 것이 아쉬운 대회.
