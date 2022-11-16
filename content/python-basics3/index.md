---
emoji: 👻
title: python 기초3
date: '2022-09-05 21:00:00'
author: coding-palette
tags: python
categories: python
---

## 1.while

반복해서 문장을 수행해야 할 경우 while문을 사용합니다. 그래서 while문을 반복문이라고도 부릅니다.

### 1-1.while 기본구조
```python
while <조건문>:
    <수행할 문장1>
    <수행할 문장2>
    <수행할 문장3>
```
```python
index = 0
result = 0

while index < 100:
    index += 1
    result = result + index

print(f'index 값은 {index} 입니다.')
print(f'result 값은 {result} 입니다.')
# Output:
# index 값은 100 입니다.
# result 값은 5050 입니다.
```

### 1-2.while break
while문은 조건문이 참인 동안 계속해서 while문 안의 내용을 반복적으로 수행합니다. 하지만 강제로 while문을 빠져나가고 싶을 때가 있으면 break를 이용하면 됩니다.

```python
index = 0
result = 0

while index < 100:
    index += 1
    if index % 2 == 0:
        result = result + index

    if result > 1000:
        break


print(f'index 값은 {index} 입니다.')
print(f'result 값은 {result} 입니다.')
# Output:
# index 값은 64 입니다.
# result 값은 1056 입니다.
```
result_even 는 짝수만 더하다가 더한 결과 값이 1000을 넘었을때 break가 걸리도록 하는 코드 입니다.

### 1-2.while continue
while 반복문을 돌다가 특정 조건을 만족할때, 아래 코드는 무시하고 바로 반복문의 맨위로 올라가고 싶을때가 있을 수 있습니다.
즉 중간에서 바로 맨 처음으로 올라가는 기능을 하는, 키워드 continue 입니다.

```python
index = 0
result = 0

while index < 100:
    index += 1
    if index % 2 == 1:
        continue

    result = result + index

print(f'index 값은 {index} 입니다.')
print(f'result 값은 {result} 입니다.')
# Output:
# index 값은 100 입니다.
# result 값은 2550 입니다.
```


## 2.for
for문은 while문과 달리 지정한 횟수만큼을 반복할 때 주로 사용됩니다.

리스트, 문자열, 튜플 등 컬랙션 타입의 아이템을 하나씩 순회하면서 사용합니다.

for문의 기본 구조는 아래와 같습니다.

```python
for 변수 in 리스트(또는 튜플, 문자열):
    수행할 문장1
    수행할 문장2
    ...
```

### 2-1.for 기본
```python
rainbow = ['Red', 'Orange', 'Yellow', 'Green', 'Blue', 'Indigo', 'Violet']

for color in rainbow:
    print(f'컬러는 {color} 입니다.')
    
# Output:
# 컬러는 Red 입니다.
# 컬러는 Orange 입니다.
# 컬러는 Yellow 입니다.
# 컬러는 Green 입니다.
# 컬러는 Blue 입니다.
# 컬러는 Indigo 입니다.
# 컬러는 Violet 입니다.
```

### 2-2.for에서 index 사용, enumerate
```python
rainbow = ['Red', 'Orange', 'Yellow', 'Green', 'Blue', 'Indigo', 'Violet']

for index, color in enumerate(rainbow):
    print(f'인덱스는 {index} 입니다.')
    print(f'컬러는 {color} 입니다.')
    
# Output:
# 인덱스는 0 입니다.
# 컬러는 Red 입니다.
# 인덱스는 1 입니다.
# 컬러는 Orange 입니다.
# 인덱스는 2 입니다.
# 컬러는 Yellow 입니다.
# 인덱스는 3 입니다.
# 컬러는 Green 입니다.
# 인덱스는 4 입니다.
# 컬러는 Blue 입니다.
# 인덱스는 5 입니다.
# 컬러는 Indigo 입니다.
# 인덱스는 6 입니다.
# 컬러는 Violet 입니다.

```



```toc

```




