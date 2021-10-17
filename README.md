# google_naver_map_rating_analysis
네이버 및 구글 지도의 음식점 별점 비교 분석

## 1. 배경
    - 목적 : 맛집을 찾을 때 플랫폼 지도가 제공하는 별점은 도움이 될까? 
            같은 지역, 음식점의 별점 비교를 통해 제공되는 정보를 믿을 수 있는지 살펴본다.
    - 플랫폼 : NAVER, GOOGLE
    - 지역 : 제주도 애월읍, 성산읍 
    - 대상 : 해당 지역 내 음식점 전체 

## 2. 과정
1. 스크래핑 
    - 네이버 지도 스크래핑 : [naver_map_scrapping_selenium.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/naver_map_scrapping_selenium.ipynb)  
    - 구글 지도 스크래핑 : [google_map_scrapping_selenium.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/google_map_scrapping_selenium.ipynb)

2. 데이터 전처리  
    - 중복제거 : [google_concat_dropduplicate.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/google_concat_dropduplicate.ipynb)  
        - 파일 취합, 중복 제거, 데이터 타입 변경
    - 주소 및 업종 분류 : [contains_address_isin_restaurant.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/contains_address_isin_restaurant.ipynb) 
        - 해당 주소가 아닌 장소 걸러내기, 음식점 아닌 곳 제외하기 
        
3. EDA
    - 기술 통계 및 분포 분석 : [EDA_nolimit.ipynb](https://github.com/hmii/map_scrapping_project/blob/master/EDA_nolimit.ipynb)
