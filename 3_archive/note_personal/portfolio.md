## (주)바인드소프트, 연구원

2023/08/29 ~ 현재

### Cortex-M4 교육 커리큘럼 제작

#### brief

- duration : 미정 (2024/09 ~ 현재)
- goal : 대학 강의에 사용 가능한 Cortex-M4 교육 커리큘럼 제작
- language : C
- team size : 1명

#### detail

- 장비 : CNDI mCube-Cortex M4 (STM32F407VGT6)
- GPIO, ADC, Timer, PWM, UART, WiFi

### Edge플랫폼 실시간 신호 처리 모듈 개발

#### brief

- duration : 2달 (2024/08 ~ 2024/09)
- goal : Jetson Orin Nano에서 SPI를 통신으로 2byte 데이터를 20kHz로 샘플링
- language : C++
- team size : 2 명

#### detail

- result : 샘플 사이에 알 수 없는 delay로 인해 요구사항 충족 실패, 해당 성능을 위해서는 os 수준에서 문제 분석 필요

### Mobius 기반 IoT 시스템 유지관리

#### brief

- duration : 3 달 (2024/01 ~ 2024/04)
- goal : 기존 시스템 문서화 및 기능 확장
- language : Javascript
- team size : 1 명

#### detail

- Windows 10에서 Mobius 플랫폼 구축 매뉴얼 작성
- 아두이노 및 라즈베리파이 연동 매뉴얼 작성

## Tiny Home 앱 개발

2023/05/03 ~ 2023/07/23

- 목표: iOS 에서 동작하는 게임 만들기
- GitHub: https://github.com/Liemani/a-month-game
- language: Swift
- environment: Xcode, Git, Vim, Numbers, Gimp
- framework: SpriteKit, CoreData
- team size : 1 명
- total code line : 5036

상세 구현
- 생성형 오픈 월드
- 멀티 터치 구현
- 아이템 스케쥴러

하나의 앱을 만들어 보았습니다.
객체의 내부 작동과 외부 호출을 분리시키는 연습



## haven and hearth 클라이언트 개조

![liefeni.png](/image/liefeni.png)

2022/07/29 ~ 2022/09/23

- 목표: 매크로 기능 구현하기
- GitHub: https://github.com/Liemani/liefeni
- language: Java
- environment: Vim, Git
- team size : 1 명
- total code line : 5094

상세 구현
- 커맨드 라인으로 명령을 입력받아서 설명을 출력하거나 매크로를 실행하는 기능
- 프로그램을 분석하여 원하는 데이터를 가져와 따로 보관하는 기능
- 원하는 동작을 위해 서버에 전달해야 하는 명령을 분석
- 캐릭터 이동 기능 구현
- 물건 들고 내려놓는 기능 구현
- 최종적으로 어질러져 있는 오브젝트를 차곡차곡 정리하는 매크로 구현

제가 좋아하는 이 게임은 매크로 개발 문화가 발달해 있습니다.
저는 기존에 유저가 만든 매크로 api 의 한계를 극복하고 싶었습니다.
그래서 오픈되어 있는 클라이언트 소스를 수정하기로 했습니다.

기존 매크로는 상태 변화를 변하는 순간 인식하는 것이 아니라 일정 시간마다 상태를 추적하여 변화했는지 여부를 판단하였습니다.
때문에 이미 상태가 변했는데도 다음 추적 싸이클이 돌아오기까지 딜레이가 있습니다.
그리고 한 추적 싸이클 안에 상태가 여러 번 변하는 것을 감지하지 못하는 문제도 있습니다.
이런 문제를 해결하기 위해, 서버로부터 원하는 메세지를 받을 경우 바로 상태 변화를 적용하도록 작성했습니다.



## [이노베이션 아카데미] 42 Seoul 교육 과정

2020/12/25 ~ 2022/06/20

### webserv

2022/04/11 ~ 2022/06/20

- 목표: 기초적인 기본 함수들로 HTTP protocol 을 준수하는 web server 를 만드는 42 프로젝트
- language: C++98
- environment: Vim, Git, atlassian jira
- team size : 총 3 명
- total code line : 3583

참조 문서
- RFC7230 등
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

상세 구현
- 서버 실행 시 config 파일을 읽고, 거기에 서술된 기능을 수행하도록 구현
- kevent 를 사용하여 이벤트 중심으로 동작하도록 구현

