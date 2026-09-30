<div align="center">

# GangEun · 31%

[![Solved.ac Profile](https://mazassumnida.wtf/api/v2/generate_badge?boj=rkddms0420)](https://solved.ac/rkddms0420/)

</div>

<br />

## Open Source

### <img src="https://github.com/spring-projects.png" width="18" /> Spring

- **[spring-kafka#4727](https://github.com/spring-projects/spring-kafka/pull/4727)** Commit through the last record of the batch on `acknowledge()` after a partial ack, instead of throwing
- **[spring-amqp#3626](https://github.com/spring-projects/spring-amqp/pull/3626)** Wait for confirms on the captured physical channel instead of the proxy, so returned channels no longer leak

### <img src="https://github.com/celery.png" width="18" /> Celery

- **[celery#10667](https://github.com/celery/celery/pull/10667)** Keep a task cancelled by cold shutdown unacked, so it is requeued instead of lost
- **[celery#10715](https://github.com/celery/celery/pull/10715)** Release the Redis pubsub lock while waiting for messages, so `result.get()` under gevent no longer hangs
- **[celery#10679](https://github.com/celery/celery/pull/10679)** Skip the `REVOKED` write when a task already has a final result, so a chord `FAILURE` is not overwritten
- **[celery#10080](https://github.com/celery/celery/pull/10080)** Close only the fds that are actually open on `--detach`, removing minute-long stalls in containers
- **[py-amqp#466](https://github.com/celery/py-amqp/pull/466)** Serialize `frame_writer()` with a lock, so concurrent publishers no longer interleave frames

<details>
<summary><sub>+ 16 more</sub></summary>

- **[celery#10689](https://github.com/celery/celery/pull/10689)** Forward `propagate` to child results in native joins, so nested failures respect `propagate=False`
- **[celery#10676](https://github.com/celery/celery/pull/10676)** Add a smoke test workflow that runs against py-amqp, Kombu and billiard `main`
- **[celery#10682](https://github.com/celery/celery/pull/10682)** Adapt the consumer smoke tests to Kombu 5.7's per-consumer QoS
- **[celery#10674](https://github.com/celery/celery/pull/10674)** Wait for a new child pid in the respawn smoke test to remove a flake
- **[celery#10672](https://github.com/celery/celery/pull/10672)** Prepare any `BaseException` before encoding, so JSON backends store the failure
- **[celery#10623](https://github.com/celery/celery/pull/10623)** Make `app.conf.copy()` return a settings object that can be read
- **[celery#10610](https://github.com/celery/celery/pull/10610)** Exit the fallback context manager itself, not the value returned by `__enter__()`
- **[celery#10609](https://github.com/celery/celery/pull/10609)** Keep an explicitly supplied empty `Schedule` in `Timer`
- **[celery#10596](https://github.com/celery/celery/pull/10596)** Stop the execv flag from leaking between tests
- **[celery#10584](https://github.com/celery/celery/pull/10584)** Allow the `spawn` start method with the asynchronous prefork pool
- **[celery#10583](https://github.com/celery/celery/pull/10583)** Detect spawned pool children, so they run the worker initialisation
- **[celery#10076](https://github.com/celery/celery/pull/10076)** Document that `task_retry` signal args may be `None`
- **[billiard#462](https://github.com/celery/billiard/pull/462)** Reject `Pool` with fewer than one process instead of hanging forever
- **[billiard#457](https://github.com/celery/billiard/pull/457)** Exit the pool worker after `SystemExit`, so a hard time limit no longer stalls the pool
- **[billiard#456](https://github.com/celery/billiard/pull/456)** List the fd directory and close only open descriptors in `close_open_fds()`
- **[billiard#455](https://github.com/celery/billiard/pull/455)** Bind the `closerange()`-based `close_open_fds()` that never ran on Python 3

</details>

### <img src="https://github.com/pytest-dev.png" width="18" /> pytest

- **[pytest#15040](https://github.com/pytest-dev/pytest/pull/15040)** Mark editable-installed plugins for assertion rewriting

<br />

## Latest Posts

<!-- BLOG-POST-LIST:START -->
- [Celery 톺아보기](https://gangeunzzang.github.io/posts/celery%EB%9E%80/)
- [FastAPI 톺아보기](https://gangeunzzang.github.io/posts/fastapi%EB%9E%80/)
- [Dispatcher Servlet 톺아보기](https://gangeunzzang.github.io/posts/Dispatcher-Servlet-%ED%86%BA%EC%95%84%EB%B3%B4%EA%B8%B0/)
- [개인 프로젝트 MSA 전환 - &lpar;6&rpar; Circuit Breaker와 Fallback을 활용한 장애 복구](https://gangeunzzang.github.io/posts/MSA-%EA%B0%9C%EC%9D%B8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-MSA-%EC%A0%84%ED%99%98-(6)-Circuit-Breaker%EC%99%80-Fallback%EC%9D%84-%ED%99%9C%EC%9A%A9%ED%95%9C-%EC%9E%A5%EC%95%A0-%EB%B3%B5%EA%B5%AC/)
- [개인 프로젝트 MSA 전환 - &lpar;5&rpar; Config Server를 활용한 설정 관리](https://gangeunzzang.github.io/posts/MSA-%EA%B0%9C%EC%9D%B8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-MSA-%EC%A0%84%ED%99%98-(5)-Config-Server%EC%9D%84-%ED%99%9C%EC%9A%A9%ED%95%9C-%EC%84%A4%EC%A0%95-%EA%B4%80%EB%A6%AC/)<!-- BLOG-POST-LIST:END -->
