---
emoji: ๐ป
title: python ๊ธฐ์ด2
date: '2022-09-04 21:00:00'
author: coding-palette
tags: python
categories: python
---



## 1.๋ฆฌ์คํธ

๋ฆฌ์คํธ๋ ์ฌ๋ฌ ์์๋ค์ ๊ฐ๋ ์งํฉ(์ปฌ๋ ์)์ผ๋ก ์๋ก์ด ์์๋ฅผ ์ถ๊ฐํ๊ฑฐ๋ ๊ฐฑ์ , ์ญ์ ํ๋ ์ผ์ด ๊ฐ๋ฅํฉ๋๋ค.

ํ์ด์ฌ์ ๋ฆฌ์คํธ๋ ๋์ ๋ฐฐ์ด(Dynamic Array)๋ก์ ์์ ๋กญ๊ฒ ํ์ฅํ  ์ ์๋ ๊ตฌ์กฐ๋ฅผ ๊ฐ์ง๊ณ  ์์ต๋๋ค.

๋ฆฌ์คํธ๋ ๊ทธ ์์ ์์(element)๋ค์ ๊ทธ ๊ฐ์ ์์ ๋กญ๊ฒ ๋ณ๊ฒฝํ  ์ ์๋ Mutable ๋ฐ์ดํฐ ํ์์๋๋ค.

### 1-1.๋ฆฌ์คํธ ๋ง๋ค๊ธฐ
๋ฆฌ์คํธ๋ฅผ ์ฌ์ฉํ๋ฉด 1, 3, 5, 7, 9 ์ซ์ ๋ชจ์์ ๋ค์๊ณผ ๊ฐ์ด ๊ฐ๋จํ๊ฒ ํํํ  ์ ์์ต๋๋ค.
```python
number_list = [1,2,3,7,9]
```

### 1-2.๋ฆฌ์คํธ ๊ฐ ์ฐพ๊ธฐ
๋ช ๋ฒ์งธ ๋ฆฌ์คํธ์ ์ด๋ค ๊ฐ์ด ์๋์ง ์๋ ค๋ฉด ์๋์ ๊ฐ์ด ํด์ฃผ์๋ฉด ๋ฉ๋๋ค.
```python
a = [1,2,3,4]
print('a์ 0๋ฒ์งธ ๊ฐ์', a[0], '์๋๋ค.')
# Output:
# a์ 0๋ฒ์งธ ๊ฐ์ 1 ์๋๋ค.
```

```python
a = [1,2,3,4]
print('a์ 1~2๋ฒ์งธ ๊ฐ์', a[0:2], '์๋๋ค.')
# Output:
# a์ 1~2๋ฒ์งธ ๊ฐ์ [1, 2] ์๋๋ค.
```

```python
a = [1,2,3,4]
print('a์ ๋ค์์ 2๋ฒ์งธ ๊ฐ์', a[-2], '์๋๋ค.')
# Output:
# a์ ๋ค์์ 2๋ฒ์งธ ๊ฐ์ 3 ์๋๋ค.
```

### 1-3.๋ฆฌ์คํธ ์ฐ์ฐํ๊ธฐ
๋ฆฌ์คํธ ๋ํ๊ธฐ
```python
a = [1, 2, 3]
b = [4, 5, 6]
print(a + b)
# Output:
# [1, 2, 3, 4, 5, 6]
```

๋ฆฌ์คํธ ๋ฐ๋ณตํ๊ธฐ
```python
a = [1, 2, 3]
print(a * 3)
# Output:
# [1, 2, 3, 1, 2, 3, 1, 2, 3]
```

๋ฆฌ์คํธ ๊ธธ์ด ๊ตฌํ๊ธฐ
```python
a = [1, 2, 3]
print(len(a))
# Output:
# 3
```

ํน์  ๊ฐ์๊ฐ ๋ช๊ฐ์ธ์ง ๊ตฌํ๊ธฐ
```python
a = [1, 2, 3, 4, 1]
print(a.count(1))
# Output:
# 2
```

ํน์  ๊ฐ์ด ๋ช๋ฒ์งธ์ ์๋์ง ๊ตฌํ๊ธฐ
```python
a = [1, 2, 3, 4]
print(a.index(3))
# Output:
# 2
```