내가 맡은 부분
- 서버에 연결하여 임의의 텍스트 메세지를 전송하고 응답을 출력하는 테스트용 클라이언트 프로그램 작성
- 실제 서버 프로그램인 nginx 에 다양한 request 를 전송하여 그에 따른 response 분석
- socket fd 로 데이터를 읽고 적절한 response 를 전송
- test case 작성 및 테스트

초기에는 팀원과 함께 프로그램의 구조를 잡았습니다.
그리고 config 파일 처리, 이벤트 구조 설계, 입출력 처리의 3 부분으로 나누어 맡아 각자 개발을 진행했습니다.
다른 두 팀원이 다른 프로젝트를 병행하여 작업이 더디게 진행되어 아쉬웠습니다.
구현 범위를 결정하는 등의 선택 사항의 경우, 다수의 팀원이 만족하거나 다른 팀원을 설득하는 방식으로 진행되었습니다.
지식이 부족해 선택이 애매한 경우에는 한 명씩 돌아가면서 원하는 방식을 적용했습니다.
가령 이슈 트래커로 jira 를 쓸지 말지에 대해 제가 쓰고 싶다고 하여 제 의견이 반영되었고, 전역 변수를 쓸까 말까에 대해서는 다른 팀원의 의견을 반영하여 가능한 줄이기로 했습니다.
팀원 중 한 명은 먼저 말을 꺼내지 않는 성격이라 제가 굳이 의견을 물어보면서 대화의 밸런스를 맞추기도 했습니다.



### philosophers

2021/06/21 ~ 2021/12/13

- 목표: 비동기 시뮬레이션 프로그램을 만들어보는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 1316

상세 구현
- 특정 인원의 철학자가 한 원형 테이블에 모여 있고, 각 철학자 사이에 포크가 있는 상황을 시뮬레이션
- 철학자는 자고 생각하고 먹는 것을 반복한다
- 일정 시간 이상 먹지 못하면 죽는다
- 먹기 위해는 양 옆의 2 개의 포크가 필요하며, 철학자를 최대한 많이 살려야 한다
- 각 철학자는 서로 다른 thread 를 갖는다
- 출력은 실제 시뮬레이션 내용을 1ms 이내의 오차로 출력할 것

이 프로젝트에서는 최대한 근사한 시간을 sleep 하는 방법을 고안해 낸 부분이 자랑스럽습니다.
이 프로젝트에서는 thread 를 sleep 할 때 usleep() 을 사용하도록 강제하고 있습니다.
그런데 usleep() 을 사용하여 특정 시간만큼 sleep 을 하도록 하면 커널이 딱 해당 시간에 thread 를 실행하는 것이 아니라 살짝의 지연 시간이 발생하게 됩니다.
저는 시스템의 sleep() 함수를 '최소한, 입력된 시간 후에 실행하는 것을 보장' 으로 이해하고 있습니다.
그래서 이 sleep 의 지연시간이 얼마나 되는지 생성되어 있는 thread 의 갯수에 따라, usleep() 의 인자로 건내준 입력값의 크기에 따라 표를 만들어 정리해 보기도 했습니다.
일반적으로 지연 시간은 정규 분포를 그리며, 실제 sleep 시간은 프로그램 실행 후 처음 몇 번의 경우 큰 지연 시간을 갖지만, 곧 안정화되어 입력된 시간의 두배를 넘는 경우는 없을 것으로 판단했습니다.
이 데이터를 토대로 저는 1ms 이내의 오차를 달성하기 위해 다음과 같이 구현했습니다.

```
static int	should_sleep_a_sec(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);
	return (gap.tv_sec >= 2);
}

static int	should_sleep_100_msec(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);
	if (gap.tv_sec == 0)
		return (gap.tv_usec > 200 * MSEC_IN_USEC);
	if (gap.tv_sec > 0)
		return (TRUE);
	else
		return (FALSE);
}

static int	should_sleep_10_msec(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);
	if (gap.tv_sec == 0)
		return (gap.tv_usec > 20 * MSEC_IN_USEC);
	if (gap.tv_sec > 0)
		return (TRUE);
	else
		return (FALSE);
}

static int	should_sleep_a_msec(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);
	if (gap.tv_sec == 0)
		return (gap.tv_usec > 2 * MSEC_IN_USEC);
	if (gap.tv_sec > 0)
		return (TRUE);
	else
		return (FALSE);
}

void	sleep_philosopher(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	while (should_sleep_a_sec(time_target))
		usleep(SEC_IN_USEC);
	while (should_sleep_100_msec(time_target))
		usleep(100 * MSEC_IN_USEC);
	while (should_sleep_10_msec(time_target))
		usleep(10 * MSEC_IN_USEC);
	while (should_sleep_a_msec(time_target))
		usleep(MSEC_IN_USEC);
	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);
	if (gap.tv_sec == 0)
		usleep(gap.tv_usec);
}
```

