# Data_Science
동국대 X 부스트코스 코칭스터디 데이터사이언스

## 비서울권 관광 인프라와 방문자 수의 상관 관계 분석

> Hyphothesis : 외부 방문자 수가 많은 지역은 관광 인프라도 많이 조성되어있을 것이다.
> > 외부 방문자 수와 관광 인프라의 상관 계수가 높을 것으로 예상
```

1. 전국 기초지자체 방문자 수 수집 및 전처리

2. 외부 방문자 수 기준으로 상위 15개 지역, 하위 15개 지역 추출

3. 서울을 제외한 지역의 관광데이터를 수집 및 전처리 진행

4. 관광 인프라["관광지", "문화시설", "축제공연행사", "여행코스", "레포츠", "숙박", "쇼핑", "음식점"]를 분석

5. 상위 15개 지역의 관광 인프라의 공통점 및 차이점들을 비교 분석한 후 하위 15개 지역과 비교하여 결론을 도출

6. 상관계수를 구하여 상관 관계를 추출
```

### 전처리 과정
![preprocessing](https://user-images.githubusercontent.com/73403038/129845826-07d9aa23-667d-4eaa-828b-dbb359f164c7.png)


### 참고사항
```
관광 데이터의 관광 인프라를 분석할 때 주소 데이터의 오류가 많아 절대적인 기준인 위경도를 카카오맵 API를 이용하여 자세한 행정구역을 추출
```

## 결론
> 각 지역의 외부 방문자 수와 해당 지역 관광 인프라 수의 상관 관계가 명확하지 않음
> > 관광 인프라만으로 결론 도출이 어렵기에 다른 부가적인 요소의 작용이 크다고 판단 
> > -> 관광객 수 증진 요소들에 대한 추가적인 분석이 필요함

--------------------------------------------------

### 추가 분석
![visit_reason](https://user-images.githubusercontent.com/73403038/129849892-0bc2689d-f5d1-42cf-8b88-fa24c0c9ad50.jpg)

- 문화체육관광부 2019 국민여행조사에 의하면 국내의 경우, 볼거리 즉, 관광 인프라도 관광객수 증진에 중요한 역할을 하지만, 여행지 지명도, 즉 해당 관광목적지의 브랜드 가치가 주요함을 알 수 있음.
 - 따라서, 단순히 관광지 진흥을 위해선 관광 인프라 마련 뿐 아니라  관광정책, 지역 홍보 및 장소마케팅이 더욱 중요함을 알 수 있음.



---------------------------------------------
### 데이터셋 출처
- [한국관광데이터랩(외부관광객수)](https://datalab.visitkorea.or.kr/datalab/portal/bda/getLocgoAna.do)

- [TourAPI3.0 사이트(관광인프라수집)](https://api.visitkorea.or.kr/search/galleryList.do)

- [DBPia_참고논문](https://www.dbpia.co.kr/Journal/articleDetail?nodeId=NODE01642617)
  * 김태헌, 박숙진 (2011). 지역경제 활성화를 위한 관광자원개발과 관광정책의 역할. 한국콘텐츠학회논문지, 11(5), 403-412
    * 관광인프라가 지역경제활성화에 유의한 영향을 미칠 것이라는 가설 기각
 

  * 아무리 우수한 관광자원을 갖고있다 하더라도 관광정책이 구체적으로 시행되지 않으면 무익하다는 결론 도출
  * 즉, 관광지 활성화에 있어서 지역관광자원보다는 해당 지역의 관광 사업을 지원하는 정책적인 지원이 더 큰 영향을 미침.
