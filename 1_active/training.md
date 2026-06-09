# Training

## Question

학습을 전통적인 gradient 기반으로 할지, 규칙 기반 또는 실험적 방식으로 할지 결정해야 합니다.

## Learning Modes

- [active_learning.md](active_learning.md): 시스템이 스스로 탐색하고 상호작용하며 학습하는 방식
- [passive_learning.md](passive_learning.md): 주어진 데이터나 정답을 기반으로 학습하는 방식

## Options

- backpropagation
- local update rule
- Hebbian-like learning
- reinforcement-style feedback
- evolutionary search

## Consider

- activation function이 미분 가능한가
- 각 node가 local state를 갖는가
- 목표가 정확도인지 구조 이해인지
- 학습 속도와 구현 난이도 사이의 균형

## Next

- baseline으로 단순 supervised training 가능 여부 확인
- custom node model에 맞는 local rule도 병행 검토
