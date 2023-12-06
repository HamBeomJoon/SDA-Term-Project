CSV의 column은 [Date_reported, Country_code, Country, WHO_region, New_cases, Cumulative_cases, New_deaths, Cumulative_deaths]로 구성되어 있다.
 date_reported는 2020-01-20 이런식으로 연-월-일 형식으로 되어있는데, 전처리를 통해 월별로 WHO_region의 코로나 신규 감염자 수와 신규 사망자 수를 지역별로 다 더해서 line plot을 그림
* WHO_region은 대륙별로 나누어져 있음, y축값이 10**8까지 나와있어서 log10 scale로 변환시켜서 그림
* 신규 감염자 수는 WPRO 제외하고 그렸고, 신규 사망자 수는 Other 제외하고 그림
* 각각 지역별로 그리고, 마지막에 지역상관없이 누적 감염자 수, 사망자 수도 line plot으로 나타냄
