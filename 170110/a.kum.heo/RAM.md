---
#RAM
---

##1. RAM에 대해
RAM은 Random Access Memory의 줄임말로 여기서 Random Access란 무작위로 접근한다는 말이 아닌, 어디로든 똑같은 시간으로 접근 가능하다는 의미로, 메모리의 주소말 알고 그곳을 지정하면 별다른 절차 없이 바로 접근이 가능하다는 의미이다<br/>

RAM을 두가지로 나누어보면 RAM과 같은 주기억장치인 ROM과 RWM(Read Write Memory)로 나눌 수 있는데, 우리가 지금 부르는 RAM은 엄밀히 따지면 RWM 이라 할 수 있다.<br/>
	하지만 이름이 RAM이 된 이유는 RAM의 개발당시에 RWM이 SAM(Sequentail Access Memory)의 세분화된 메모리 방식을 말하는 용어로 선점되어 있었기에 용어의 혼란을 막고자 RAM이라 명명했다.<br/>

RAM은 사용자가 자유롭게 내용을 읽고 쓰고 지울수 있는 주 기억 장치로, 컴퓨터는 CPU에서 이뤄진 연산을 메모리에 기록하며 또 읽어온다. 때문에 메모리가 없거나, 뻑나는 경우 os는 부팅조차 할 수 없다.

RAM은 보조기억장치인 HDD나 SSD와 달리 전원이 끊기면 내부에 저장된 데이터가 삭제되는 휘발성 메모리이다.

흔히 ‘메모리’라 하면 HDD나 SSD, USB를 생각하기 쉬운데 이것들은 어디까지나 주기억장치의 확장격인 보조기억장치이다

##2. RAM의 종류
RAM의 종류는 크게 SRAM과 DRAM으로 나뉜다

* SRAM : 주기적으로 내용을 갱신해 주어야 하는 DRAM과는 달리 전원이 공급되는 한 그내용이 계속 보존된다. SRAM은 회로가 대칭구조를 가지고 있기 때문에 DRAM보다 빠른 입출력이 가능하고 주소에 접근할 때 상위 비트와 하위비트 순서로 두번 접근해야 하는 DRAM과 달리 SRAM은 한번에 접근할 수 있다는 장점이 있다.

* DRAM : DRAM은 정보를 구성하는 개개의 비트를 기본적으로 capacitor(축전기)에 저장하며 각각의 capacitor가 담고 있는 전자의 수에 따라 비트의 1과 0을 표현하지만 결국 축전기가 전자를 누전하므로 정보를 잃게되므로 계속해서 재충전해 사용한다.
기억장치의 내용을 일정시간마다 재생시켜야 되는것을 일컬어 동적(Dynamic)이란 명칭이 붙었다.


<br/>
