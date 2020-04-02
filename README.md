# lms-get


![demo](assets/demo.gif)

이러닝 문서 다운로더

## 용도

강의자료가 `.pptx`나 `.pdf`로 제공되지 않고 이러닝 강좌 게시판에서만 이용할 수 있게 되어 있나요?

이걸 쓰세요.

## 사용법

~~~
./lms-get <url> --token <token> --output <directory>
~~~

- `--token`: 로그인 토큰 (브라우저에서 `MoodleSession`으로 확인 가능).
- `--output`: 문서를 저장할 디렉토리. 없으면 새로 생성됨 (`mkdir -p` 사용)
