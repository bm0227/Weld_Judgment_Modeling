## 전압, 전류데이터를 통한 용접판단 모델링

## 1. 로봇용접 정상/결함 자동 분류 분석

작업자의 수정용접으로 인한 작업 MH Loss와 예상치 않은 로봇 가동률의 증가가 발생하기 때문에 이를 해결하기 위해 데이터를 분석함

## 2. 데이터 가공

불필요한 데이터를 제거하고 불량 데이터들을 다시 라벨링 및 결측치 처리

파생변수로 저항과 온도를 저항의 경우에는 로그처리하여 0~1 사이의 값으로 온도는 전압x전류로 추가함

## 3. 모델링

모델링의 경우에는 2차례로 나누어서 진행함. (전처리 전후)

전처리 전의 모델은 최대 71%의 성능을 보이며 XGB가 가장 정확도가 높음

전처리 후의 모델은 랜덤 포레스트가 약 92%의 정확도를 보이며 가장 성능이 좋음


## 4. 결론

용접의 특징을 파악하여 파생변수를 만든 것이 성능 향상에 큰 역할을 하였으며

다양한 모델을 적용해보고 하이퍼 파라미터를 통하여 정확도를 향상시킴
