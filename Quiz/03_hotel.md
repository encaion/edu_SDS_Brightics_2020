## 'hotel_booking_train_1m.csv' 데이터를 사용하여 다음의 분석을 실시하시오
(수치형 변수 [orig_destination_distance], [srch_adults_cnt], [srch_children_cnt], [srch_rm_cnt], [cnt] 를 제외한 나머지 변수는 전부 문자형으로 설정한다.) 

### 1. 데이터에 존재하는 결측치 개수의 총합은 얼마인가?

### 2. 결측치가 존재하는 행(row)를 전부 제거하시오.
 ※ 날짜 관련 변수에도 null이 아닌 결측치로 의심되는 데이터가 있다.
 ※ 본 문제의 결과를 base table 로 정의 한다.)

### 3. base table을 기준으로 접속 사이트[site_name]의 개수와 유입 경로[channel] 개수가 각각 몇 개인지 차례대로 기술하시오.

### 4. base table을 기준으로 접속 사이트[site_name]의 개수와 유입 경로[channel] 개수의 조합은 총 몇 개인가?

### 5. base table을 기준으로 유입 경로[channel]별 성과 분석을 하고자 한다. 유입 경로별 예약[is_booking] 비율이 가장 높은 채널 3개를 골라 높은 순으로 차례대로 기술하시오.

### 6. 5번에서 확인한 3개의 유입 경로를 기준으로 데이터를 필터링 하시오.
(본 문제의 결과를 table1 로 정의 한다.)

### 7. table1을 기준으로 사용자 접속 국가[user_location_country]와 호텔이 위치한 국가[hotel_country]가 같은 경우 국내 여행이라고 할 수 있다. 국내 여행 중 가장 거리(orig_destination_distance)가 먼 경우의 국가 번호(user_location_country)를 기술하시오.

### 8. table1을 기준으로 검색일(date_time)에서 체크인 일자(srch_ci) 까지의 차이를 계산하고 [date_diff] 라는 새로운 변수에 그 값을 대입하시오.
 ※ SQlite - julianday() 활용 가능

### 9. [date_diff] 가 음수인 행(row)의 개수를 기술하고 이를 제거하시오.
(본 문제의 결과를 table2 로 정의 한다.)

### 10. table2를 기준으로 각 검색데이터에서(row) 숙박 일수를 계산하고 "nights" 라는 새로운 변수에 그 값을 대입하시오.
 ※ srch_ci, srch_co 변수 활용, 4박 5일의 경우 4로 계산
 ※ SQlite - julianday() 사용 권장

### 11. table2를 기준으로 [date_diff], [nights], [orig_destination_distance] 변수간 상관분석을 실시하고 상관계수가 가장 높은 것을 골라 소수점 둘 째 자리까지 반올림하여 기술하시오.
