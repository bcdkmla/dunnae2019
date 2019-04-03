###### 2019년 3월 21일 수업 자료.

# 첫 번째 교실

#### 키워드
`Python 설치`, `인터프리터 대화형 모드`, `Turtle Demo`

## Python의 기초

### Python의 설치

> 둔내초등학교 컴퓨터실은 Windows 컴퓨터만 있는 관계로, 앞으로의 모든 내용은 Windows를 기준으로 서술될 예정입니다.

1. [Python 홈페이지](https://www.python.org)에 접속합니다.
   * [Windows Python Download](https://www.python.org/downloads/windows/)
   * [macOS Python Download](https://www.python.org/downloads/mac-osx/)
1. 원하는 버전의 Python 설치 프로그램 중 다음의 표를 참고해서 알맞는 Python 설치 프로그램을 내려 받습니다.

|Windows|다운로드할 파일|
|----|----|
|64 bit|Windows x86-64 executable installer|
|32 bit|Windows x86 executable installer|

1. 다운로드가 끝나면 그 파일을 실행시킵다.
1. 설치 창에서 다음 항목들이 선택된 것을 확인하고 `Install Now`를 누릅니다. Path에 추가하는 이유는 `cmd.exe`에서 Python을 바로 실행시킬 수 있기 때문입니다.
   * `Add Python to PATH`
   * `Install launcher for all users`
1. 설치가 끝나고 나면 `Disable path length limit`을 누릅니다. Windows의 글자 수 제한을 막기 위해서 입니다.
1. 모든 설치가 종료되면 `Close` 버튼을 클릭하여 창을 닫습니다.

### Sublime Text의 설치
* [Sublime Text](https://www.sublimetext.com) 홈페이지에 접속하여 Sublime Text를 설치합니다.

### 그 외에 하면 좋은 것들
* Windows 탐색기를 열어 파일 확장자를 항상 표시하도록 해둡니다.
* `.py` 확장자를 Sublime Text로 항상 열도록 설정해둡니다.

## 인터프리터: Hello, World!

1. `cmd.exe`를 실행해 `python`을 작성하고 `enter`을 누릅니다.
1. 다음과 같은 내용이 보일 것입니다.

	```console
	/* 버전 정보, OS 정보 */
	Type "help", "copyright", "credits" or "license" for more 	information.
	>>>
	```

1. 이를 Python Interpreter라고 합니다. 우리는 지금 Python Interpreter를 대화형 모드로 사용하고 있는 것입니다. 대화형 모드는 말 그대로 컴퓨터와 우리가 대화하듯이 상호 작용한다는 것입니다.

	```console
	Type "help", "copyright", "credits" or "license" for more information.
	>>> 1+1
	2
	```

1. `print()`는 `cmd.exe` 같은 `console`에 무언가를 출력하는 `프린터` 같은 도구입니다.
1. 즉, 우리가 `Python`에게 `print()`를 이용해서 무언가를 출력하라고 할 수 있습니다.
1. 대신 우리가 출력하고 싶은 말을 할 때는`''`나 `""`를 이용해 우리가 말하고 싶은 부분을 표시해줘야 합니다.
1. 만약 "안녕하세요!"를 인쇄하고 싶다면, 인터프리터에 다음과 같이 작성해보세요.

	```console
	Type "help", "copyright", "credits" or "license" for more information.
	>>> print("안녕하세요!")
	안녕하세요!
	```

### 도전 과제
* 자신의 이름을 출력해보기
* 자기가 가장 좋아하는 동물을 출력해보기
* 자기가 좋아하는 동물을 출력하고, 바로 옆에 다시 좋아하는 식물을 출력하기.


<details><summary>정답 확인하기</summary>
<p>

```python
print("조성현")
print("고양이")
print("고양이", "선인장")
```
</p>
</details>

## Python 파일 실행하기
1. `cmd.exe`를 엽니다.
1. 자신이 열고자 하는 `Python` 파일의 폴더로 이동합니다.
1. 다음 명령어들을 사용하면 편리합니다.

	|명령어|기능|
	|----|----|
	|`dir`|현재 폴더 안에 들어있는 모든 파일을 출력합니다.|
	|`cd ` + NAME | 이 폴더 내에 존재하는 폴더 중 'NAME'이라는 이름을 가지는 폴더로 이동합니다.|
	|`cd ..` | 상위 폴더로 이동합니다.|

1. `python (파일 이름).py` 라고 입력히고 Enter 키를 누릅니다.
1. `Python` 파일이 실행되는 것을 볼 수 있습니다.

### 도전 과제
* 미리 `dunnae2019` Repository를 저장해두었다고 할 때, `Snowflake.py`를 실행해보기.

<details><summary>정답 확인하기</summary>
<p>

`dunnae2019` Repository가 바탕화면에 `git clone` 되어 있다고 할 때,

```console
$ cd Desktop
$ cd dunnae2019
$ cd Snowflake
$ python Snowflake.py
```
</p>
</details>

