﻿## 2017.01.12 오늘의 과제

> #### 1. 국내에 공인인증서가 생긴 배경과 그 위험성은?
>> 1. **국내에 공인인증서가 생긴 배경 (출처: 나무위키, 공인인증서 - 역사 항목)**
>> 
>> : 1999년 전자서명법이 발효되면서 전자정부의 초석을 다지기 위해 11명의 암호학 교수들이 모여서 연구를 시작했다. 연구 도중 두 파벌로 나뉘면서 상공회의소+행정부를 중심으로 한 축과 금융결제원, 은행, 보험등 금융업계로 나뉘게 된다.
>>
>> 이에 따라 전자는 모든 국민의 개인정보를 행정부가 보증하게 되었고, 입찰을 통해 사인 발급자로서 한국정보인증(KICA, Signgate)이 담당하게 되었다. 즉, 사인의 보증을 공적 주체가 맡게 된다. 반면 후자는 금융결제원(yessign)이 발급 주체가 되었고, 은행, 보험회사들이 보증 주체가 되었다.(결국 보증을 사적 주체가 하게 되는 셈이다.) 이 경우 금융 거래만 하는 사람만 금융결제원에 기록이 있으므로 대상이 제한되게 되었다.
>>
>> 이는 전자인감이 필요한 공적 증명을 행정부가 맡고, 일반 은행 거래 정도는 금융결제원이 한다는 초기 목표가 있었기 때문에 이뤄진 것인데, 문제는 99년 당시엔 전자서명법은 발효되었어도 전자정부법은 아직 없었다. 그래서 '전자인감'이라는 개념은 효력이 없었고, 따라서 전자인감으로 인증서를 발급받을 만한 근거도 없었다. 이는 2001년까지 기다리게 된다.
>>
>> 이 과정에서 먼저 범용 인증서가 상공회의소, 전자정부, 학교를 중심으로 사용하게 되었지만 일반 개인 인증서는 커버할 수 있는 부분이 매우 적어졌다. 즉, 개인이 결제하는데 인증서를 발급받고자 하면, 사인시 사적 보증을 서주는 은행의 커버 범위로만 한정되는데다, 은행간 연동이 안되었던 것이다. 이후 타행 인증서를 만듦으로서 서로 연대보증하는 개념으로 이 문제를 해결하였다. 이 와중에 은행권에서도 금융결제원(yessign) 자체가 보증을 서는 범용 인증서를 만들었다. 2001년 전자정부법이 나오기 전 불과 2년 사이에 아수라장이 되어버린 것이다.
2001년이 되어서 전자 정부법이 발효되고, 사람들이 대거 공인인증서를 쓰게 되자 이러한 결과에 대한 불평이 쏟아져 나왔다. 결국 전자서명법이 개정되었다. ([국회-의안정보시스템 참조](http://likms.assembly.go.kr/bill/jsp/BillDetail.jsp?bill_id=PRC_D1A3N0P5U2L8K1H3C4E1H2C4B0Z3U2)) 오직 정부만 보증 주체가 될 수 있고 보안을 강화시켰다. 다만 발급을 대행하는 곳을 한국정보인증(KICA), 한국전자인증(crosscert) 등등 여러 회사로 두게 하였다. 개정된 법에 따라 금융결제원(yessign), 은행 및 보험사는 범용인증서를 발급할 수 없게 되었다. 이 과정에서 기존의 인증서들은 범용인증서로 이관이 되었다.
>>
>>2012년 1월부터 알고리즘이 강화되어 인증서를 발급/갱신하게 되면서 기존의 인증서보다 알고리즘이 강화된 인증서로 교체된다.
>>
>> 2. **공인인증서의 위험성**
>>     1. 공인인증서는 표준화되지 않은 기술, 즉 ActiveX 방식으로 배포된다. 사용자의 주의가 없다면 ActiveX로 악성프로그램까지 설치할 수 있게 되므로, 피싱사이트 등에서 보안 사고가 발생할 가능성이 높다.
>>     2. 안전상 중요한 공인인증서를 공개되어있는 사용자의 저장장치에, 그것도 일반 폴더인 NPKI 폴더에 저장하며, 그냥 이 폴더를 복사해가면 공인인증서를 복사할 수 있다. 포털사이트의 암호 등이 공인인증서와 비슷하거나 같으면 크래커가 바로 사용자의 공인인증서를 이용 가능하다.
>>     3. 대다수의 사용자가 낮은 보안의식을 가지고 공인인증서를 사용하기에 ActiveX 설치프로그램이 나타나면 반사적으로 확인을 누르게 되어 있다. 애초에 ActiveX를 설치하겠냐는 물음에 아니오를 누르면 결제가 안 되므로, 설치하겠냐는 물음이 뜨면 조건반사적으로 예를 누르게 되고, 결국 잘 알지도 못하는 프로그램을 무작정 설치 및 실행할 위험성이 높다.
>>     4. 만약 개인이 공인인증서가 털려 해킹과 같은 문제를 당하면 기업에서 지정한 절차를 지켰음에도 개인의 부주의로 해킹을 당했음을 증명해야 하는 등, 기업에서 책임을 면피하려 한다.
>
>#### 2. 애플리케이션 접근성의 의미와 현 상황
>>  1. 앱(애플리케이션) 접근성?
>>
>>     : 접근성이란 사용자의 신체적 특성이나, 지역, 성별, 나이, 지식 수준, 기술, 체험과 같은 제한 사항을 고려하여 가능한 많은 사용자가 불편 없이 이용할 수 있도록 제품, 서비스를 만들어 제공하고 이를 평가할 때 쓰이는 말이다. 접근성이 높다는 것은 이러한 제한사항을 가진 사용자도 불편없이 사용할 수 있다는 것을 뜻하며 접근성이 낮다는 것은 어떠한 제한 때문에 사용하기 불편하거나 사용할 수 없을 때를 말한다. 따라서 애플리케이션 접근성이란 프로그램을 사용할 때 위와 같은 접근성의 조건을 충족하는 것이라 볼 수 있다.
>>  2. 앱(애플리케이션) 접근성의 현 상황
>> 
>>     : 현재 참조할 수 있는 애플리케이션 접근에 관한 문서를 찾아보니 모바일 애플리케이션 접근성 지침 2.0에 관한 글이 있어서 이를 바탕으로 현 상황을 살펴보고자 한다.

>>       모바일 애플리케이션 접근성 지침 2.0의 목적은 모바일 애플리케이션 서비스 제공자가 장애인, 고령자 등의 접근성을 보장하기 위해 지켜야 할 규정을 마련하는 데에 있다고 설명되어 있다. 접근성 지침이 만들어짐으로써 장애인, 고령자 등이 동등하게 모바일 애플리케이션을 이용할 수 있는 환경을 조성하는 데에 기여하는 것이다.

>>       접근성 지침 2.0은 세부적으로 4개의 원칙 하에 19개의 지침이 있고, 4개의 원칙만 살펴보면 다음과 같다.
>>       1. 인식의 용이성 : 인식의 용이성은 사용자가 장애유무 등에 관계없이 애플리케이션의 모든 콘텐츠를 동등하게 인식할 수 있도록 제공하는 것을 의미
2. 운용의 용이성 : 운용의 용이성은 사용자가 장애무 등에 관계없이 애플리케이션에서 제공하는 모든 기능들을 운용할 수 있게 제공하는 것을 의미
3. 이해의 용이성 : 이해의 용이성은 사용자가 장애유무 등에 관계없이 애플리케이션에서 제공되는 콘텐츠를 이해할 수 있도록 제공하는 것을 의미
4. 견고성 : 견고성은 사용자가 기술에 관계없이 애플리케이션에서 제공하는 콘텐츠를 이용할 수 있도록 제공하는 것을 의미
>>
>>       또한, 접근성 지침 2.0에는 4가지 원칙을 제외한 총 5가지의 지침이 신설되었다고 하는데, 이는 다음과 같다.
>>            * (명확한 지시사항) 지시사항은 모양, 크기, 위치, 방향, 색, 소리 등에 관계없이 인식될 수 있어야 한다. : 화면에 표시된 특정 객체를 가리킬 때나, 지시사항을 전달하는 콘텐츠는 가리키고자 하는 객체의 정확한 명칭이나 객체에 포함된 대체텍스트를 언급하여 사용자가 지시하고자 하는 것이 무엇인지를 명확히 알 수 있도록 합니다. 또한, 지시사항은 하나의 감각에 의존하지 않고 여러 감각을 통해 인식할 수 있도록 해야 합니다. 예를 들어 특정 음향 신호를 통해 지시사항을 전달할 경우 청각에 장애가 있는 사용자를 위한 대체 수단이 함께 제공되어야 합니다.
>>            * (응답시간 조절) 시간 제한이 있는 콘텐츠는 응답시간을 조절할 수 있어야 한다. : 보안 등의 이유로 시간 제한이 있는 콘텐츠는 제한시간 연장 또는 이를 제어할 수 있도록 해야 합니다. 단, 경매나 실시간 게임과 같이 반응 시간을 조절할 수 없는 콘텐츠는 예외로 하지만 반드시 사용자에게 해당 내용을 고지해야 합니다.
>>            * (정지기능 제공) 자동으로 변경되는 콘텐츠는 움직임을 제어할 수 있어야 한다. : 자동으로 변경되는 콘텐츠는 일시 정지할 수 있는 기능을 제공해야 합니다. 또한, 자동으로 변경되는 콘텐츠 중 지나간 콘텐츠 등을 다시 확인할 수 있는 컨트롤 수단을 제공해야 합니다.
>>            * (입력 도움) 입력서식 이용 시, 입력 오류를 방지하거나 정정할 수 있는 방법을 제공해야 한다. : 입력 서식에는 반드시 입력 내용의 제목을 제공해야 합니다. 만약 사용자가 잘못된 내용을 입력했다면 어떤 입력 서식에서 오류가 있었는지 등을 명확히 알려야 하며, 되도록 잘못 입력된 입력 서식으로 초점을 이동시켜주어야 합니다.
>>            * (예측가능성) 사용자가 의도하지 않는 화면 전환이나 이벤트 등이 실행되는 경우 사용자가 이해할 수 있는 방법으로 제공되어야 한다. : 모바일 애플리케이션에서는 PC의 웹과는 달리 객체 정보에 Native Component를 이용하지 않고, 커스터마이징하는 경우 모바일 스크린리더는 해당 객체가 링크 등의 컨트롤 요소인지 텍스트 인지 등을 알 수 없게 됩니다. 따라서 사용자는 포커스한 객체의 실행 결과를 전혀 예측할 수 없게 됩니다. 그러므로 스크린리더가 객체의 유형을 인식할 수 있는 정보를 제공해야 하며, 컨트롤 객체를 선택했을 때 스크린리더가 인식할 수 있도록 화면의 변경 내용을 출력해야 합니다.

