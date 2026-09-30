<div align="center">

# GangEun · 31%

[![Solved.ac Profile](https://mazassumnida.wtf/api/v2/generate_badge?boj=rkddms0420)](https://solved.ac/rkddms0420/)

</div>

<br />

## Open Source

### <img src="https://github.com/spring-projects.png" width="18" /> Spring

- **[spring-kafka#4727](https://github.com/spring-projects/spring-kafka/pull/4727)** 배치 리스너에서 부분 ack 후 `acknowledge()`가 배치 끝까지 커밋하지 않고 예외를 던지던 문제
- **[spring-amqp#3626](https://github.com/spring-projects/spring-amqp/pull/3626)** confirm 대기 중인 채널을 반납할 때 채널이 누수되던 문제

### <img src="https://github.com/celery.png" width="18" /> Celery

- **[celery#10667](https://github.com/celery/celery/pull/10667)** cold shutdown 때 실행 중이던 태스크가 재큐잉되지 않고 유실되던 회귀
- **[celery#10715](https://github.com/celery/celery/pull/10715)** gevent 환경에서 Redis 결과 백엔드의 `result.get()`이 timeout을 무시하고 멈추던 문제
- **[celery#10679](https://github.com/celery/celery/pull/10679)** chord 실패로 저장한 `FAILURE`를 뒤늦은 revoke가 `REVOKED`로 덮어쓰던 경쟁 조건
- **[celery#10080](https://github.com/celery/celery/pull/10080)** fd 한도가 큰 컨테이너에서 `--detach`가 수 분간 멈추던 문제
- **[py-amqp#466](https://github.com/celery/py-amqp/pull/466)** 한 커넥션에서 여러 스레드가 publish하면 프레임이 뒤섞여 전송되던 문제

<details>
<summary><sub>+ 16 more</sub></summary>

- **[celery#10689](https://github.com/celery/celery/pull/10689)** 중첩 group에서 `get(propagate=False)`가 예외를 던지던 문제
- **[celery#10676](https://github.com/celery/celery/pull/10676)** py-amqp·Kombu·billiard `main`으로 도는 스모크 테스트 워크플로 추가
- **[celery#10682](https://github.com/celery/celery/pull/10682)** Kombu 5.7의 per-consumer QoS에 맞춰 consumer 스모크 테스트 수정
- **[celery#10674](https://github.com/celery/celery/pull/10674)** respawn 스모크 테스트의 간헐 실패 수정
- **[celery#10672](https://github.com/celery/celery/pull/10672)** `BaseException`으로 실패한 태스크 결과가 JSON 직렬화 오류로 저장되지 않던 문제
- **[celery#10623](https://github.com/celery/celery/pull/10623)** `app.conf.copy()`로 복사한 설정을 읽으면 `TypeError`가 나던 문제
- **[celery#10610](https://github.com/celery/celery/pull/10610)** `FallbackContext`가 `with` 본문 실행 전에 리소스를 정리하던 문제
- **[celery#10609](https://github.com/celery/celery/pull/10609)** 빈 `Schedule`을 넘기면 `Timer`가 무시하던 문제
- **[celery#10596](https://github.com/celery/celery/pull/10596)** 테스트 사이로 execv 플래그가 새던 순서 의존성 제거
- **[celery#10584](https://github.com/celery/celery/pull/10584)** 비동기 prefork 풀에서도 `spawn` 시작 방식 허용
- **[celery#10583](https://github.com/celery/celery/pull/10583)** macOS 기본 `spawn`으로 뜬 풀 자식이 초기화를 건너뛰던 문제
- **[celery#10076](https://github.com/celery/celery/pull/10076)** `task_retry` 시그널 인자가 `None`일 수 있음을 문서화
- **[billiard#462](https://github.com/celery/billiard/pull/462)** 프로세스 수가 1 미만인 `Pool` 생성 거부 (0이면 영원히 대기)
- **[billiard#457](https://github.com/celery/billiard/pull/457)** 하드 타임리밋 후 워커가 종료되지 않아 풀이 멈추던 회귀
- **[billiard#456](https://github.com/celery/billiard/pull/456)** 실제로 열린 fd만 골라 닫도록 `close_open_fds()` 개선
- **[billiard#455](https://github.com/celery/billiard/pull/455)** Python 3에서 한 번도 안 쓰이던 `closerange()` 경로 복구

</details>

### <img src="https://github.com/pytest-dev.png" width="18" /> pytest

- **[pytest#15040](https://github.com/pytest-dev/pytest/pull/15040)** editable 설치된 플러그인에 assertion rewriting이 적용되지 않던 문제

<br />

## Latest Posts

<!-- BLOG-POST-LIST:START -->
<!-- BLOG-POST-LIST:END -->
