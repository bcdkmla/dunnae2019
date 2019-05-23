###### 2019년 4월 25일 수업 자료.

# 네 번째 교실

#### 키워드
``list``

## Python List

다른 언어에서의 **배열**이 Python에서는 `list`라는 형태로 존재합니다. `list`는 번호(`index`)와 번호에 대응하는 **데이터**들로 이루어진 자료구조를 의미합니다. Python `list`에서는 **다양한 종류**의 데이터들이 순차적으로 저장됩니다.

Python `list`는 **동적 배열 (Dynamic Array)** 의 개념으로 구현되어 프로그램 수행 도중 `list`에 새 항목들이 추가 또는 삭제 된다면 `list`의 크기 가 변동 됩니다. 
	
### Python `list`의 사용
Python `list`는 다음과 같은 방법을 통해서 만들 수 있습니다.

```python
a = [1, 3 , 5, 7]
```

Python `list`는 다양한 형태의 값들이 들어갈 수 있습니다.

```python
a=[1,'A',3.5,True]
```

그리고 `list` 안의 값을 불러오고 싶다면 `index`를 통해서 접근가능합니다.

```python
a=[1,'A',3.5,True]
print(a[0]) #  1
print(a[1]) # 'A'
print(a[2]) #  5
```

만약 `list` 자체를 보고 싶다면

```python
print(a)
```

와 같이 `print()` 를 이용해서 할 수 있습니다.

* 학생들에게 `index` 넘버가 `1`이 아닌 `0`부터 시작한다는 것을 확실하게 가르쳐 줄 것!

### Python `list`의 사용 2

* `list`에 새로운 값을 추가하기

```python
a = [3, 4, 5]
a.append(6)
print(a) # [3, 4, 5, 6]
```

* 다른 `list`를 연결하기

```python
a = [3, 4, 5]
b = [6, 7]
a.extend(b)
print(a) # [3, 4, 5, 6, 7]
```

* `list` 안에 새로운 값을 넣기

```python
a = [3, 4, 5]
a.insert(2, 7) # a.insert(index, obj)
print(a) # [3, 4, 7, 5]
```

### Python `list`의 사용 3
* `list`의 정렬
**sort** : Python `list`에서는 기본적으로 sort 함수를 이용해서 `list`를 오름차순(작은 값이 앞, 큰 값은 뒤)으로 정렬할 수 있습니다.

```python
a = [1,23,4,6,2]
a.sort()
print(a) # [1,2,4,6,23]
```

만약 오름차순이 아닌 내림차순으로 정렬을 하고 싶다면

```python
a = [1,23,4,6,2]
a.sort(reverse=True)
print(a) # [23,6,4,2,1]
```
처럼 `sort(reverse=True)`를 사용하면 됩니다.

## 다음 문제를 풀어 봅시다.

A 라는 `list`에는 5명의 학생들의 시험 점수가 다음과 같이 담겨 있습니다

```python
A= [90,88,92,78,95]
```

1. 학생들의 점수가 담긴 `list` A를 정렬해서 1등한 친구의 점수를 출력해 봅시다.
1. 그런데 어느날 2명의 친구가 전학을 와서 점수가 각각 98점, 70점이었습니다. `list` A에 새로 전학온 친구들의 점수를 추가하고 가장 점수가 낮은 친구와 가장 점수가 높은 친구의 점수를 출력해 봅시다.

* `list`의 출력
* `list`의 추가
* `list`의 정렬
* `list`의 `index` 번호

<details><summary>정답 확인하기</summary>
<p>

### 정답

```python
A = [90,88,92,78,95]

A.sort(reverse=True) # 내림차순으로 정렬.

print(A[0])

A.append(98)
A.append(70)

A.sort(reverse=True)

print(A[-1]) # 가장 낮은 점수. -1번째는 뒤에서 첫 번째를 뜻합니다.
print(A[0])  # 가장 높은 점수.
```

또는 `max(<list>)`나 `min(<list>)`를 사용하면 훨씬 간편하게 답을 구할 수 있습니다.

```python
A = [90,88,92,78,95]

print(max(A))

A.append(98)
A.append(70)

print(min(A)) # 가장 낮은 점수
print(max(A)) # 가장 높은 점수
```

</p>
</details>
