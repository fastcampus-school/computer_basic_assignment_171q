﻿---
1월 10일 과제
---

#1. RAM은 어떤 단어들의 약자이며, 왜 RAM이라고 부르게 되었을까?

옆자리 앉은 분에게 물어본 결과 랜덤 억세스 메모리. RANDOM ACCESS MEMORY 이다.<br/>
휘발성 메모리이기 때문에 저장하는 위치가 랜덤이고 무작위의 위치의 읽기와 쓰기의 시간이 동일하기 때문에 그렇게 부르게 되었다고 한다.<br/>
찾아보니 맞다.<br/>


#2. 한글을 표현할 수 있는 문자 인코딩 방식에는 무엇이 있을까? 각각의 장단점도 조사해 보세요

한글을 표현할 수 있는 문자 인코딩 방식에는 크게 UTP-8 과 EUC-KR 가 있다.


## UTF-8
UTF-8은 유니코드(전 세계의 모든 문자를 컴퓨터에서 일관되게 표현하고 다룰 수 있도록 설계된 산업 표준)이다.   <br/><br/>

현재 웬만한 서버운영체제와 웹서버, 코딩자체가 UTF-8로 제작하면 별다른 인코딩을 따로 할 필요가 없으며
초성과 중성, 종성을 각 1바이트로 인식하는 조합형 인코딩 방식이고 일반적인 한글을 3바이트로 인식한다. <br/>
단점이라면 영문은 ASCII 를 사용하면 각 문자당 1바이트로 모든 영어를 표현할수 있기 때문에 비교된다.<br/>
그렇지만 다른 국가에서 한글 언어팩이 설치되지 않았다고 하더라도 한글표현이 가능하기 때문에 다양한 언어로 작성되는 환경이나 웹같은 환경에서 좋다.<br/>
UTF-7 , UTF-16, UTF-32 와 같이 다른 인코딩방식이 있으나 UTF-8이 ASCII 와 호환되기 때문에 가장 많이 사용한다.<br/>

## EUC-KR
완성형 인코딩 방식으로 한글을 2바이트로 사용한다.<br/>
한글과 영어만을 사용하는 페이지에서 적합하나 그외의 환경에서는 부적합할 가능성이 많다. 또 완성형 문자 이기 때문에 빠져있는 문자가 있으면 표현이 되지 않는다.<br/>  
EUC-KR은 2350자의 완성형 한글을 표현할수 있게 해주며 이후 확장된 CP949 인코딩방식은 11,172개의 완성된 한글을 제공하는 인코딩 방식이다.<br/>


<br/><br/><br/><br/>




---
덧. 어제 관심분야 작성 과제가 remote repository에 업로드가 안되었었습니다 ㅠㅠ 수정했으니 한번더 확인부탁드리겠습니다. [9일 과제 링크]

[9일 과제 링크]:<https://github.com/fastcampus-school/computer_basic_assignment_171q/tree/master/170109/a.choongyul.lee>
---