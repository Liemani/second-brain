# Voltage

## Question

AI node 내부에서 `voltage`를 실제 상태값처럼 둘지, 단순한 누적 입력값으로 둘지 결정해야 합니다.

## Points

- voltage를 뉴런의 현재 상태로 본다면 시간 축이 중요해집니다.
- voltage를 단순 합산값으로 본다면 일반적인 weighted sum과 가까워집니다.
- biological inspiration을 얼마나 반영할지 먼저 정해야 합니다.

## Consider

- 입력 신호 누적 방식
- threshold와의 관계
- decay가 필요한지 여부
- discrete step 기반인지 continuous update 기반인지

## Next

- 가장 단순한 voltage model 하나 정의
- decay가 있는 모델과 없는 모델 비교