- 목적 시간까지 남은 시간에 따라 다른 시간만큼 usleep() 을 하도록 구현했습니다.
- 하지만 이 구현은 불필요하게 usleep() 을 많이 호출하는 것 같다는 생각이 떠나지 않았습니다.
- 그러다 문득 '남은 시간의 절반만큼 sleep 하도록 하면 어떨까?' 하는 아이디어가 떠올랐습니다.
- 아래는 그 구현입니다.

```
static int	gt_a_sec(const struct timeval *time_target)
{
	struct timeval	time;
	struct timeval	gap;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, &gap);

	return (gap.tv_sec >= 2);
}

static int	gt_a_msec(const struct timeval *time_target, struct timeval *gap)
{
	struct timeval	time;

	gettimeofday(&time, NULL);
	timeval_subtract(time_target, &time, gap);

	if (gap->tv_sec == 0)
		return (gap->tv_usec > MSEC_IN_USEC);
	else if (gap->tv_sec > 0)
		return (TRUE);
	else
		return (FALSE);
}

void	sleep_philosopher(const struct timeval *time_target, int *is_end)
{
	struct timeval	time_curr;
	struct timeval	gap;
	struct timeval	gap_half;

	while (gt_a_sec(time_target))
	{
		if (*is_end)
			return ;
		usleep(SEC_IN_USEC);
	}

	while (gt_a_msec(time_target, &gap))
	{
		timeval_divide(&gap, 2, &gap_half);
		usleep(gap_half.tv_sec * SEC_IN_USEC + gap_half.tv_usec);
	}

	gettimeofday(&time_curr, NULL);
	timeval_subtract(time_target, &time_curr, &gap);

	if (gap.tv_sec == 0)
		usleep(gap.tv_usec);
	else if (gap.tv_sec > 0)
	{
		timeval_divide(&gap, 2, &gap_half);
		usleep(gap_half.tv_sec * SEC_IN_USEC + gap_half.tv_usec);
	}
}
```

남은 시간이 2 초 이상으로 많이 큰 경우는 자원 소모에 민감하지 않기 때문에 1s 씩 sleep 하도록 하였습니다.
1s 보다는 작지만 1ms 이상인 경우 남은 시간의 절반을 sleep 하도록 하여 기존에 평균 O(nlog n) 의 usleep() 호출을 O(log n) 수준으로 줄일 수 있었습니다.

usleep 분석 표: https://docs.google.com/spreadsheets/d/1foXWyx1iNWta76hwp5Q2UI6twG4kJuliuVCLcb6n0g8/edit#gid=0
- 다양한 상태에서 usleep() 함수를 1000 번 호출했을 때 실제 sleep 한 시간을 분석한 테이블



### minishell

2021/06/29 ~ 2021/10/30

- 목표: 경량 버전의 shell 프로그램을 만들어보는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 총 2 명
- total code line : 3971
- 내가 작성한 코드 라인 : 2265

내가 구현한 부분
- 기초 파싱된 데이터를 더욱 가공하여 '()', '&&', '||' 를 파싱한 데이터 생성
- redirection 구현
- 적절한 자식 프로세스 생성 및 관리
- signal 처리
- test case 작성 및 테스트

팀원과의 궁합이 좋지 않은데 코로나로 소통도 원할히 하지 못해 고생했습니다.
이 프로젝트에서 어떻게 해야 성격이 맞지 않는 팀원과 함께 원활히 프로젝트를 진행할 수 있을지 고민을 많이 했습니다.
팀원이 다른 프로젝트에 시간을 배로 들이면서 소통할 시간이 거의 없었던 것도 굉장히 힘들었습니다.
일단 성격이 맞지 않는 팀원의 경우 대화 시간을 많이 갖고, 처음에는 천천히 프로젝트를 진행해야 할 것 같습니다.
만약 팀원이 대화를 원치 않거나 물리적인 시간이 부족한 경우는 최대한 오해를 살 행동을 피하고 서로 공손히 대해야 할 것 같습니다.
불필요한 불편함이 있다면 집중에 방해가 되기 때문에 깔끔한 관계를 유지하는게 최고일 것 같습니다.



