---
emoji: 👻
title: python 내장 함수
date: '2022-11-16 09:00:00'
author: coding-palette
tags: python
categories: python
---

파이썬의 내장 함수는 모듈이나 패키지를 가져오지 않고 바로 사용할 수 있는 함수입니다.

## 1.abs

어떤 숫자를 입력받았을 때, 그 숫자의 절댓값을 돌려주는 함수 입니다.

```python
print(abs(-10))
print(abs(10))

# Output:
# 10
# 10
```

## 2.all

반복 가능한 객체의 요소가 모두 참이면 True, 거짓이 하나라도 있으면 False를 돌려줍니다.

```python
print(all([1, 2, 3]))
print(all([1, 0, 3]))

# Output:
# True
# False
```

0은 거짓이므로 때문에 두 번째 프린트는 False를 리턴 합니다.

## 3.any

반복 가능한 객체의 요소가 하나라도 참이면 True를 돌려주고, x가 모두 거짓일 때에만 False를 돌려줍니다. all(x)의 반대라고 생각하시면 됩니다.

```python
print(any([1, 2, 0]))
print(any([0, ""]))

# Output:
# True
# False
```

0, "" 2개 모두 거짓이므로 두 번째 프린트는 False를 리턴 합니다.

## 4.chr

ASCII 코드값에 해당하는 문자를 반환 합니다.

```python
print(chr(97))

# Output:
# a
```

## 5.divmod

a를 b로 나눈 몫과 나머지를 튜플 형태로 돌려 줍니다.

```python
print(divmod(7, 2))

# Output:
# (3, 1)
```


## 6.filter

반복 가능한 객체에서 특정 조건에 맞는 요소만 가지고 옵니다.

```python
numbers = [1, 2, 3, 4, 5]

def check(v):
    return v > 3

result = list(filter(check, numbers))

print(f'필터된 값은 {result} 입니다.')

# Output:
# 필터된 값은 [4, 5] 입니다.
```

## 7.map

반복 가능한 객체의 요소를 지정된 함수로 처리한 뒤 map 객체를 반환 합니다.

```python
numbers = [1, 2, 3, 4, 5]

def change(v):
    return v + 1

result = list(map(change, numbers))

print(f'변경된 값은 {result} 입니다.')

# Output:
# 변경된 값은 [2, 3, 4, 5, 6] 입니다.
```




```toc

```