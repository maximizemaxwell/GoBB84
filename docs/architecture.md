# Directory Arch

```txt
GoBB84
 ├── go.mod                # Go 모듈 설정
 ├── go.sum                # 라이브러리 버전 관리
 ├── main.go               # BB84 실행 메인 프로그램
 ├── internal
 │    ├── quantum
 │    │    ├── quantum.go  # 기본 양자 연산 (Hadamard, 측정, 상태 벡터)
 │    │    ├── qgo.go      # QGo 라이브러리 래퍼 (QGo가 필요한 경우)
 │    ├── protocols
 │    │    ├── bb84.go     # BB84 프로토콜 로직 (Evelyn, Astra 통신)
 │    │    ├── e91.go      # (향후 확장) E91 프로토콜 로직
 │    ├── simulation
 │    │    ├── channel.go  # 양자 채널 (잡음 모델, 도청 시뮬레이션)
 │    │    ├── ias.go      # 도청자(Ias) 행동 모델
 │    ├── utils
 │    │    ├── logger.go   # 로깅 기능 (실험 기록)
 │    │    ├── config.go   # 설정 파일 로딩
 ├── tests
 │    ├── bb84_test.go     # BB84 기능 테스트
 │    ├── quantum_test.go  # 양자 연산 테스트
 ├── docs
 │    ├── architecture.md  # 프로젝트 설계 
 │    ├── usage.md         # 사용법 설명
 ├── README.md             # 프로젝트 설명
```