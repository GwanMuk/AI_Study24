# AI_Study24
python을 이용한 머신러닝, 딥러닝 학습용

시나리오

MBC 상점에서 앱 마켓을 운영하는데 AI를 활용하는 기법을 학습해보자

미션이 있다고 가정하고 진행을 해본다.

1. 단계 : 앱 마켓에서 살아있는 생선을 팔기 시작함
2. 물류 센터에서 생선을 고르는 직원이 있는데 생선 이름을 못 외운다.
3. 생선의 종류 : 도미, 곤돌매기, 농어, 강꼬치고기, 빙어, 송어 ....
4. AI 미션 : 생선의 길이가 30cm 이상이면 도미

---------------------------------------------------------------
12/30
머신 러닝의 이론을 배우고 물고기의 데이터를 받아서 훈련세트, 테스트 세트로 나누어 ai학습 시킨다.
그 후에 값을 도출하고, 근사치의 값이 주어질 때 잘 예측해내는지 확인을 해본다.
단, 훈련세트와 테스트세트가 데이터의 편향화가 되지 않게 잘 섞어서 만들어야 한다.


12/31
훈련된 데이터 값을 볼 때 그래프의 x, y축 비율이 다르다면 판단을 제대로 할 수가 없다.
그래서 데이터 전처리를 표준점수화 해서 객채간 사이의 거리값을 줄여 값을 더 정확하게 도출하게 한다

추가적인 미션
1. 물고기의 주문량이 늘어나고 물고기 종류또한 달라지는 바람에 길이가 아닌 무게단위로 판매를 한다
2. 공급처에서 생선의 무게를 잘못 측정을 해서 보낼수도 있다.
3. 다행히 다른 데이터들은 정상범주에 있는 것 같으니 정상범위 데이터로 무게가 잘못 측정된 데이터의 무게를 예측을 해본다.

k-최근접 이웃 알고리즘을 이용해서 정상적인 데이터들을 비교해서 예상하는 값을 도출하게 해본다.

01/02
데이터들이 갯수가 적으면 예측하기 어려운 부분이 있다. 
만약 기존 데이터 이상의, 혹은 이하의 값을 예측하려고 할 때 예상값이 기대치보다 못한다.
그래서 만약에 데이터가 선형적으로 분포해 있다면 선형회귀와 다항회귀를 사용해서 값을 예측해서 구하는 방법을 연습한다.

선형회귀와 다항회귀를 사용해서 표본 이상의 값들을 함수를 활용해서 예측하는 연습을 함
선형회귀와 다항회귀의 한계점은 과소적합이 일어날 수 있다는걸을 알게됨

특성공학을 사용해서 특성을 여러개로 늘려서 고차항으로 만든 다음 다중회귀모델을 훈련시킨다.
단, 너무 많은 특성을 만들고 실행할 경우 선형 데이터가 아주 강해지기 때문에 과대적합이 나올 수 있다.
그래서 규제를 걸고 훈련세트와 테스트 세트의 격차를 좁게 규제를 건 뒤에 훈련을 시키고 평가한다.

01/03
추가적인 미션
1. 물고기가 너무 잘 팔린 나머지 랜덤 물고기박스를 판매하기로 함
2. 물고기의 종류는 7가지정도로 지정
3. 물고기의 종류가 몇%확률로 나오는지 표시해야함










