---
status: "Open"
created: "2026-06-12"
---

# custom ai

아래 레벨부터 직접 구현하는 custom AI 아이디어다.

## Notes

- 높은 수준의 라이브러리를 사용하는 것보다, 가능한 한 아래 레벨부터 직접 구현하며 이해하는 custom AI 아이디어다.
- node 단위부터 시작해 전체 구조를 스스로 설계하는 방향을 전제로 한다.

### Main Topics

- activation 계층을 어떻게 해석하고 구성할지
- voltage 또는 내부 상태를 어떤 모델로 둘지
- neural network 구조를 어떤 방식으로 설계할지
- 학습을 gradient 기반, local rule, reinforcement 성격 중 무엇으로 이끌지
- 실시간 처리를 tick 기반 또는 event-driven 방식으로 어떻게 풀지

### Focus

- 단순 사용보다 직접 구현 중심으로 접근한다.
- 각 요소를 독립적으로 실험하고 이후 하나의 시스템으로 통합한다.
- 추상 개념보다 실제 동작 가능한 모델을 우선한다.

### Activation

- activation은 `voltage`나 입력 누적값이 실제 출력 신호로 바뀌는 구간이다.
- 입력 신호와 내부 상태를 어떤 식으로 다룰지 정리해야 한다.
- activation 단계에서 어떤 함수를 사용할지 결정해야 한다.
- activation을 단순 임계값 통과로 볼지, 연속적인 출력 변환으로 볼지, 시간 축이 있는 상태 변화와 연결할지 검토한다.
- voltage와 activation의 역할을 분리해서 정의한 뒤, activation function 후보를 비교한다.

### Activation Function

- 활성 함수는 node의 출력 방식과 학습 안정성에 직접 영향을 준다.
- 후보로는 sigmoid, tanh, ReLU, leaky ReLU, step function, custom threshold function이 있다.
- 미분 가능성이 필요한지, 출력 범위를 제한할 필요가 있는지, sparse activation이 중요한지, biological model과 유사성을 추구할 것인지 검토한다.
- 초기 구현은 step function과 ReLU를 우선 비교하고, 이후 학습 방식에 맞춰 sigmoid 또는 tanh 필요성을 재검토한다.

### Voltage

- AI node 내부에서 `voltage`를 실제 상태값처럼 둘지, 단순한 누적 입력값으로 둘지 결정해야 한다.
- voltage를 뉴런의 현재 상태로 보면 시간 축이 중요해진다.
- voltage를 단순 합산값으로 보면 일반적인 weighted sum과 가까워진다.
- biological inspiration을 얼마나 반영할지 먼저 정해야 한다.
- 입력 신호 누적 방식, threshold와의 관계, decay 필요 여부, discrete step 기반인지 continuous update 기반인지 검토한다.
- 가장 단순한 voltage model 하나를 정의하고, decay가 있는 모델과 없는 모델을 비교한다.

### Neural Network Structure

- 어떤 구조의 neural network를 만들지 먼저 정해야 전체 구현 범위가 정리된다.
- 후보는 단일 layer perceptron, 다층 feedforward network, recurrent structure, event-driven node network, fully custom graph structure다.
- node 연결을 고정된 layer로 볼지 그래프로 볼지, feedback loop를 허용할지, 시간 개념을 구조에 포함할지, 실험용 최소 구조를 어디까지로 잡을지 검토한다.
- 가장 먼저는 단순 feedforward 구조를 구현하고, 이후 recurrent 또는 event-driven 확장 가능성을 본다.

### Training

- 학습을 전통적인 gradient 기반으로 할지, 규칙 기반 또는 실험적 방식으로 할지 결정해야 한다.
- 능동 학습은 시스템이 스스로 탐색하고 상호작용하며 학습하는 방식이다.
- 수동 학습은 주어진 데이터나 정답을 기반으로 학습하는 방식이다.
- 후보는 backpropagation, local update rule, Hebbian-like learning, reinforcement-style feedback, evolutionary search다.
- activation function이 미분 가능한지, 각 node가 local state를 갖는지, 목표가 정확도인지 구조 이해인지, 학습 속도와 구현 난이도 사이의 균형이 어떤지 검토한다.
- baseline으로 단순 supervised training 가능 여부를 확인하고, custom node model에 맞는 local rule도 병행 검토한다.

### Active Learning

- 능동 학습은 시스템이 어떤 입력을 더 볼지, 어떤 행동을 시도할지 스스로 결정하는 방향의 학습이다.
- exploration을 얼마나 허용할지, feedback를 어떤 형태로 받을지, 실시간 처리와 어떻게 연결할지, reward 또는 signal을 어떻게 정의할지 검토한다.
- 작은 환경에서 선택과 피드백 루프를 먼저 실험하고, node 기반 구조와 결합 가능한지 확인한다.

### Passive Learning

- 수동 학습은 외부에서 주어진 데이터, 정답, 또는 고정된 입력 흐름을 바탕으로 학습하는 방식이다.
- supervised dataset을 사용할지, 입력과 정답의 형식을 어떻게 정의할지, batch 기반으로 처리할지 stream 기반으로 처리할지, baseline 성능 측정에 적합한지 검토한다.
- 가장 단순한 입력-출력 매핑 문제부터 실험하고, 이후 능동 학습과 비교 가능한 기준을 만든다.

### Real Time Processing

- 실시간 처리는 입력이 계속 들어오는 상황에서 node와 network를 어떻게 업데이트할지의 문제다.
- 입력 스트림을 frame 단위로 처리할지 event 단위로 처리할지, 전체 network를 매 tick마다 갱신할지 변화가 있는 node만 갱신할지, latency와 accuracy 중 무엇을 우선할지, state synchronization이 필요한지 검토한다.
- tick-based simulation, event-driven update, hybrid approach를 설계 방향으로 둔다.
- 가장 단순한 tick-based loop부터 구현하고, 이후 event-driven 최적화 가능성을 검토한다.
