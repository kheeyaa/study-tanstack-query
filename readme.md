# TanStack Query

## 동기

기존 상태 관리 라이브러리는 클라이언트 상태를 관리하는데 적합합지만, 비동기 또는 서버 상태를 관리하는데엔 적합하지 않다.

### 서버 상태

- 사용자가 제어하거나 소유하지 않는 위치에서 원격으로 유지됨
- 가져오기 및 업데이트에 비동기 API 필요
- 공유 소유권을 의미하며 사용자 몰래 다른 사용자가 변경할 수 있음
- 주의하지 않으면 잠재적으로 애플리케이션에서 "오래된" 상태가 될 수 있음

어플리케이션에서 서버 상태 특성을 파악하면 다음과 같은 문제들을 직면할 수 있다.

- 캐싱 중... (프로그래밍에서 가장 어려운 작업임을 알 수 있음)
- 동일한 데이터에 대한 여러 요청을 단일 요청으로 중복 제거
- 백그라운드에서 "오래된" 데이터 업데이트
- 데이터가 "최신 버전이 아닌" 시기 파악
- 가능한 한 빨리 데이터 업데이트 반영
- 페이지네이션 및 느린 로드 데이터와 같은 성능 최적화
- 서버 상태의 메모리 및 가비지 컬렉션 관리
- 구조 공유를 사용하여 쿼리 결과 메모화

> TanStack Query는 서버 상태를 관리하는데 가장 적합한 라이브러리이다. 웹 응용 프로그램의 서버 상태 가져오기, 캐싱, 동기화 및 업데이트를 쉽게 수행할 수 있다.

TanStack Query는 다음과 같은 기능을 제공한다.

- 응용프로그램에서 복잡하고 잘못 이해된 코드의 많은 줄을 제거하고 몇 줄의 응답 쿼리 논리로 대체할 수 있습니다.
- 새로운 서버 상태 데이터 소스를 연결할 필요 없이 애플리케이션을 보다 안정적이고 쉽게 새로운 기능을 구축할 수 있습니다
- 애플리케이션이 그 어느 때보다 빠르고 응답성이 향상되어 최종 사용자에게 직접적인 영향을 미칩니다.
- 대역폭을 절약하고 메모리 성능을 향상시킬 수 있습니다

## 설치

```bash
$ npm i @tanstack/react-query
# or
$ pnpm add @tanstack/react-query
```

```bash
$ npm i @tanstack/react-query-devtools
# or
$ pnpm add @tanstack/react-query-devtools
```
