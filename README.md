# google_naver_map_rating_analysis
네이버 및 구글 지도의 음식점 별점 비교 분석

## 개요
포털사이트에서 제공하는 음식점 별점은 과연 믿을 만 한 것인지 네이버와 구글 지도에서 별점을 수집하여 비교하여 분석해보다


## 프로젝트 설명
- 같은 음식점을 대상으로 각 사이트에서 제공하는 방문자수, 리뷰수, 별점 비교
```
- 플랫폼 : NAVER, GOOGLE
- 지역 : 제주도 애월읍, 성산읍 
- 대상 : 해당 지역 내 음식점 전체 
```
- 네이버는 구글보다 별점이 전반적으로 상향 평준화된 결과가 나왔다. 
- 평균 0.4점이 높았으며, 4.0이상인 음식점이 네이버는 97.5%  구글은 64.7% 였다. 

## 프로젝트 과정
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