### 1-4.๋ฆฌ์คํธ ์ถ๊ฐ,์์ ,์ญ์ 
append ๋ก ๋ฆฌ์คํธ ์ถ๊ฐ

append(x)๋ ๋ฆฌ์คํธ์ ๋งจ ๋ง์ง๋ง์ x๋ฅผ ์ถ๊ฐํ๋ ํจ์ ์๋๋ค.
```python
a = [1, 2, 3]
a.append(4)
print(a)
# Output:
# [1, 2, 3, 4]
```
insert ๋ก ๋ฆฌ์คํธ ์ถ๊ฐ

insert(a, b)๋ ๋ฆฌ์คํธ์ a๋ฒ์งธ ์์น์ b๋ฅผ ์ฝ์ํ๋ ํจ์ ์๋๋ค.
```python
a = [1, 2, 3]
a.insert(0, 4)
print(a)
# Output:
# [4, 1, 2, 3]
```

๋ฆฌ์คํธ ํ์ฅํ๊ธฐ

extend(x)์์ x์๋ ๋ฆฌ์คํธ๋ง ์ฌ ์ ์์ผ๋ฉฐ ์๋์ a ๋ฆฌ์คํธ์ x ๋ฆฌ์คํธ๋ฅผ ๋ํฉ๋๋ค.
```python
a = [1, 2, 3]
a.extend([4, 5])
print(a)
# Output:
# [1, 2, 3, 4, 5]
```

๋ฆฌ์คํธ์์ ๊ฐ ์์ ํ๊ธฐ
```python
a = [1, 2, 3, 4]
a[1] = 7
print(a)
# Output:
# [1, 7, 3, 4]
```

del ํจ์๋ฅผ ์ด์ฉํ์ฌ ์ญ์ ํ๊ธฐ
```python
a = [1, 2, 3, 4]
del a[1]
print(a)
# Output:
# [1, 3, 4]
```

### 1-5.๋ฆฌ์คํธ ์ ๋ ฌ, ๋ค์ง๊ธฐ
sort ํจ์๋ ๋ฆฌ์คํธ์ ์์๋ฅผ ์์๋๋ก ์ ๋ ฌํด ์ค๋๋ค.
```python
a = [1, 4, 3, 2]
a.sort()
print(a)
# Output:
# [1, 2, 3, 4]
```

reverse ํจ์๋ ๋ฆฌ์คํธ๋ฅผ ์ญ์์ผ๋ก ๋ค์ง์ด ์ค๋๋ค.
```python
a = ['a', 'c', 'b']
a.reverse()
print(a)
# Output:
# ['b', 'c', 'a']
```

## 2.ํํ
Tuple์ ๋ฆฌ์คํธ์ ๋น์ทํ๊ฒ ์ฌ๋ฌ ์์๋ค์ ๊ฐ๋ ์ปฌ๋ ์ ์๋๋ค.

๋ฆฌ์คํธ์ ๋ค๋ฅธ ์ ์ Tuple์ ์๋ก์ด ์์๋ฅผ ์ถ๊ฐํ๊ฑฐ๋ ๊ฐฑ์ , ์ญ์ ํ๋ ์ผ์ ํ  ์ ์์ต๋๋ค.

### 2-1.ํํ๊ณผ ๋ฆฌ์คํธ์ ๋ค๋ฆ์ 
- ๋ฆฌ์คํธ๋ [ ]์ผ๋ก ๋๋ฌ์ธ์ง๋ง ํํ์ ( )์ผ๋ก ๋๋ฌ์ผ๋ค.
- ๋ฆฌ์คํธ๋ ๊ทธ ๊ฐ์ ์์ฑ, ์ญ์ , ์์ ์ด ๊ฐ๋ฅํ์ง๋ง ํํ์ ๊ทธ ๊ฐ์ ๋ฐ๊ฟ ์ ์๋ค.

### 2-2.ํํ ๋ง๋ค๊ธฐ
```python
t1 = ()
t2 = (1,)
t3 = (1, 2, 3)
t4 = 1, 2, 3
t5 = ('a', 'b', ('ab', 'cd'))
```

