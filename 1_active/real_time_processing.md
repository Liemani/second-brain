# Real Time Processing

## Question

실시간 처리는 입력이 계속 들어오는 상황에서 node와 network를 어떻게 업데이트할지의 문제입니다.

## Consider

- 입력 스트림을 frame 단위로 처리할지 event 단위로 처리할지
- 전체 network를 매 tick마다 갱신할지, 변화가 있는 node만 갱신할지
- latency와 accuracy 중 무엇을 우선할지
- state synchronization이 필요한지

## Design Direction

- tick-based simulation
- event-driven update
- hybrid approach

## Next

- 가장 단순한 tick-based loop부터 구현
- 이후 event-driven 최적화 가능성 검토
