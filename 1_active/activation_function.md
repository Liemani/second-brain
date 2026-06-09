# Activation Function

[activation.md](activation.md) 아래에서 activation의 구체적인 출력 함수를 정리합니다.

## Question

활성 함수는 node의 출력 방식과 학습 안정성에 직접 영향을 줍니다.

## Candidates

- sigmoid
- tanh
- ReLU
- leaky ReLU
- step function
- custom threshold function

## Consider

- 미분 가능성이 필요한가
- 출력 범위를 제한할 필요가 있는가
- sparse activation이 중요한가
- biological model과 유사성을 추구할 것인가

## Next

- 초기 구현은 step function과 ReLU를 우선 비교
- 이후 학습 방식에 맞춰 sigmoid 또는 tanh 필요성 재검토
