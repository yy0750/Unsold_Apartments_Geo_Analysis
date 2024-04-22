# 시공간 데이터분석 캡스톤디자인
## 미분양 아파트 입지 분석

👨‍💻 팀원: 조용진, 이채현 <br>
🕑 준비기간: 2023.05.04 ~ 2023.06.15<br>
🖥 분석도구: Python

## 1. 사용 데이터
- 경쟁률
- 지역별 미분양 수
- 인구수
- 면적
- 지역 내 총생산

|index|지역|연도|데이터|
|---|---|---|---|
|0|종로구|2013\.1\.1|27|
|1|종로구|2014\.1\.1|28|
|2|종로구|2015\.1\.1|211|

|index|지역|인구|면적|인구밀도|지역내총생산|
|---|---|---|---|---|---|
|0|종로구|150453|23\.91|6292|35719537|
|1|중구|131793|9\.96|13232|61342710|
|2|용산구|227106|21\.87|10386|13294640|



|index|연도|월|지역|주택 명|공급 세대 수 |접수 건수|경쟁률|위도|경도|
|---|---|---|---|---|---|---|---|---|---|
|0|2018|8|노원구|노원 꿈에그린|60|5877|97\.95|37\.66138873|127\.061417|
|1|2018|9|동대문구|장안동 U 포그니 2차|54|547|10\.13|37\.57112601|127\.0646213|
|2|2018|10|강서구|신마곡 벽산 블루밍|69|3778|54\.75|37\.57119225|126\.8041|


## 2.분석 목적
```
지리적 정보, 경쟁률, 인구 데이터를 이용하여 미분양 아파트의 위치를 분석하여 자주 발생하는 미분양 아파트의 위치를 파악하고 향후 우려 지역을 예측
```
## 3. 프로젝트 요약
```
- 변수들 간의 상관관계를 조사하고 최적 군집 수를 결정하기 위해 Elbow Method 사용
- Folium 지리 정보 시각화 도구를 활용하여 연도별 미분양 지역을 표시
```

## 참고사항
서울시 미분양주택 현환 통계: https://data.seoul.go.kr/dataList/10741/S/2/datasetView.do <br>
서울시 주민등록인구 (구별) 통계: https://data.seoul.go.kr/dataList/419/S/2/datasetView.do <br>
국토교통 통계누리: https://stat.molit.go.kr/portal/main/portalMain.do <br>
국토교통부 공간빅데이터 분석플랫폼: http://geobigdata.go.kr/portal/case/standardList.do