๋ฆฌ์คํธ์ ๋ชจ์ต์ ๊ฑฐ์ ๋น์ทํ์ง๋ง ํํ์์๋ ๋ฆฌ์คํธ์ ๋ค๋ฅธ 2๊ฐ์ง ์ฐจ์ด์ ์ ์ฐพ์๋ณผ ์ ์์ต๋๋ค.

t2 = (1,)์ฒ๋ผ ๋จ์ง 1๊ฐ์ ์์๋ง์ ๊ฐ์ง ๋๋ ์์ ๋ค์ ์ฝค๋ง(,)๋ฅผ ๋ฐ๋์ ๋ถ์ฌ์ผ ํ๋ค๋ ๊ฒ๊ณผ t4 = 1, 2, 3์ฒ๋ผ ๊ดํธ( )๋ฅผ ์๋ตํด๋ ๋ฌด๋ฐฉํ๋ค๋ ์ ์๋๋ค.

ํํ์ ๊ฐ์ ๋ณํ์ํฌ ์ ์๋ค๋ ์ ๋ง ์ ์ธํ๋ฉด ๋ฆฌ์คํธ์ ์์ ํ ๋์ผํฉ๋๋ค.

## 3.๋์๋๋ฆฌ
๋์๋๋ฆฌ๋ "ํค(Key) - ๊ฐ(Value)" ์์ ์์๋ก ๊ฐ๋ ์ปฌ๋ ์ ์๋๋ค.

๋์๋๋ฆฌ๋ ํํ Map ์ด๋ผ๊ณ ๋ ๋ถ๋ฆฌ์ฐ๋๋ฐ, ํค(Key)๋ก ์ ์ํ๊ฒ ๊ฐ(Value)์ ์ฐพ์๋ด๋ ํด์ํ์ด๋ธ(Hash Table) ๊ตฌ์กฐ๋ฅผ ๊ฐ์ง๊ณ  ์์ต๋๋ค.

์๋ฐ์คํฌ๋ฆฝํธ์ object๋ผ๊ณ  ์๊ฐํ์๋ฉด ํธํฉ๋๋ค.

### 3-1.๋์๋๋ฆฌ ๋ง๋ค๊ธฐ
```python
dic = {"name": "ํ๊ธธ๋", "age": 25, "phone": "010-000"}
print(dic)
# Output:
# {'name': 'ํ๊ธธ๋', 'age': 25, 'phone': '010-000'}
```

๋์๋๋ฆฌ dic์ ์ ๋ณด

|  key   | 	value  |
|:------:|:-------:|
|  name  |   ํ๊ธธ๋   |
|  age	  |   25    |
| phone	 | 010-000 |

### 3-2.๋์๋๋ฆฌ ๊ฐ ์ฐพ๊ธฐ
๋์๋๋ฆฌ์ ๊ฐ์ key๋ฅผ ์ด์ฉํด์ ์ฐพ์ ์ ์์ต๋๋ค.
```python
dic = {"name": "ํ๊ธธ๋", "age": 25, "phone": "010-000"}
print(dic["name"])
# Output:
# ํ๊ธธ๋
```

### 3-3.๋์๋๋ฆฌ ์ถ๊ฐ,์์ ,์ญ์ 
์ถ๊ฐ ๋ฐฉ๋ฒ
```python
dic = {"name": "ํ๊ธธ๋", "age": 25, "phone": "010-000"}
dic["gender"] = "man"
print(dic)
# Output:
# {'name': 'ํ๊ธธ๋', 'age': 25, 'phone': '010-000', 'gender': 'man'}
```

์์  ๋ฐฉ๋ฒ
```python
dic = {"name": "ํ๊ธธ๋", "age": 25, "phone": "010-000"}
dic["age"] = 30
print(dic)
# Output:
# {'name': 'ํ๊ธธ๋', 'age': 30, 'phone': '010-000'}
```

์ญ์  ๋ฐฉ๋ฒ
```python
dic = {"name": "ํ๊ธธ๋", "age": 25, "phone": "010-000"}
del dic["phone"]
print(dic)
# Output:
# {'name': 'ํ๊ธธ๋', 'age': 25}
```



```toc

```
