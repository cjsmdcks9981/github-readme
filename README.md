# Linux

![리눅스 ](https://github.com/cjsmdcks9981/helloworld_230517/assets/111216695/55967e7a-3279-4371-a953-64701ccef970)




리누즈 토발즈(Linus Torvalds)에 의해 만들어진 컴퓨터 운영체제로, 자유 소프트웨어와 오픈 소스 개발의 가장 유명한 표본이다.
리눅스는 유닉스(Unix)라는 운영체제를 기반으로 하고 있으며, 뛰어난 안정성과 보안성, 높은 신뢰성과 성능이 특징이다.

| Linux_종류 | 출시 날짜 | 최신 버전 |
|------|---|---|
|Ubuntu|	1993년 9월 | 22.0.4.2LTS |
|Debian| 2004년 10월 20일 | 11 |
|Redhat| 1995년 5월 13일 |	9 alias Shrike |
|Oracle| 2006년 10월 26일 | 9.0 |
|Fedora|	2003년 11월 6일 | 35 |
|Centos|	2004년 5월 14일 | 8.5.2111 |
|Suse| 2000년 8월 31일 | 15 Service Pack 4 |

# Linux_Commands

## top
Top 명령어

- **개**
![top예시](https://github.com/cjsmdcks9981/github-readme/assets/111216695/8f34dbee-bbd6-4f7f-a396-4ab8fe0c33fc)



 Top 명령어는 실시간으로 OS의 상태를 나타내주는 명령어이다. Top 명령어을 통해서 메모리 사용량, CPU 사용량 등을 확인 할 수 있다. 
top 명령어를 실행 후 상단에는 시스템에 대한 전반적인 요약 정보가, 하단에는 프로세스별 구체적인 정보가 표기된다.
정보는 3초마다 업데이트 된다.

---

- **명령어**

`top [option]`
 을 입력하게 되면 바로 실행이 된다
 
 ---

- **옵션**

`-a` 메모리 사용에 따라 정렬


`-b` 배치 모드에서 시작


`-c` 명령어 대신 명령어 라인을 보여줌


`-d time` 업데이트 간격을 조정


`-h` 도움말


`-H` 모든 개별 쓰레드가 보여짐


`-i` 좀비 또는 Idle 상태의 것들은 무시해서 출력


`-m` VIRT 대신 USED를 보고


`-M` 메모리 유닛( Kib / Mib / Gib )을 출력


`-n` 반복의 최대 수를 지정


`-P` 지정된 프로세스 ID들만 출력


`-s` 보안 모드로 시작


`-S` 누적 시간 모드로 시작. 활성화되면 각 프로세스는 CPU를 사용한 시간과 함께 출력


`-u user` 지정된 유효 사용자에 의한 프로세스만 출력


`-U` 지정된 사용자에 의한 프로세스만 표시. 사용자는 실제, 유효한, 저장된 및 파일시스템 UID를 의미


`-v` 프로그램 라이브러리 버전을 출력


 ---
 
- **단축키**

`h`
 도움말 출력
 
`k`
 프로세스 강제 종료
 
`q`
 top 명령어 종료
 
`r`
 우선순위 변경
 
`s`
 프로세스 간격 변경
 
`f`
표시할 항목 선택

`u`
특정 사용자의 프로세스만 보기

`M`
메모리 사용률 순으로 정렬

`m`
메모리 사용률을 시각화 하여 표시

`E`
상단에 표기되는 데이터 단위가 변경

`e`
하단에 표기되는 데이터 단위가 변경

`P`
CPU 사용률 순으로 정렬

`T`
실행 시간 순으로 정렬

`1`
CPU Core별로 사용량 출력


---


- **요약 정보**

![요약 ](https://github.com/cjsmdcks9981/github-readme/assets/111216695/11ee904d-2a2a-489c-88f5-63d8c3bebf21)

**시스템 정보**


`top` 현재 시간을 출력

`up` 컴퓨터가 연속으로 실행되고 있는 시간을 출력

`user` 로그인 한 사용자 수를 출력

`load average` 왼쪽 순서대로 1분, 5분, 15분 간의 로드의 평균 출력

>여기서 로드란 **리소스 사용량**을 비율로 표시한 지표를 의미한다. **싱글코어** 일때 1.0 이면 **100%** 를 사용하고 있다는 의미고 **코어**에 1.0 이면 **50%** 를 사용 하고 있다는 것을 의미한다.

---

**프로세스 정보**


`Tasks` 프로세스의 상태를 출력.

`total` 총 프로세스 수

`running` 실행되고 있는 프로세스 수

`sleeping` 대기 중인 프로세스 수

`stopped` 멈춘 프로세스 수

`zombie` 좀비 상태인 프로세스 수

---

**CPU 정보**


`us` 사용자 영역 프로세스에서의 cpu 사용률

`sy` 커널 영역 프로세스에서의 CPU 사용률

`ni` 우선순위로 할당된 사용자 영역 프로세스를 실행하는데 소요되는 CPU 사용률

`id` CPU를 사용하고 있지 않은 비율

`wa` I/O가 완료될 때까지 기다리는 CPU 사용률

`hi` 하드웨어 인터럽트에 사용되는 CPU 사용률

`si` 소프트웨어 인터럽트에 사용되는 CPU 사용률

>인터럽트란? 
 인터럽트는 CPU가 하던 작업을 중단하고, 먼저 처리할 다른 작업을 수행하고 다시 원래의 작업으로 복귀하도록 하는 신호이다.
 
 **하드웨어 인터럽트**는 외부 장치 또는 **하드웨어**에서 생성되는 인터럽트이다.
 
 **소프트웨어 인터럽트**는 컴퓨터의 **내부 시스템**에서 생성되는 인터럽트이다.
 

`st` CPU를 가상 머신에서 사용함으로써 생기는 손실된 CPU의 비율

---

**메모리 정보**

**KiB, MiB, GiB는 데이터 단위**


`Mem` 물리 메모리 사용 정보

`total` 총 메모리

`free` 여유 메모리

`used` 사용 중인 메모리

`buff/cache` 버퍼 또는 캐시 메모리

---


`Swap` 스왑 메모리 정보 출력

>Note. 스왑 메모리는 가상 메모리로 불리며, 메모리가 부족할 때 디스크 공간을 이용해서 부족한 메모리 공간을 대체할 수 있는 메모리

`total` 총 메모리

`free` 여유 메모리

`used` 사용 중인 메모리

`buff/cache` 버퍼 또는 캐시 메모리

---

- **하단 정보**

`PID` 프로세스 ID

`USER` 프로세스의 소유 계정

`PR` 프로세스 우선순위

`NI` PR에 영향을 주는 나이스 값

>Note. linux 상에서 process 가 실행될 때, nice 라는 값을 갖고 실행되는데. nice 값은 process 간 실행 우선순위를 의미한다.
 
>PR은 우선순위*

`VIRT` 프로세스가 사용하고 있는 가상 메모리의 총량

`RES` 프로세스가 사용하고 있는 물리 메모리의 양

`SHR` 다른 프로세스와의 공유 메모리

`S` 프로세스의 상태를 의미

 >***D***는 네트워크 I/O를 대기하고 있는 상태, ***R***은 실행 중인 상태, ***S***는 대기 상태, ***Z***는 좀비 상태 
 
 >Note. 좀비 상태란 부모 프로세스가 죽은 자식 프로세스를 의미*

`%CPU` 프로세스의 CPU 사용률

`%MEM` 프로세스의 물리 메모리 사용률

`TIME+` 프로세스가 사용한 토탈 CPU 시간

`COMMAND` 해당 프로세스를 실행한 커맨드





## ps
ps명령어

![a](https://github.com/cjsmdcks9981/github-readme/assets/111216695/56427cca-37a7-430a-b52c-5b94af2ab30d)


- **개요**

ps는 **process status**의 줄인 말로 현재 실행 중인 프로세스의 목록과 상태를 출력해준다. ps를 사용하면 수 많은 프로세스의 정보를 얻을 수 있으며 **운영체제(V, BSD, GNU)**에 따라 결과가 다르게 나타나고 표기법에도 차이를 보인다. ps 명령어를 이용해 분석하여 시스템의 오류를 감지할 수 있다.


기본적으로 PID, TTY, TIME, CMD 네 개의 기본적인 정보만 출력을 해준다. 더 많은 정보를 출력하기 위해서는 옵션을 넣어 자세한 내용을 출력 할 수 있다.


- **명령어**

`ps [option]` 을 입력하면 출력이 된다.


- **옵션**

`-a` 터미널과 연관이 없는 프로세스를 제외한 모든 프로세스를 출력한다.

`a` 터미널과 연관된 모든 프로세스를 출력하거나, x 옵션과 함께 사용되어 모든 프로세스를 출력할 수 있다.

`-d` 세션 리더를 제외한 모든 프로세스들을 출력한다.

> 세션 리더는 세션을 만든 프로세스이다.


`r` 실행 프로세스만 출력한다.

`x` 사용자에 의해 소유된 모든 프로세스를 출력한다.

>a 옵션과 함께 사용되며 모든 프로세스를 출력한다.

`-l` 상세한 내용을 출력한다.

`-f` 완전한 형식의 목록을 출력한다.

`-h` PID, TTY, STAT, TIME 등의 항목을 보여주지 않는다.

`-j` 작업에 관련된 ID를 출력한다.

`u` 사용자 친화적인 형식으로 출력한다.

`f` 프로세스  간 상속관계를 트리구조로 출력 한다.

`n` 사용자의 정보를 숫자로 표시한다.

`-w` 출력결과를 생략하지 않고 넓게 출력한다.

`-e` 모든 프로세스 출력

`-o` 출력 포맷을 지정하여 출력 (pid, tty, time, cmd 등)

>ps -o pid

- **자주 사용되는 옵션**

`ps -ef` : 모든 프로세스를 풀 포맷으로 출력

`ps -ef|grep 'name'` : 'name'의 프로세스 구동 확인

`ps aux` 실행중인 모든 프로세스 확인

`ps auxf` 실행 중인 프로세스를 트리구조로 출력

`ps auxfww` 실행 중인 프로세스를 트리구조 + 모든 실행 중인 옵션 확인 가능

`ps ax` 시스템의 모든 프로세스를 BSD 포맷으로 출력한다.


- **출력 정보**


`SID` 세션 ID

`PID` 프로세스마다 주어지는 번호

`PPID` 부모 프로세스의 ID다.

`%CPU(BSD)` CPU 사용 비율의 추정치

`%MEM(BSD)` 메모리의 사용 비율의 추정치

`VSZ` k단위 또는 페이지 단위의 가상메모리 사용량

`RSS` 실제 메모리 사용량

`S(System V), STAT(BSD)` 현재 프로세스의 상태코드

`TIME` 총 CPU 사용 시간

`COMMAND` 사용자가 실행한 명령어

`STIME` 프로세스가 시작된 시간 또는 날짜

`C(System V), CP(BSD)` 짧은 기간 동안의 CPU사용률

`F` 프로세스의 플래그

`PRI` 실행하는 우선순위에 따른 프로세스

`NI` nice 우선순위 번호

`STAT` 실행되고 있는 프로세스 상태 (D: 무중단 절전, R: 실행 중, 실행 가능 S: 인터럽트 가능 절전, T: 중지됨, W: 페이징, X: 사망, Z: 좀비 프로세스)

##top과 ps의 차이점

ps는 ps를 한 시점에서 proc에서 검색한 정보이고 top은 proc에서 일정 주기로 합산해서 정보를 출력한다. 즉, top 과 ps가 보여주는 결과가 서로 다르다. 따라서 top은 모니터링 툴 이라고 할 수 있고 ps는 사진 이라고 생각을 하면 이해 하기 쉽다.

>proc는 리눅스 부팅시 커널이 메모리 상에 가상으로 만들어놓은 파일시스템이다. /proc 디렉토리에 실행중인 프로세스 정보, CPU, 메모리 등 시스템 정보를 담고 있다.

## jobs

jobs 명령어

- **개요**

![b](https://github.com/cjsmdcks9981/github-readme/assets/111216695/cfe17fa3-034a-4160-a3c1-fc8eb93a4b3a)

jobs 명령어는 백그라운드로 실행된 프로그램이나 실행한 프로그램에 대해서 작업의 상태를 표시하는 명령어이다. jobs 명령어를 통해서 작업이 중지된 상태, 백그라운드로 진행 중인 작업 상태, 변경 되었지만 보고되지 않은 상태 등을 확인 할 수 있다.

- **명령어**

`jobs [option]` 를 사용하면 실행이 된다.

- **옵션**

`-p` 각 프로세스 ID에 대해 출력

`-l` 프로세스 그룹 ID를 state 필드 앞에 출력

`-s` 프로세스 중 멈춰있는 프로세스만 출력

`-n` 각 프로세스 ID에 대해 한 행씩 출력

`-r`  프로세스 중 실행중인 프로세스만 출력

`command` 지정한 명령어를 실행

- **출력 정보**

`Running` 작업이 계속 진행중

`Done` 작업이 완료되어 0을 반환하고 종료함.

`Done(code)` 작업이 종료되었으며 0이 아닌코드 반환.

`Stopped` 작업이 일시중단됨

`Stopped(SIGTSTP)` SIGTSTP 신호가 작업을 일시 중단

`Stopped(SIGSTOP)` SIGSTOP 신호가 작업을 일시 중단

`Stopped(SIGTIM)` SIGTTIN 신호가 작업을 일시 중단

`Stopped(SIGTTOU)` SIGTTOU 신호가 작업을 일시 중단


## kill

kill 명령어

- **개요**


![adsaa](https://github.com/cjsmdcks9981/github-readme/assets/111216695/00b887b4-3db5-4a7f-9426-a9d3aa9c8cbe)


kill 명령어는 이름 때문에 프로세스를 강제로 종료시키는 명령어로 kill 명령어는 주로 프로세스를 종료하는 용도로 많이 사용된다.

- **명령어**

`kill [option] [pid]`

`kill -s [signal id or text] [pid]`

`kill -[signal id or text] [pid]`

s 옵션으로 시그널을 지정하지 않으면 기본 시그널 값이 정상종료된다.
프로세스를 안전하게 종료하기 위해서는 데이터 유실 위험이 있어 강제 종료를 권장하지 않는다. 

>`PID` 프로세스마다 주어지는 번호

![as](https://github.com/cjsmdcks9981/github-readme/assets/111216695/686087e0-e2e2-42e6-870b-7607ab14e7f7)

>`PID` 프로세스마다 주어지는 번호

파이프와 grep, awk 등을 이용하여 조합하면 특정 이름의 프로세스를 모두 찾아서 종료 시킬 수 있다.

``` kill `ps -ef | grep 프로세스이름 | grep -v grep | awk '{print $2}'` ```

- **옵션**

`kill -l`

![arw](https://github.com/cjsmdcks9981/github-readme/assets/111216695/3bcc402a-39e9-482c-8330-7ba5aeec3839)

> 앞에 SIG를 빼고 이름을 넣어도 작동하고 숫자를 넣어도 작동한다.

이렇게 많은 옵션이 있지만 아래 3개의 옵션이 가장 일반적으로 사용된다

`1) SIGHUP` 프로세스를 다시 로드한다.

`9) SIGKILL` 프로세스를 제거.

`15) SIGTERM` 프로세스를 정상적으로 중지.






