###### 2019년 3월 28일 수업 자료.

# 두 번째 교실

#### 키워드
`정수형`, `실수형`, `연산자`

## 숫자형
### 정수

양의 정수 (1, 2, 3, 4, 5, 6, 7 ...), 0 그리고 음의 정수 (-1,-2,-3,-4,-5,-6)를 **정수** 라고 합니다.

![수직선.png](https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Number-line.svg/1280px-Number-line.svg.png)

Python에서는 이러한 정수를 사용하기 위해서는 정수형(Integer)이라는 자료형을 사용해야 합니다.

```python
a = 123 
a = -178  
a = 0
```

### 실수

`/* to be added */`

## 연산자 


|종류|이름|기능|
|----|----|----|
|`+`|덧셈 연산자|두 수를 더합니다.|	
|`-`|뺄셈 연산자|앞의 숫자에서 뒤의 숫자를 뺍니다.|
|`/`|나눗셈 연산자|앞의 숫자에서 뒤의 숫자를 나눈 값을 계산합니다.<br>실수 (Double) 형을 반환합니다.|
|`%`|나머지 연산자|앞의 숫자에서 뒤의 숫자를 나눈 나머지를 계산합니다.|

### 사칙연산 

파이썬에서 사칙연산을 하기위해서는 아래와 같은 연산자를 사용해야 합니다.

```python
a = 3 # 대입
b = 4
print(a + b) # 덧셉입니다. 7이 나오게 됩니다.
print(a - b) # 덧셉입니다. -1이 나오게 됩니다.
print(a * b) # 곱셈입니다. 12가 나오게 됩니다.  
print(a / b) # 나눗셈입니다. 0.75가 나오게 됩니다.
```

### 나머지 연산자

```python
print(7 % 3) # 7을 3으로 나누면 몫은 2이고 나머지는 1입니다. 1이 출력됩니다. (7 = 3 * 2 + 1)  
print(3 % 7) # 3을 7로 나누면 몫은 0이고 나머지는 3입니다. 3이 출력됩니다. (3 = 7 * 0 + 3)
```

## 도전

점수들의 평균을 구해 출력해보기

|과목|점수|
|----|----|
|국어|85|
|영어|90|
|수학|100|

```python
국어 = 85
영어 = 90
수학 = 100

# 점수들의 평균을 구해 출력하기 위해서는 무엇이 들어가야할까요?

```


<details><summary>정답 확인하기</summary>
<p>

```python
print((국어 + 영어 + 수학)/3)
```
* test
</p>
</details>