### minitalk

2021/06/13 ~ 2021/06/21

- 목표: 한 컴퓨터 내에서 SIGUSR1, SIGUSR2 signal 을 이용하여 한 컴퓨터 내에서 통신하는 서버, 클라이언트 프로그램을 만드는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 722

상세 구현
- SYN, ACK 구현
- checksum 값이 잘못된 경우 데이터 재요청
- UTF-8 전송 가능

packet 구조
- 0: data size
- 4: acknowledgement number
- 8: data
- 8 + data size: checksum

직접 packet 을 설계해서 통신을 구현해볼 수 있는 재밌는 프로젝트였습니다.
UTF-8 이 어떻게 생긴 포멧인지를 이해하는 것은 고통스러웠지만, 이해하고 나서는 유용하게 써먹을 수 있을 것 같아 좋습니다.



### push_swap

2021/05/25 ~ 2021/06/17

- 목표: 배열을 정렬하는 일을 하는 어떤 머신의 instruction 이 있습니다 . 이 때, 이 머신이 배열을 정렬하기 위한 최적화된 프로그램을 생성하는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 2059

마치 컴파일러가 소스 코드를 읽고 최적화된 바이너리 코드를 생성하는 기능을 구현하는 것 같은 최적화 문제입니다.
입력된 배열의 길이가 짧은 경우에는 깊이 우선 탐색으로 모든 경우의 수 중 가장 짧은 프로그램을 얻도록 했습니다.
입력된 배열의 길이가 긴 경우에는 고정된 알고리즘을 통해 정렬 프로그램을 생성한 후 불필요한 instruction 을 제거하는 최적화를 하도록 했습니다.



### miniRT

![output.bmp](/image/output.bmp)

2021/04/04 ~ 2021/06/03

- 목표: 점을 찍는 기초적인 instruction 으로 3D 그래픽을 구현하는 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 2764

상세 구현
- 삼각형, 사각형, 평면, 원, 구, 원기둥, 빛의 3D 이미지 생성
- 'c' 버튼을 누르면 미리 정의된 다음 카메라 위치로 이동
- 특정 파일을 읽고 명시된 작업 내용을 토대로 이미지를 출력하도록 구현
- 생성한 이미지를 bmp 형식으로 저장 하는 기능

저는 이미 엑셀에서 색을 바꾸는 매크로를 이용하여 선과 정육면체를 구현해 본다거나, 셀의 색 데이터를 압축하여 저장했다가 다시 이미지로 불러오는 것을 구현해 볼 정도로 그래픽 구현에 관심이 있었습니다.
그래서 점을 찍는 것과 같은 원시적인 instruction 으로 3D 그래픽을 구현하는 이 project 는 매우 의욕이 있었습니다.
2 달간 주말도 쉬지 않고 매일 10 시간 이상씩 작업할 정도로 제 인생에서 가장 몰입하여 프로그래밍을 했습니다.
이 과제는 욕심이 있어서 참고 자료를 보지 않고 제가 생각하는 레이 트레이싱을 직접 구현해보는 기회가 되었습니다.

단일 도형들을 구현하고 난 후 원기둥을 구현하자니 구조가 아름답지 않았습니다.
지금까지 모든 도형은 단일 개체인 것을 의도로 작성하였습니다.
하지만 원기둥은 3 개의 단일 개체가 모인 복합 도형입니다.
새롭게 복합 도형 개념을 추가하자니 중심 로직을 수정해야 해서 추가 소용 기간이 부담되었습니다.
저는 현재 프로젝트가 이미 많은 부분 진행됐으며, 42 커리큘럼의 가이드 기간을 슬슬 넘어가고 있었기 때문에 다소 아름답지 않더라도 현재 구조에서 빠르게 구현 가능한 방향으로 구현하였습니다.



### ft_server

2021/03/21 ~ 2021/03/28

- 목표: docker 를 사용하여 요구하는 환경을 설정해보는 42 프로젝트
- environment: Docker, Vim, Git



### ft_printf

2021/02/11 ~ 2021/03/28

- 목표: C 언어의 printf() 함수의 경량 버전을 만들어보는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 1181

상세 구현
- '0', '-', '#', ' ', '+' flag 구현
- optional minimum field width 구현
- optional precision 구현
- 'll', 'l', 'hh', 'h' optional length modifier 구현
- 'd', 'i', 'o', 'u', 'x', 'X', 'c', 's', 'p', 'n', '%' conversion specifier 구현



