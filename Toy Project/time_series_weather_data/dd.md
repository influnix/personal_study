아래는 실제로 다운로드 가능한 공개 날씨 데이터를 활용하고, 해당 날짜를 기준으로 **synthetic(합성) 판매 데이터**를 생성하여 merge하는 코드 예시입니다.

> 참고:
> 
> - 날씨 데이터는 [Daily Minimum Temperatures in Melbourne](https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-min-temperatures.csv)를 사용합니다.
> - 판매 데이터는 날씨 데이터를 기반으로 간단한 가정(기온, 프로모션 여부 등)을 반영하여 합성합니다.
