# Dacon_Jobcare_rec
데이콘 잡케어 추천 알고리즘 경진대회

### Summary
- Model : Catboost
- Feature : 약 60개 카테고리컬 설명변수, 이진분류 예측(1 : 사용, 0 : 미사용)
- 핵심 : **카테고리컬 변수가 많을 때 Catboost가 높은 성능을 보일 수 있는 이유**

### Features
- 사람에 관련된 feature들과 콘텐츠에 관련되 feature들로 나뉘어져있음
- 양 쪽에 매칭 가능한(공통의) feature : a, c, d, e, h
- d, h, l은 각각 더욱 세부적으로 나뉨

![image](https://user-images.githubusercontent.com/25517592/152281049-8f500836-9746-488b-b1c3-329ec99c5003.png)

## Feature Engineering
- nof_match(int) : 공통 feature인 a, c, d, e, h 중 몇개가 일치하는지
