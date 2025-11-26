# WeathePrediction
여러 관측소의 6년 치 기상데이터를 이용해 날씨 예측

# 데이터 셋 설명
- 모델 구성에 사용한 train set은 동두천, 서울, 강화, 인천, 이천, 양평 관측소의 2019년 1월 1일부터 2024년 12월 30일까지의 측정 데이터로 이루어져 있고, test set은 파주, 수원의 랜덤 날짜들의 측정 데이터로 이루어져 있다.
- station, date 변수를 제외한 모든 변수는 수치형 데이터이다.
- 변수명_n 형태의 변수들은 모두 시간대별로 나누어져 있으며, 각 변수는 하루 24시간에 해당하는 24개의 열로 구성되어 있다.
  
train, test set 모두 다음과 같은 feature를 가진다.
● id: 순서
● station: 지상관측소 번호
● station_name: 지상관측소 이름
● date: 날짜(월-일)
● cloud_cover_n: 증하층운량(10분위)
● dew_point_n: 이슬점 온도(°C)
● humidity_n: 습도(%)
● local_pressure_n: 현지기압(hPa)
● min_cloud_height_n: 최저운고(100m)
● precipitation_n: 강수량(mm)
● sea_level_pressure_n: 해면기압(hPa)
● snow_depth_n: 적설(cm)
● sunshine_duration_n: 일조(hr)
● surface_temp_n: 지면온도(°C)
● vapor_pressure_n: 증기압(hPa)
● visibility_n: 시정(10m)
● wind_speed_n: 풍속(m/s)
● wind_direction_n: 풍향(°)
● climatology_temp: 해당 날짜의 평균 기온(°C) (7년 평균 – 1월 1일인 경우 2018년부터 2024년까지 1월 1일 평균)
