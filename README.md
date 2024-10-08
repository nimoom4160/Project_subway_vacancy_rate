# 🚉 지하철 공실률 해결을 위한 현황 파악

✅**한 줄 소개**</br>지하철 상가 공실 현황을 분석하고 지하철 이용객들에게 더욱 편리한 상가 시설을 제공하는 방향으로 프로젝트가 진행됩니다.
</br>
</br>
✅**기간**</br>2023.10 ~ 2023.11
</br>
</br>
✅**맡은 역할**</br>역별 공실률 막대 그래프 시각화, 상관분석 및 회귀분석, 연령대별 출발 및 도착 시군구에 대한 연관분석 실시
</br>
</br>
✅**팀원**</br>3명
</br>
</br>
✅**사용 툴**</br>R
</br>
</br>
✅**분석 방법**</br>상관/회귀, 시각화, 연관분석
</br>
</br>
✅**수상명**</br>대상
</br>
</br>

## 📈 분석 요약

 지하철을 이용하는 사람들이 많아지면서 상가를 이용하는 사람들도 증가하고 있습니다. 그러나 ‘지하철 역사 내 상가 공실률은 어떨까?’라는 궁금증으로 시작하여 본 연구는 서울시 인구 이동 데이터를 활용하여 지하철 역사 내 상가 공실 현황을 조사하고자 하였습니다.

 이번 연구는 지하철 역사 내 상가 공실 현황을 조사하고, 이를 통해 상가 업체들이 더욱 효율적으로 운영할 수 있도록 도움을 주고자 하는 목적을 가지고 있습니다. 이를 통해 지하철 역사 내 상가 공실률을 낮추고, 지하철 이용객들에게 더욱 편리한 상가 시설을 제공할 수 있을 것으로 기대됩니다.
</br>
</br>

## 🧐 연구 배경

 코로나가 시작한 이후부터 지하철 역사 내 상가는 꾸준한 하락세를 보이고 있으며, 유동인구가 많았던 서울 지하철 상가가 8년 동안 25%나 줄었습니다. 

 따라서 지하철 공사의 적자 해결과 상가의 폐업을 막을 수 있는 방법을 고민하게 되었고, 지하철 상가와 지하철 이용 데이터 등을 분석해 해결 방안을 찾아보고자 했습니다.
</br>
</br>
## ✏️ 분석 내용

### 사용한 데이터

 사용한 데이터는 서울시 지하상가 임대정보 데이터, 지하철 승객 데이터, 서울시 생활이동 데이터입니다.

 지하상가 데이터와 승객 데이터를 이용하여 **공실률의 내부적인 원인**을 살펴보고, 서울시 생활이동 데이터를 이용하여 **외부적인 원인**을 파악했습니다.
</br>

### 시각화

 지하철 상가의 공실 현황을 알아보기 위해 서울시 지하상가 임대정보 데이터를 이용하여 상가 유형 비율과 공실률 등을 시각화했으며, 지하철 승객 데이터를 이용하여 노선별 공실률과 무임승차 비율을 살펴보았습니다.

 또한 유동인구 데이터를 이용하여 연령대별 인구수와 지역별 이동빈도를 시각화했습니다.
</br>

### 상관분석 및 회귀분석

공실률을 종속변수로 하여 임대료 및 상가면적 간의 상관관계와 인과관계를 파악했습니다.
</br>

### 연관분석

유동인구 패턴과 같은 외부적인 요인에도 초점을 맞추어, 특정 자치구에서 출발하면 특정 자치구로 가는 패턴이 많이 보일 것이라는 규칙을 기대하여 연관분석을 진행했습니다.
</br>

### 업종 추천

위 분석 내용들을 바탕으로 자치구 한 곳을 선정한 후 공실률을 줄이기 위한 상가 업종을 추천하고자 하였습니다.
</br>
</br>

## 📝 분석 결과

### 서울시 지하상가 임대정보 데이터, 지하철 승객 데이터

**시각화**

