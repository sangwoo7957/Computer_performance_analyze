# Computer_performance_analyze
- 컴퓨터의 성능을 종합하여 어떠한 차이가 있는지 알아보기 위한 프로젝트

# Requirements
- requests
- pandas
- numpy
- csv
- matplotlib
- scikit-learn

# Structure
1. Data Collection
   - 데이터들을 Amazon api(Rainforest API)에서 key를 받아 amazon 해당 url를 통하여 데이터들을 request해 json형식으로 수집(get)하여 우리가 필요한 데이터(Computer price, speed, ram etc)들만을 추출
2. 추출한 데이터를 PCA를 사용하여 차원을 2차원으로 축소하였다 (raw data는 총 10차원)
3. Kmeans를 사용
   - n_cluster를 차례로 높여가며 비교를 해보았지만 3개의 군집으로 하였을 때가 가장 분류하기가 좋았다
   - 각 군집 별로 나누어 성능 비교
   - matplotlib을 사용하여 그래프 생성
# Result
   - 가격이 비쌀수록 hardware의 성능이 높은 것을 알 수 있다
   - 다른 성능(Speed, ram etc)은 거의 다 비슷한 것을 알 수 있다

