
<h1> 프로젝트 제목 : 따릉이 대여량 예측 </h1>
<h2> <li> 프로젝트 팀 이름 : DDA-BIKE </li> </h2>
<h2> <li> 프로젝트 내용 </li></h2>
<h3> 1. 데이터 전처리 </h3> 
- 결손값 처리, 이상치 제거 <br>
boxplot을 이용하여 이상치를 찾아냈는데 precipitation(비가오면 1 비가 안오면 0), windspeed(평균 풍속) <br>
ozone(오존), pm10(미세먼지), pm2.5(초미세먼지) 이 데이터들에서 나타났다. 이상치 처리 방법에는 <br>
1. 이상치 데이터를 행에서 모두 제거한다. <br>
2. 이상치 데이터를 중앙값, 평균값, 최빈값등으로 변경한다. <br>
이렇게 두가지로 나눌 수 있는데 나는 데이터를 제거하지 않고 fillna()를 이용하여 평균 값을 넣어주었다. (2022-10-30) <br>
<h3> 2. 탐색적 데이터 분석(EDA) </h3> 
- 데이터의 조직, 설명, 표현, 분석  <br>
1) count(시간에 따른 따릉이 대여수)는 pyplot을 이용하여 따릉이 대여수 이상치를 분석했다. <br>
2) windspeed(풍속)은 hist()를 이용하여 히스토그램을 그려보았는데 따릉이 예측에 필요한 데이터는 아니라고 분석했다.<br>
3) count와 hour 두개의 데이터 지표를 이용하여 시간에 따른 따릉이 대여수를 barplot으로 막대그래프를 표현했다.<br>
4) temperature(온도) 와 humidity(습도)를 곱해 날씨에 따른 따릉이 대여수를 scatterplot으로 표현했다.<br>
5) 데이터들의 상관관계를 알아보기위해 heatmap을 이용하였다. (2022-10-30) <br>
<h3> 3. 머신러닝 모델 학습 </h3> 
- XGBoost 및 다른 알고리즘을 사용하여 모델을 학습시킨다.  

<h3> 4. 모델 평가 및 실행 </h3>
- 모델의 성능이 좋은지 안좋은지 평가하고 안좋으면 좋게 발전시킨다.
<h2> <li>프로젝트 개발 툴 - Google Colab </li> </h2>
<h2> <li> 프로젝트 개발 언어 - Python </li> </h2>
<h2> <li> 앞으로 해야할 것 </li> </h2>
- 세가지 또는 더 많은 모델을 더해서 더 좋은 모델로 만들어 RMSE (평균 제곱근 오차)를 낮춘다