![2  전체 지하철 상가 중 공실 비율 시각화](https://github.com/user-attachments/assets/e34945fc-bf21-48bc-9136-ddd6e950efb0)

전체 지하철 상가 중 공실 비율 시각화

![1  지하철 상가 공실률 지도 시각화](https://github.com/user-attachments/assets/c2c34c97-d7ac-49af-915b-f2a80b86ece4)

지하철 상가 공실률 지도 시각화

전체 지하철 상가 중 공실은 19.8%로 꽤 높은 비중을 차지했으며, 지도 시각화에서 점의 분포를 통해 공실률이 70%를 넘는 지역도 볼 수 있었습니다. 또한 서울을 서부/동부/남부/북부/중부 총 5개 구역으로 나누었을 때, 전반적으로 중부 지역의 공실률이 38.1%로 가장 높았습니다.

![3  노선별 공실률과 무임승차 비율](https://github.com/user-attachments/assets/a838b535-5b3a-41c6-9783-42c16f00f815)

노선별 공실률과 무임승차 비율

![4  역별 공실률](https://github.com/user-attachments/assets/51ede340-57e0-43ae-9162-984713e8de21)

역별 공실률

노선별 공실률과 무임승차 비율이 관련 있는지 보기 위해 시각화한 결과, 두 변수는 비례하지 않다는 점을 알 수 있었습니다. 역별 공실률의 경우 1호선 동대문역과 6호선 광흥창역, 4호선 미아역이 차례대로 높게 나타났습니다.
</br>

**상관분석 및 회귀분석**

![5  회귀분석 그래프](https://github.com/user-attachments/assets/93469696-6f51-4552-8841-5029ec301314)

임대료 및 상가면적과 공실률 간의 관계를 산점도로 나타냈습니다. 산점도를 통해서는 음의 관계를 나타내지만, 상관분석 결과 임대료와 공실률의 상관계수는 -0.397, 상가면적과 공실률의 상관계수는 -0.305로 약한 음의 선형 관계를 나타냈습니다. 즉, **임대료와 공실률, 상가면적과 공실률 모두 상관성이 낮다**고 판단했습니다.

![6  독립변수 임대료, 종속변수 공실률](https://github.com/user-attachments/assets/7e0c3b72-22af-4ce3-b8f6-0fc4e51d5c70)

독립변수 : 임대료, 종속변수 : 공실률

![7  독립변수 상가면적, 종속변수 공실률](https://github.com/user-attachments/assets/a3671a55-f83a-4e08-9f2f-c253a04983d5)

독립변수 : 상가면적, 종속변수 : 공실률

임대료 및 상가면적과 공실률 간의 회귀분석을 실시한 결과, p-value가 모두 0.05보다 작았지만 R-squared 값이 매우 작아 설명력이 좋지 않았습니다. 또한 회귀분석의 기본 가정인 선형성과 정규성, 등분산성을 만족하지 않았습니다.

따라서 임대료와 상가면적 등의 **내부적인 요인들은 공실률과 큰 연관이 없다**고 판단하였고, 유동인구 패턴과 같은 외부적인 요인에 중점을 두어 직관적인 패턴 분석을 진행하였습니다.
</br>

### 유동인구 데이터

**시각화**

![8  유동인구 시각화](https://github.com/user-attachments/assets/9c369149-03f3-4433-b3ff-44ba130e24ce)

연령대별 인구 수를 시각화한 결과, 20~30대가 가장 많았고 이동 유형에서는 직장 외의 위치(E)에서 집으로 가는 인구가 많았습니다.

**연관분석**

연관분석 결과 강북구에서 출발하여 도봉구에 도착하는 경우, 송파구에서 출발하여 강동구에 도착하는 경우, 양천구에서 출발하여 강서구에 도착하는 경우 순서대로 향상도가 높게 나타났습니다.

연령대별로 나누어 지역별 관계를 살펴본 결과, 자치구 이동 패턴이 매우 상이한 점을 관찰할 수 있었습니다.

**공실률을 줄일 수 있는 최적의 업종 추천**

1. 업종 추천을 위한 자치구 선정 : 지하철 상가 공실률 지도 시각화에서 중부의 공실률이 가장 높았으므로 서울에서 **중부**로 범위를 좁혔습니다.

![8  지역 이동 빈도](https://github.com/user-attachments/assets/6c68b931-d685-44b4-9a03-56a8e5b47706)

이후 사람들의 이동이 많은 출퇴근 시간대에 중부에 속하는 자치구들이 목적지인 경우를 살펴본 결과, 전반적으로 **용산구가 출퇴근 시간대 모두 이동 빈도가 높아** 업종 추천을 위한 자치구로 용산구를 선정했습니다.

1. 용산구의 특징 : 용산구는 여성과 남성의 비율 차이가 거의 없고 20대 중반에서 30대 중반의 사람들이 많습니다. 또한 평균 이동 시간은 40분에서 60분 사이이며, 출퇴근 시간대에 인구가 가장 몰립니다.

1. 업종 추천 
    - 성별 비율 차이가 거의 없으므로 **성별에 관계 없이 청년층에게 수요가 높은 드럭스토어와 꽃집** 등을 추천할 수 있습니다.
    - 청년층이 많은 용산구에는 중년층에 비해 경제적 여유가 없는 **청년층을 타깃으로 한 천원숍이나 SPA 브랜드와 같은 저가형 브랜드**를 추천할 수 있습니다.
    - 평균 이동 시간이 긴 사람들이 앉아서 쉴 수 있고 청년층이 부담 없이 갈 수 있는 **저가형 프렌차이즈 카페**를 최적의 업종으로 추천할 수 있습니다.
</br>
</br>

## 📝 결과 활용

- 지하철 상가 공실률 감소로 얻게 된 임대료를 철도 회사의 적자 감소에 활용함으로써 철도 회사에 이익이 될 수 있습니다.
- 각 지역의 특성에 맞는 업종을 추천함으로써 해당 지역에 거주하는 고객의 니즈에 맞는 상권을 형성할 수 있습니다.
- 지하철 이용객의 연령과 성별을 고려한 상가는 역사 내 상가의 다양성과 경쟁력을 증가시킬 수 있습니다.
</br>
</br>

## 😀 성장 경험

- 지하철 공실의 원인을 내부적인 원인과 외부적인 원인으로 나누어 심층적으로 살펴볼 수 있었습니다.
- 공실률에 대한 전반적인 현황을 바탕으로 공실률 감소를 위한 업종을 추천함으로써, 공실률 문제를 해결하는 인사이트를 도출할 수 있었던 유익한 프로젝트 경험이었습니다.
</br>
</br>

## 😅 아쉬운 점

- 지하철 공실률을 대상으로 하는 분석이므로, 대중교통 이용 데이터를 활용한다면 유동인구 데이터보다 더 정확한 결과를 얻을 수 있었을 것입니다.
- 신용카드 데이터 등의 소비 데이터를 활용한다면 업종 추천에 대한 신뢰도가 올라갈 것입니다.
