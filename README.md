# e-learning-download
이러닝 문서 다운로더

## 사용법

~~~
./lms-get <url> --output <directory> --cookie <sessionid>
~~~

- `--output`: 문서를 저장할 디렉토리. 없으면 새로 생성됨(`mkdir -p` 사용)
- `--cookie`: 로그인 세션 id(브라우저에서 `MoodleSession`으로 확인 가능)
