---
emoji: 👻
title: python 기초
date: '2022-09-03 21:00:00'
author: coding-palette
tags: python
categories: python
---

테스트를 하기 앞서 저는 이전 [파이썬 가상환경 만들기](https://codingpalette.com/python-venv/) 에서 코드를 작성하도록 하겠습니다.

`source venv/bin/activate` 으로 가상환경을 실행시켜 주시고 `main.py`라는 파일을 생성합니다.

생성이 완료 되었으면
```python
print('hello word') 
```
라고 입력한 뒤 터미널에서 `python main.py` 라고 입력하시고 아래 이미지 처럼 나오시면 정상적으로 준비가 완료 된 것 입니다.

![img1.png](img1.png)

아래 코드들을 입력하시고 확인하고 싶으시면 `python main.py` 라고 입력하시면 됩니다.

## 1.주석 및 프린트

### 1-1.주석
주석처리는 `#` 으로 하면 주석이 됩니다.
```python
# 이것은 주석 입니다.
```

### 1-2.프린트
프린트 출력은 `print()`으로 출력이 가능합니다.
```python
print('텍스트 출력')
# Output:
# 텍스트 출력 
```

## 2.변수

### 2-1.변수 할당
**cat_name**이라는 변수에 나비라는 문자열을 할당해 보겠습니다.
```python
cat_name = "나비"
print(cat_name)
# Output:
# 나비
```

### 2-2.숫자 계산
변수에 숫자를 담아 사칙연산을 해보도록 하겠습니다.
```python
a = 20
b = 10
print(a + b)
# Output:
# 30
```
- +: 더하기 연산
- -: 빼기 연산
- /: 나누기 연산
- *: 곱하기 연산
- //: 정수 나누기 연산 나눈 값을 내림해서 가져옵니다.
- %: 모듈러 연산 (Modulo Operator), 나눗셈의 나머지만 가져옵니다.
- **: 거듭제곱 연산

### 2-3.변수 + 텍스트 출력
변수와 텍스트를 합칠때는 앞에 `f' 입력 '`(한줄일 때) 또는 `f''' 입력 ''''`(여러줄일 때)를 활용하면 됩니다.

```python
cat = '고양이'
name = '나비'
cat_name = f'{cat} 이름은 {name} 입니다.'
print(cat_name)
# Output:
# 고양이 이름은 나비 입니다.
```

## 3.조건문
조건문에 들어가기전에 우션 비교연산이라는 것을 알아야 합니다.

a = 10, b = 20 이라고 하면

| Operator | Description            | Example          |
|:--------:|------------------------|------------------|
 |    ==    | 값이 동일하다                | (a == b) → false |
|    !=    | 값이 동일하지 않다             | (a != b) → true  |
|    >     | 왼쪽 값이 오른쪽 값보다 크다       | (a > b) → false  |
|    <     | 왼쪽 값이 오른쪽 값보다 작다       | (a < b) → true   |
|    >=    | 왼쪽 값이 오른쪽 값보다 크거나 동일하다 | (a >= b) → false |
|    <=    | 왼쪽 값이 오른쪽 값보다 작거나 동일하다 | (a <= b) → true  |


### 3-1.if
특정 값이 참일 때 출력하도록 해보겠습니다.
```python
number = 10
if number == 10:
    print('숫자는 10입니다.')
# Output:
# 숫자는 10입니다.
```
위 코드는 number 라는 변수에 10이라는 숫자가 들어가 있고 조건문에서 number는 10이라는 숫자와 동일하기 때문에 참이고 안쪽에 프린트가 출력 될 수가 있습니다.

### 3-2.else
여기서 특정 값이 아니라고 하면 아래처럼 하면 됩니다.
```python
number = 11
if number == 10:
    print('숫자는 10입니다.')
else:
    print('숫자는 10이 아닙니다.')
# Output:
# 숫자는 10이 아닙니다.
```

### 3-3.elif
조건을 여러 개 주는 것도 가능합니다.
```python
number = 12
if number == 10:
    print("숫자는 10입니다.")
elif number == 12:
    print("숫자는 12입니다.")
else:
    print("숫자는 10도 12도 아닙니다.")
# Output:
# 숫자는 12입니다.
```


```toc

```
