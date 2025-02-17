> 참고:
> 
> - 날씨 데이터는 [Daily Minimum Temperatures in Melbourne](https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-min-temperatures.csv)를 사용합니다.
> - 판매 데이터는 날씨 데이터를 기반으로 간단한 가정(기온, 프로모션 여부 등)을 반영하여 합성합니다.

- **프로젝트 주제:**
    - **데이터 융합:**
        - 멜버른의 일일 최저 기온 데이터를 활용해, 동일한 날짜 범위를 기준으로 합성 판매 데이터를 생성하고 두 데이터를 날짜를 기준으로 병합.
    - **합성 판매 데이터 생성:**
        - 판매량은 기온, 프로모션 여부, 그리고 잡음(noise)을 반영해 생성되었으며, 강수량 또한 랜덤으로 추가.
    - **모델링:**
        - 기온(`temp`), 강수량(`rainfall`), 프로모션 여부(`promotion_flag`)를 주요 피처로 사용해 RandomForestRegressor를 적용하였고, 시계열 특성을 고려해 날짜순으로 학습 및 테스트 세트를 구분.