### get_next_line

2021/01/25 ~ 2021/02/10

- 목표: 주어진 fd 로부터 한 줄의 데이터를 읽어서 caller 에게 전달하는 함수를 만들어보는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 479



### libft

2020/12/25 ~ 2021/01/24

- 목표: 명세서의 함수들을 구현하여 libft.a 라이브러리 파일을 만드는 42 프로젝트
- language: C
- environment: Vim, Git
- team size : 1 명
- total code line : 1252



## [대한상공회의소 충남인력개발원] ROS 기반 자율비행 드론 애플리케이션 개발자 과정

2020/05/18 ~ 2020/09/30



### 드론 비행 미션 수행 프로그램

- 목표: 1 ~ 3 대의 드론에 미리 작성된 여러 패턴의 비행 미션 수행 프로그램 작성
- GitHub: https://github.com/Liemani/_deprecated_portfolio/tree/main/tool/ROS
- language: C++
- environment: VS Code, Git
- 팀원: 총 2 명

내가 구현한 부분
- 선 이동 같은 가장 단순한 미션인 CoreMission 을 합쳐 ConcreteMission 을 작성할 수 있도록 구조 설계 및 구현
- 코어 미션: 특정 고도 이동
- 코어 미션: 특정 상대 위치 이동
- 코어 미션: 특정 gps 좌표 이동

제 인생 첫 팀 프로젝트입니다.
팀원이 프로그래밍이 처음이라, 제가 시스템을 작성하고 팀원이 이 시스템을 활용하여 복잡한 기능을 구현하도록 하였습니다.
팀원이 최대한 쓰기 편하도록 시스템을 구현하기 위해 사용법을 알려주는 동시에 사용하기 불편해 보이는 기능을 개선하는 작업을 했습니다.



### arduino

- 목표: arduino 사용해보기
- GitHub: https://github.com/Liemani/_deprecated_portfolio/tree/main/tool/Arduino
- language: C++
- environment: VS Code, Git

실습 모듈
- led
- buzzer
- 온습도 센서
- joystick
- 7-segment
- 4x4 keypad
- motor
- relay
- lcd display
- Ultrasonic Sensor
- tilt
- touch

4x4 keypad을 보고 Jubeat 라는 음악 게임이 생각나서 유사한 게임을 만들기도 했습니다.
serial print 로 4x4 의 X 를 계속 출력하다가 주기적으로 O 로 변하는 위치의 버튼을 누르면 다시 X 로 바뀌는 게임입니다.
끝나면 시간에 따른 점수가 출력되도록 했습니다.
화면을 너무 느리게 출력하면 플레이에 지장이 갔으며, 너무 빠르게 출력하면 화면이 내용을 안정적으로 보여주지 못해 적당한 속도로 설정했습니다.



### 자판기 프로그램

- 목표: 도서관 책 대출 프로그램의 자판기 버전
- GitHub : https://github.com/Liemani/_deprecated_portfolio/tree/main/project/VendingMachine
- language: C
- environment: VS Code, Git
- team size : 1 명
- total line number : 1027

상세 구현
- 프롬프트로 금액을 입력받고 선택한 음료에 대한 반응 출력
- 음수를 입력받으면 관리자 페이지 출력
- 음료 데이터를 데이터로 저장하여 프로그램이 종료 되어도 값이 보존되도록 구현



## Haven and Hearth Assistant 앱 출시

![haven_and_hearth.png](/image/haven_and_hearth.png)

2020/02/01 ~ 2020/03/14

- 목표: 빠르게 앱 출시
- 앱 링크: https://apkpure.com/haven-and-hearth-assistant/com.havenandhearthassistant
- language: Kotlin
- environment: Android Studio
- team size : 1 명
- total line number : 596

상세 구현
- Haven and Hearth 게임에 필요한 계산을 도와주는 프로그램 작성
- AdMob 달기

앱 출시 뒤 우크라이나에서는 소수점이 우리와 달리 ',' 를 사용하기 때문에 계산에 문제가 있다는 피드백을 받고 업데이트를 하기도 했습니다.



## 터미널 작업 환경 구축

2020/12/25 ~ 계속

- 목표: 어떤 터미널 환경에서도 나의 작업 환경을 바로 셋업해주는 shell script 작성
- GitHub: https://github.com/Liemani/env
- language: zsh, bash
- environment: Vim, Git
