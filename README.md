# 제1회 2023년 지역 치안 안전 데이터 분석 공모전
이 프로젝트는 "제1회 2023년 지역 치안 안전 데이터 분석 공모전"에서 우수상을 수상한 데이터 분석 프로젝트입니다. 프로젝트의 목적은 지역 치안과 안전에 관련된 데이터를 분석하여 유의미한 통찰력과 인사이트를 도출하는 것입니다.

저희 팀은 다양한 방법을 활용하여 데이터를 분석하였습니다. 프로젝트에서는 Python 프로그래밍 언어와 다양한 데이터 분석 라이브러리를 활용하여 종합적인 분석 작업을 수행하였습니다.

데이터 분석에는 다양한 도구와 기술을 사용하였습니다. 먼저, HDBSCAN 알고리즘을 이용하여 사고 발생 지점의 위도 경도 좌표 데이터를 군집화하여 HOTSPOT을 확인하였습니다. 이렇게 군집화된 결과를 Folium 라이브러리를 이용하여 지도 상에서 지역별 교통사고의 밀도를 시각화하였습니다.

또한 QGIS를 활용하여 50M * 50M의 GRID를 생성하고, 이를 연도, 계절, 요일, 밤/낮 요인과 같은 다양한 변수로 구분하여 시각화하였습니다. 이를 통해 시계열 데이터를 분석하고, 유사한 패턴과 트렌드를 가진 데이터끼리 군집화하여 분석하였습니다.

TIBCO Spotfire와 QGIS를 사용하여 데이터를 시각적으로 탐색하고 공간 분석을 수행하였으며, Folium을 활용하여 Python에서 대화형 지도 시각화를 구현하였습니다. 이러한 다양한 기술과 도구의 활용을 통해 효과적인 데이터 분석과 인사이트 도출에 기여하였습니다.

그리고, 저희는 해당 지역의 기상 정보를 수집하고 이를 기존의 사고 데이터와 통합하여 모델을 학습시켰습니다. 이 모델은 특정 기상 조건이나 패턴이 사고 발생과 관련이 있다는 인사이트를 제공하며, 미래에 발생할 수 있는 사고에 대한 예측을 수행할 수 있습니다.

이렇게 기상 정보를 포함한 다양한 데이터를 활용하여 사고 발생 예측 모델을 개발하였으며, 이 모델을 통해 사고 예방 및 대응 전략을 수립하는 데에 기여하고자 합니다.
본 프로젝트에서 우리 팀은 지역 치안 문제를 데이터로부터 탐색하고 해결책을 제시하는 분석 능력을 발휘하였으며, 우수한 결과를 도출하여 공모전에서 우수상을 수상하였습니다.

이 README 문서는 프로젝트의 개요와 목적, 사용된 기술 및 도구, 결과 요약 등을 제공하여 프로젝트에 대한 간략한 소개를 제공하고자 합니다.

본 프로젝트는 다른 분석가들이 지역 치안과 안전에 대한 데이터 분석을 진행하거나 관련된 연구를 수행할 때 참고할 수 있는 유용한 자료가 될 것입니다.
## 공모전 개요
  - <b>공모전 명칭</b>: 제1회 2023년 지역 치안 안전 데이터 분석 공모전
  - <b>목적</b>: 이 공모전은 지역 치안과 안전에 대한 데이터 분석 능력을 검증하고, 유의미한 인사이트를 도출하여 지역의 치안 정책 수립 및 안전 개선에 기여하는 것을 목표로 합니다.
  - <b>주최</b>: 경찰대학교 치안정책연구소(스마트치안지능센터)
  - <b>대회 일정</b>:
    - 공모기간 : 2023/1/20 ~ 2023/2/15
    - 심사기간 : 2023/2/16 ~ 2023/2/23
    - 최종발표:  2023/2/24
    - 시상식 : 2023/2/28
  - <b>제공되는 데이터</b> 
    - KP2020, KP2021, NPA2020
      - 이 사고가 일어나고 사건 신고가 일어난 데이터
      - 사건유형, 날짜, 시간, 경도, 위치 등등의 정보 보유 
  - <b>공모전 사이트</b> : https://www.bigdata-policing.kr/board/b_contest/view?idx=167&category=
  - <b>개최안</b> : [공모전 개최(안).pdf](https://github.com/passion3659/2023_Crime_Safety_Data_Analysis_Competition/files/11648459/default.pdf)

## 공모전에서의 팀의 역할과 기여
- <b>팀 구성</b>
  - 팀명 : 강양이 방범대
  - 팀장 : 양정열
  - 팀원 : 강훈, 이승준, 이채원
- <b>분석 배경</b>
  - 본 프로젝트에서는 스마트 치안 빅데이터 플랫폼에서 제공한 데이터를 활용하여 충남, 세종, 대전의 교통사고 발생 현황을 분석하고 교통사고를 선제적으로 예측할 수 있는 모델을 생성한다. 
  - 교통사고와 관련된 데이터를 수집하여 교통사고 Hotspot을 분석하고, 주요 Hotspot의 교통사고 발생을 예측한다.
- <b>본 팀에서의 기여</b>
  - HDBSCAN을 활용한 사고 발생 지점의 군집화와 HOTSPOT 확인
  - Folium을 통한 지역별 교통사고 밀도 시각화
  - QGIS를 이용한 GRID 생성과 시계열 데이터 분석 및 군집화
  - 시계열 데이터를 바탕으로한 사건 발생 패턴 파악과 예방/대응 전략 도출(time-series clustering)
  - hotspot별 기상데이터를 수집후 over-sampling과 feature extraction 후 randomforest classifier를 이용한 model 구축
