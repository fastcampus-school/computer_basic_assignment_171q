![ActiveX](http://www.activexcontrol.org/wp-content/uploads/2010/07/active-x-2-bb2.png)

1. ActiveX가 무엇일까?  
----
* 대한민국에서 IE를 어쩔수 없이 질리도록 써야하는 이유이자 만악의 근원이라 표현.
* 마이크로소프트에서 만든 COM(컴포넌트 오브젝트 모델)과 OLE(오브젝트 링킹 앤 임베딩) 기술 두 개를 합쳐서 이름을 새로 붙여준 것.
* 대부분 좁은 의미로 Internet Explorer에서 애드온으로 사용되는 ActiveX Control들을 말한다.
* 액티브X는 거대한 소프트웨어 프레임워크지만 대한민국에서는 '인터넷 익스플로러에 붙어서만 실행되는 윈도우 응용프로그램' 정도로 인식되는 것이 일반적이다.

2. 국내 웹에 ActiveX가 정착되게 된 이유 및 배경
----
* 한국에서 자체개발한 알고리즘 SEED
   - 한국인터넷진흥원(KISA)에서 1999년에 개발한 대칭키 암호화 알고리즘으로, 블록암호 기술로 인해 DES나 AES같은 암호 알고리즘과 친척뻘이다. 암호화키가 128비트라서 AES에 가깝다는 설명이 종종 있지만 실제로는 알고리즘 구조와 기술적으로 DES가 더 가까운 친척뻘이다.  
   - 1990년대 인터넷 뱅킹 등을 위하여 암호화 알고리즘을 사용하여야 헀지만, 당시 미국에서는 자체 기술보호를 위해 해외 접속으로 가능한 비트수를 40비트로 제한했고 우리나라(KISA)에서는 자체적으로 개발한 SEED 를 사용하여야 했다.  
   - 128비트급인 SEED가 개발되어 배포되고 이를 통해서 대한민국 인터넷 뱅킹이 시작되긴 했는데, 문제는 웹 브라우저에 당연히 지원도 안 되었고 주요 TLS/SSL 라이브러리에도 없었던 것이다. 그래서 SEED를 쓰기 위한 관련 라이브러리와 프로그램 배포를 위해서 ActiveX란 놈을 어거지로 이용하였으며, 이게 대한민국의 ActiveX 역사의 시작이 되었다.
   
3. ‘기술적 부채(Technical Debt)’에 대해 알아보기 
----
* 1992년 Ward Cunningham이 비 기술자들에게 문제를 전달하기 위해 사용하기 시작한 단어로, 간단히 말해 꼭 해 두지 않아도 또는 프로젝트가 끝날 때 까지(심지어는 끝나고 나서도) 티가 잘 나지 않는 작업들을 지칭한다.
* 간단히 말해서 기술자본이 많지않은 집단에서 당장의 이익과 빠른 개발을 위해서 포기하는 많은 것들(테스트 코드관리, CI, 품질관리 등)이 나중에는 부채(DEBT)로 들어온다는 개념이다.
* 하지만 무조건 잘못 된 것은 아니다. 당장 부채가 생긴다 하더라도 이를 인지하고 나중에 갚겠다는 생각과 책임으로 개발을 한다면 비교적 시간적여유와 기술력이 떨어지는 회사에서는 고려할만 한 상황이 될 수 있다.

4. 위 내용을 조사하며 느낀 점 
----
* ActiveX에 대해서 약간은 부정적인 생각을 갖고 있었지만 생각보다 더 욕을 많이 먹고 있는 현실을 알았습니다.
* 맥 유저로서 ActiveX가 빨리 없어졌으면 합니다.
* 전에 프로젝트를 하면서 당장의 이익과 편의를 위해 기술적 부채를 만들었었던 것 같은데, 기술적 부채의 개념을 알고나서는 조금더 개념 찬 개발을 할 수 있을 것 같습니다.