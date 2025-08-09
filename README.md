# web-socket-basic
웹 소켓 기초

## 목차
### [Chapter 01 웹 소켓 소개](#chapter-01-웹-소켓-소개)

#### [01-1 웹 소켓이란 무엇인가](chapters/01-1_what_is_websocket.md)
- 웹 소켓의 정의와 역할
- 기존 HTTP 통신과의 차이점
- 웹 소켓 프로토콜 개요
- 3가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [01-2 웹 소켓의 특징](chapters/01-2_websocket_characteristics.md)
- 양방향 통신
- 실시간 데이터 전송
- 단일 연결 유지
- 효율적인 프로토콜
- 크로스 도메인 통신
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [01-3 웹 소켓 지원 환경](chapters/01-3_websocket_support.md)
- 브라우저 호환성
  - 데스크톱 브라우저
  - 모바일 브라우저
- 폴리필과 대체 방안
- 기능 감지 방법
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 02 웹 소켓 기본 구현](#chapter-02-웹-소켓-기본-구현)
#### [02-1 웹 소켓 연결 설정](chapters/02-1_websocket_connection.md)
- 웹 소켓 URL 구조
- 서버 측 구현 (Java)
  - Jakarta WebSocket API (JSR-356)
  - Spring WebSocket
- 클라이언트 측 연결 설정 (TypeScript)
  - WebSocket 생성자
  - 이벤트 리스너 등록
- 연결 상태 관리
- 연결 종료 처리
- 자동 재연결 구현
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [02-2 메시지 송수신](chapters/02-2_message_exchange.md)
- 텍스트 메시지 전송
- 바이너리 데이터 전송
- 메시지 수신 처리
- 메시지 형식 및 직렬화
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [02-3 오류 처리 및 재연결](chapters/02-3_error_handling_reconnection.md)
- 일반적인 오류 유형
- 오류 이벤트 처리
- 재연결 전략 구현
- 지수 백오프 알고리즘
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 03 웹 소켓 프로토콜 심화](#chapter-03-웹-소켓-프로토콜-심화)
#### [03-1 웹 소켓 핸드셰이크](chapters/03-1_websocket_handshake.md)
- HTTP 업그레이드 메커니즘
- 핸드셰이크 요청 및 응답 헤더
- WebSocket 키 및 수락 과정
- 프로토콜 협상
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [03-2 프레임 구조 및 제어](chapters/03-2_frame_structure.md)
- 웹 소켓 프레임 형식
- 프레임 유형 (텍스트, 바이너리, 제어)
- 마스킹 메커니즘
- 프래그먼트화 및 메시지 조합
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [03-3 하트비트 및 연결 유지](chapters/03-3_heartbeat_connection.md)
- Ping/Pong 프레임
- 연결 타임아웃 처리
- 하트비트 구현 전략
- 연결 상태 모니터링
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 04 웹 소켓 보안](#chapter-04-웹-소켓-보안)
#### [04-1 웹 소켓 보안 위협](chapters/04-1_security_threats.md)
- 크로스 사이트 웹 소켓 하이재킹
- 인증 및 권한 부여 문제
- 메시지 주입 공격
- 서비스 거부 공격
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [04-2 보안 모범 사례](chapters/04-2_security_best_practices.md)
- WSS(WebSocket Secure) 사용
- 토큰 기반 인증
- 메시지 검증 및 필터링
- 속도 제한 및 스로틀링
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [04-3 웹 소켓 인증 구현](chapters/04-3_websocket_authentication.md)
- 세션 기반 인증
- JWT를 이용한 인증
- OAuth 통합
- 인증 상태 유지 관리
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 05 웹 소켓 확장 및 서브프로토콜](#chapter-05-웹-소켓-확장-및-서브프로토콜)
#### [05-1 웹 소켓 확장](chapters/05-1_websocket_extensions.md)
- 확장 메커니즘 개요
- 압축 확장 (permessage-deflate)
- 멀티플렉싱 확장
- 확장 협상 과정
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [05-2 STOMP 프로토콜](chapters/05-2_stomp_protocol.md)
- STOMP 개요 및 특징
- 프레임 구조
- 구독 및 발행 모델
- 트랜잭션 지원
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [05-3 MQTT 프로토콜](chapters/05-3_mqtt_protocol.md)
- MQTT 개요 및 특징
- 발행/구독 패턴
- QoS 레벨
- 주제 필터링
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 06 자바스크립트 및 프레임워크 통합](#chapter-06-자바스크립트-및-프레임워크-통합)
#### [06-1 React에서 웹 소켓 활용](chapters/06-1_websockets_in_react.md)
- React 컴포넌트 생명주기와 웹 소켓
- 커스텀 훅 구현
- 상태 관리와 웹 소켓 통합
- 실시간 UI 업데이트 패턴
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [06-2 Socket.IO 라이브러리](chapters/06-2_socketio_library.md)
- Socket.IO 소개
- 주요 기능 및 API
  - 이벤트 기반 통신
  - 룸과 네임스페이스
  - 자동 재연결
  - 폴백 메커니즘
- 클라이언트-서버 통합
- 6가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [06-3 Java 백엔드와 웹 소켓 연동](chapters/06-3_java_backend_integration.md)
- Spring WebSocket 지원
- STOMP 메시징 구현
- 보안 및 인증 처리
- 확장성 있는 아키텍처 설계
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [Chapter 07 웹 소켓 고급 주제](#chapter-07-웹-소켓-고급-주제)
#### [07-1 성능 최적화](chapters/07-1_performance_optimization.md)
- 메시지 크기 최적화
- 연결 풀링
- 바이너리 메시지 활용
- 확장성 있는 아키텍처
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [07-2 실시간 애플리케이션 패턴](chapters/07-2_realtime_application_patterns.md)
- 채팅 애플리케이션
- 실시간 대시보드
- 협업 편집기
- 멀티플레이어 게임
- 4가지 키워드로 정리하는 핵심 포인트
- 확인 문제

#### [07-3 디버깅 및 테스트](chapters/07-3_debugging_testing.md)
- 브라우저 개발자 도구
  - Chrome DevTools
  - Firefox DevTools
- 웹 소켓 디버깅 도구
- 자동화된 테스트 방법
- 부하 테스트 및 성능 분석
- 5가지 키워드로 정리하는 핵심 포인트
- 확인 문제

### [정답 및 해설](answers_and_explanations.md)
### 찾아보기
