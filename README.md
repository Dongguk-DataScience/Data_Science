# Data_Science
동국대 X 부스트코스 코칭스터디 데이터사이언스

## 비서울권 데이터 관광 인프라 분석
```

```

## 관광지 성공 및 실패 사례 분석을 통한 관광지 인프라 분석(ReBuilding 전)
![extract_density](https://user-images.githubusercontent.com/73403038/129029282-b557ad0b-50e4-4536-8200-0249490789dd.png)
```
1. 전국 숙박 업소 현황 데이터 수집

2. 전국 숙박 업소 데이터의 밀도 확인

3. 높은 밀도를 보이는 상위 15개 지역, 낮은 밀도를 보이는 하위 15개 지역 추출

4. 상위 15개 지역과 하위 15개 지역의 관광 인프라 분석

이유 : 지역마다 행정 구역 체계가 달라서 기준이 명확하지 않고 데이터 정제가 쉽지 않다. -> 절대적인 기준인 위경도를 사용하려고 했지만 위경도 데이터의 부재로 인해 힘듦
읍면동에서 -> 시 구로 늘림. 지역마다 구의 크기가 차이가 있기 때문에 애매하다., 
지자체 별로 데이터 수집 방식이 바르고 제공되는 데이터의 수도 천차만별이기에 기존의 수입한 자료는 지역별로 양적 질적 신뢰성을 저하시킨다.
-> 호텔 밀도 대신에 해당 지역에 방문한 외부 방문자 수를 새로운 기준으로 잡아보자
해결책 : 위경도라는 절대적인 기준에 부합하는 자료가 필요했고 동일한 카테고리를 수집된 자료가 필요했다.-
```


### 데이터 출처
- [전국 숙박업소 현황 데이터](https://www.mcst.go.kr/kor/s_policy/dept/deptView.jsp?pCurrentPage=1&pType=05&pTab=01&pSeq=1462&pDataCD=0417000000&pSearchType=01&pSearchWord=%EC%88%99%EB%B0%95)
- [KOSIS](https://kosis.kr/statHtml/statHtml.do?orgId=210&tblId=DT_GRDP002&conn_path=I3)
- [전국관광지정보표준데이터](https://www.data.go.kr/data/15021141/standard.do)

