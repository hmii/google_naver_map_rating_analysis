# map_scrapping_project
네이버 및 구글 지도 별점, 리뷰 스크래핑, 맛집 분석

### 스크래핑 
- 네이버 지도 스크래핑 : [naver_map_scrapping_selenium.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/naver_map_scrapping_selenium.ipynb)  
- 구글 지도 스크래핑 : [google_map_scrapping_selenium.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/google_map_scrapping_selenium.ipynb)

### 데이터 전처리  
- 중복제거 : [google_concat_dropduplicate.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/google_concat_dropduplicate.ipynb)  
    - 파일 여러개 합치기, 중복제거, 데이터 타입 변경
- 주소 및 업종 분류 : [contains_address_isin_restaurant.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/contains_address_isin_restaurant.ipynb) 
    - 해당 주소가 아닌 장소 걸러내기, 음식점 아닌 곳 제외하기 
    - regex, contains, isin
### EDA
- 기술통계 및 분포 분석 : [EDA_nolimit.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/EDA_nolimit.ipynb)
