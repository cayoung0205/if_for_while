### 제어문

- 조건문 : `if - else` 
- 반복문 : `for - in`, `while`
  - 루프 탈출: `break`, `continue`
- !!`들여쓰기` 중요!!

### 조건문

- 조건만족 여부에 따라 결과가 달라짐

```python
if <조건문> :
	<코드 블록>   ## 조건문의 코드블럭은 들여쓰기 한 후 작성!
    <코드 블록>   ## 조건문을 만족하면 실행
    <코드 블록>   ## 조건문을 만족X, 조건문 밖으로 skip
```

#### 단일 조건 및 그 외 조건

```python
if <조건문> :
	<코드블럭 1>

else :
	<코드블럭 2>
```

```python
if <조건문 1> :
	<코드블럭 1>

elif <조건문 1>
	<코드블럭 2>

else :
	<코드블럭 3>
```



### 반복문(for)

- 작업을 반복
- 범위를 지정 

```python
for <반복 변수> in <반복 범위> :

	<코드 블럭>
```

`range(stert, stop, step)` : 범위 지정

`len()`: 리스트의 길이

`zip()`: 같은 길이의 리스트를 묶음



#### 중첩 for 문

```python
for <반목 변수 1> in <반복 범위 1> :
	for <반복 변수 2> in <반복 범위 2> :
		<코드 블럭> ## 반복 변수 1, 반복 변수 2
```

- zip 함수

```python
for var1, var2 in zip(list1, list2) :
	<코드 블럭>
```



### 조건에 따라 반복 (while)

- 조건에 따라 반복 여부를 결정
- 반복 범위가 없을 때

```python
while <조건문> :  ## 조건문이 항상 참일 경우, 무한 루프
	<코드 블럭>
```

### roop 탈출 
### Break VS continue

> 반복문에서 빠져나오는 코드

#### Break

- 조건에 맞으면 코드에서 탈출
- **끝내기**

#### continue

- 조건에 맞으면 코드에서 탈출
- **재반복**



```python
k = 0
while True :
	k = k + 1 ## 1씩 값을 증가
	if(조건) :## 조건에 일치하면
		break ## if문을 빠져나옴
	print(출력내용)
```



```python
for <변수1> in <변수범위> :
	if <조건> : ## 조건과 일치하면
		continue ## 처음으로 돌아가서 다음 반복 실행
	
	print(<변수1>) ## 조건과 일치한 변수1만 빼고 출력
```



### 한 줄 for 문 (python)

- List comprehension

  `[<반복 실행문> for <반복 변수> in <반복 범위>]`

  `[<반복 실행문> for <반복 변수> in <반복 범위> if <조건문>]`

- Set comprehension

- Dictionary comprehension



