
2017.01.11 Homework
===================

##ActiveX가 무엇일까?
>####ActiveX는 재사용 가능한 객체지향 소프트웨어 구성요소 개발에 사용되는 기술이다.

COM(컴포넌트 오브젝트 모델)과 OLE(객체연결삽입)를 적용해 Web으로부터 다운로드 받은 컨텐츠들을 쓸때 ActiveX를 사용하며 이 전반적인 기술 또는 구현하는데 필요한 구성요소를 지칭한다. 흔히 국내에서 통용되는 ActiveX의 뜻은 이러한 개념보다도 ActiveX Control을 뜻하는 경우가 많다.


##국내 웹에 ActiveX가 정착되게 된 이유 및 배경

### 1.ActiveX Control이란?
>ActiveX를 이용해 만든 응용프프로그램으로 Internet Explorer에서 실행되는 ActiveX Control이다

ActiveX Control은 독립된 사용자 인터페이스를 가지는 COM서버로서 동작하며 주로 인터넷으로 배포하고 웹브라우저를 통해 실행된다. 따라서 웹브라우저의 역할을 넘어서 여러가지 기능을 자유롭게 수행할 수 있다는 큰 장점이 있다. 

### 2. 한국에서 자체 개발한 암호화 알고리즘 SEED

> 한국인터넷진흥원에서 1999년에 128비트급 블록암호 기술로 DES, AES와 유사한 대칭키 암호화 알고리즘을 개발하였다. 

이 암호화 알고리즘을 사용하여 국내 인터넷뱅킹이 시작되었는데 
웹브라우저에서 지원이 되지 않고 TLS/TTLS등의 라이브러리에도 존재하지 않아 이 SEED를 쓰기 위해 관련 라이브러리와 프로그램을 서비스제공자의 관점에서 편리한 ActiveX로 배포하여 쓰기 시작하였고 이것이 국내 ActiveX의 사용의 시작이 되었다.

### 3. ActiveX의 심각한 보안위협

ActiveX는 서비스 제공자의 입장에서 한번에 필요한 프로그램 배포 및 사용자의 데이터 수집에 용이하였다. 그러나 사용자의 동의 없이도 자동으로 설치되는 등의 심각한 보안 위협 또한 초래하였다. 일단 설치된 이후에는 서비스 제공자가 ActiveX를 통하여 사용자의 PC 자원을 마음대로 사용할 수 있는 기회가 되어 이를 악용하여 크래커들이 뿌린 악성코드 및 바이러스가 국내 사용자들의 PC에 창궐하게 되었다.

이후 MS에서는 Windows Vista부터 UAC(User Account Control)를 도입하여 자동실행, 설치 방지 등 ActiveX사용시 사용자에게 설치 알림을 하고 동의를 구하게 하여  문제를 해결하려 했으나 ActiveX를 사용하는 대부분의 웹사이트는 해당  ActiveX를 설치하지 않으면 웹사이트의 서비스를 제한하여 울며 겨자먹기로 설치할 수 밖에 없었으며 또한 ActiveX를 설치할때마다 동의를 구하는 UAC를 귀찮게 여겨 일반 사용자들로 하여금 UAC를 사용하지 않게 만드는 결과를 초래하였다.  


>참고 링크 : 	한국에서의 ActiveX문제점에 관한 웹툰
>
1. [http://minix.tistory.com/425](http://minix.tistory.com/425 "한국에서의 ActiveX문제점에 관한 웹툰(1/3)")(1/3)
2. [http://minix.tistory.com/426](http://minix.tistory.com/426 "한국에서의 ActiveX문제점에 관한 웹툰(2/3)")(2/3)
3. [http://minix.tistory.com/425](http://minix.tistory.com/427 "한국에서의 ActiveX문제점에 관한 웹툰(3/3)")(3/3)


##기술적 부채(Technical Debt)에 대해 알아보자
> 소프트웨어의 개발 단계에서 시간과 노력을 충분히 들여 개발하지 않으면 보이지 않는 일종의 `기술적 결핍`이 내재되게 되고 이는 차후에 더 큰 시간과 노력을 들여야 해결할 수 있게 되는 것을 뜻하는 말이다.


이는 1992년 Ward Cunningham이 기술자가 아닌 사람들에게 문제를 전달하기 위해 시작한 단어이다. 
보통 이는 EndUser에게 직접적인 가치를 제공하지 못하는 요소들로 구성되며 Ward Cunningham이 부채라는 단어를 쓴 이유는 이자가 급격히 늘어나기 때문이다. 대표적인 특징으로 빌린사람과 갚는 사람이 일치하지 않는다는 특성이 있다. 즉, 빌린사람은 개발자이며 갚아야 하는 사람은 유지보수 개발자이고 최종적으로는 프로젝트 오너라고 볼 수 있다. 
흔히 부채라는 것이 무조건 나쁜 개념이 아니듯 기술적인 부채 또한 비율을 적절히 유지해 나간다면 프로젝트 진행에 상당한 유연성을 가져다 주어 나쁘다고만 할 수 없다. 다만 부채는 부채인 만큼 시간에 따라 증가하게 되는 부분을 간과하지 않고 비율을 적절히 관리하여 프로젝트 진행에 도움을 줄 수 있다.
 


##위의 내용을 조사하면서 느낀 점

###_한국이 IT강국이라고 흔히 말하는 부분은 잘못된 것이다._ 


1990년대 후반 스타크래프트라는 무시무시한 게임의 등장으로 인해 많은 국민이 PC에 친숙해지게 되는 계기가 되었고 여기에 한국인 특유의 빨리빨리 정서가 가미되어 속도향상이 필요한 여러 IT요소(인터넷 속도, 컴퓨터의 성능  및 보급량) 가 따라서 발전하게 되었다. 이에 기업에서는 각종 인터넷 관련 서비스를 탄생시켰으며 전자상거래가 활성화 되었다.  이 중 대표적인 서비스가 은행의 **인터넷 뱅킹**이다. 

### 인터넷뱅킹의 태동
그러나 당시 안전한 금융거래를 위해서는 강력한 보안이 필수적이었지만, 웹브라우저에는 암호화 기능이 없어 KISA(한국정보보호진흥원)에서 SEED라는 암호화 기술을 개발하였고 이를 웹브라우저에 탑재하기 위해 ActiveX Control을 사용하였으며, 이는 곧 국내 표준이 되었으며 관련 법규도 생겼다.
>전자금융감독규정 제7조(공인인증서 사용기준) 모든 전자금융
거래에 있어 「전자서명법」에 의한 공인인증서를 사용하여야
한다. 다만 기술적ㆍ제도적으로 공인인증서 적용이 곤란한 전자
금융거래로 감독원장이 정하는 경우에는 그러하지 아니하다. 

여기까지 왔을때 뭔가 눈치 채이는게 있다. 그것은 바로 기업과 정부의 서비스 편의성에 의한 논리로 ActiveX가 이용되었다는 점이다. ActiveX Control에서 SEED의 안정성, 보안성은 차치하더라도 ActiveX를 이용하는 것 자체가 일반 시민들이 PC를 이용할때 보안을 항상 염두에 두어야 한다는 점을 잊게 하는데 크게 작용했다. 

그럼에도 불구하고 법적으로 아직도 암호화 통신이 필요한 전자상거래를 이용할때는 울며 겨자먹기로 자신의 PC에 보안프로그램(ActiveX와 비슷)을 받아들여야 하며 법령의 개정을 통해 바뀔 생각도 없어보인다.  

이는 기술적부채의 특징이 잘 적용되는 사례로 보인다. 