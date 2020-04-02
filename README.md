# lms-get


![demo](assets/demo.gif)

이러닝 문서 다운로더

## 용도

강의자료가 `.pptx`나 `.pdf`로 제공되지 않고 이러닝 강좌 게시판에서만 이용할 수 있게 되어 있나요?

그런데 다운로드가 막혀 있나요?

이걸 쓰세요.

## 지원하는 파일 확장자

- `ppt`
- `pptx`
- `pdf`

나머지는 나중에 추가될 지도 몰라요.

## 환경

리눅스에서 돌아갑니다.

다음 유틸리티를 사용합니다:

- `gnu-getopt`
- `curl`
- `grep`
- `awk`

## 사용법

~~~
./lms-get <content id> --token <token> --output <dirname>
~~~

- `content id`: 이러닝 자료 id. http://cyber.inu.ac.kr/mod/ubfile/viewer.php?id=(content id)의 형태로 링크에 포함되어 있음.
- `token`: 로그인 토큰 (브라우저에서 `MoodleSession`으로 확인 가능).
- `dirname`: 문서를 저장할 디렉토리. 없으면 새로 생성됨 (`mkdir -p` 사용)
