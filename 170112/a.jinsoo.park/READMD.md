##1. 국내에 공인인증서가 생긴 배경과 그 위험성은?

###탄생 배경

>태어나지 말았어야...

1999년 전자서명법의 발효로 11명의 암호학 교수들이 모여 연구를 시작한다. 고작 11명이 2 파벌로 나뉘어 싸우고 공인인증서의 전신인 범용 인증서가 먼저 사용된다. 문제가 끊임없이 제시되다가 2001년 전자 정부법이 발효되면서 공인인증서가 나타난다.

---

###위험성
공인인증서를 사용 가능하게 하는 모듈의 대부분이 ActiveX 기반이다. 하필 ActiveX를 이용하는 이유는 공인인증서 초기에는 SSL이 56비트 암호만을 지원했기 때문이다. 추후 128비트 기술이 공개되었지만 이미 고착화된 ActiveX를 계속 이용할 수 밖에 없었다.  
이것이 위험한 이유는 우선  ActiveX로 인해 Windows / IE에서만 사용가능하도록 만들어 졌다는 것이다. 이미 지원이 끊긴 고전 OS버젼의 보안성도 문제가 되고 ActiveX로 인해 사용자가 책임을 지게 된다는 점이다.


##2. 애플리케이션 접근성

###앱(애플리케이션) 접근성이란?
**모바일 기기**[^1]에서 사용되는 **모바일 애플리케이션**[^2]는 애플리케이션 서비스 제공자가 장애인, 고령자 등의 접근성을 보장하기 위해 지켜야 할 규정

###앱(애플리케이션)접근성의 현상황
최초 1.0 지침서에서는 7개의 준수사항과 8개의 권고사항이었으나 2.0에서 이를 통합, 수정하여 4개의 범용 준수사항과 19개의 세부 권고사항으로 이루어지게 되었다. 접근성을 높이기 위한 처우의 개선이 점차적으로 이루어지고 있는 실정이다.

---

[^1]: (입력 및 출력기능이 있고 무선 인터넷 서비스를 사용할 수 있는 휴대용 기기)
[^2]: (모바일 플랫폼 개발 언어로 제작된 응용프로그램 및 콘텐츠)