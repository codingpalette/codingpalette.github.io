---
emoji: π»
title: python μ½λ©νμ€νΈ - μ κ³  κ²°κ³Ό λ°κΈ°
date: '2022-09-19 16:00:00'
author: coding-palette
tags: python μ½λ©νμ€νΈ
categories: python μ½λ©νμ€νΈ
---

## 1.μ κ³  κ²°κ³Ό λ°κΈ° λ¬Έμ  μ€λͺ

μ μμ¬μ λ¬΄μ§λ κ²μν λΆλ μ΄μ©μλ₯Ό μ κ³ νκ³  μ²λ¦¬ κ²°κ³Όλ₯Ό λ©μΌλ‘ λ°μ‘νλ μμ€νμ κ°λ°νλ € ν©λλ€. λ¬΄μ§κ° κ°λ°νλ €λ μμ€νμ λ€μκ³Ό κ°μ΅λλ€.

κ° μ μ λ ν λ²μ ν λͺμ μ μ λ₯Ό μ κ³ ν  μ μμ΅λλ€.

μ κ³  νμμ μ νμ μμ΅λλ€. μλ‘ λ€λ₯Έ μ μ λ₯Ό κ³μν΄μ μ κ³ ν  μ μμ΅λλ€.

ν μ μ λ₯Ό μ¬λ¬ λ² μ κ³ ν  μλ μμ§λ§, λμΌν μ μ μ λν μ κ³  νμλ 1νλ‘ μ²λ¦¬λ©λλ€.

kλ² μ΄μ μ κ³ λ μ μ λ κ²μν μ΄μ©μ΄ μ μ§λλ©°, ν΄λΉ μ μ λ₯Ό μ κ³ ν λͺ¨λ  μ μ μκ² μ μ§ μ¬μ€μ λ©μΌλ‘ λ°μ‘ν©λλ€.

μ μ κ° μ κ³ ν λͺ¨λ  λ΄μ©μ μ·¨ν©νμ¬ λ§μ§λ§μ νκΊΌλ²μ κ²μν μ΄μ© μ μ§λ₯Ό μν€λ©΄μ μ μ§ λ©μΌμ λ°μ‘ν©λλ€.

λ€μμ μ μ²΄ μ μ  λͺ©λ‘μ΄ ["muzi", "frodo", "apeach", "neo"]μ΄κ³ , k = 2(μ¦, 2λ² μ΄μ μ κ³ λΉνλ©΄ μ΄μ© μ μ§)μΈ κ²½μ°μ μμμλλ€.

|  μ μ  ID	  | μ μ κ° μ κ³ ν ID |             	μ€λͺ             |
|:--------:|:----------:|:---------------------------:|
|  "muzi"  |  	"frodo"  |  	"muzi"κ° "frodo"λ₯Ό μ κ³ νμ΅λλ€.  |
| "apeach" |  	"frodo"  | 	"apeach"κ° "frodo"λ₯Ό μ κ³ νμ΅λλ€. |
| "frodo"	 |   "neo"	   |   "frodo"κ° "neo"λ₯Ό μ κ³ νμ΅λλ€.   |
|  "muzi"  |   "neo"    |   	"muzi"κ° "neo"λ₯Ό μ κ³ νμ΅λλ€.   |
| "apeach" |  	"muzi"   | 	 "apeach"κ° "muzi"λ₯Ό μ κ³ νμ΅λλ€. |

κ° μ μ λ³λ‘ μ κ³ λΉν νμλ λ€μκ³Ό κ°μ΅λλ€.

|  μ μ  ID   | μ κ³ λΉν νμ |
|:--------:|:-------:|
|  "muzi"  |    1    |
| "frodo"  |    2    |
| "apeach" |    0    |
|  "neo"   |    2    |

μ μμμμλ 2λ² μ΄μ μ κ³ λΉν "frodo"μ "neo"μ κ²μν μ΄μ©μ΄ μ μ§λ©λλ€. 

μ΄λ, κ° μ μ λ³λ‘ μ κ³ ν μμ΄λμ μ μ§λ μμ΄λλ₯Ό μ λ¦¬νλ©΄ λ€μκ³Ό κ°μ΅λλ€.

|  μ μ  ID	  |     μ μ κ° μ κ³ ν ID     |      	μ μ§λ ID      |
|:--------:|:------------------:|:-----------------:|
|  "muzi"  | 	["frodo", "neo"]  | 	["frodo", "neo"] |
| "frodo"  |      	["neo"]      |     	["neo"]      |
| "apeach" | 	["muzi", "frodo"] |    	["frodo"]     |
|  "neo"   |       	μμ 	        |        μμ         |

λ°λΌμ "muzi"λ μ²λ¦¬ κ²°κ³Ό λ©μΌμ 2ν, "frodo"μ "apeach"λ κ°κ° μ²λ¦¬ κ²°κ³Ό λ©μΌμ 1ν λ°κ² λ©λλ€.

μ΄μ©μμ IDκ° λ΄κΈ΄ λ¬Έμμ΄ λ°°μ΄ id_list, κ° μ΄μ©μκ° μ κ³ ν μ΄μ©μμ ID μ λ³΄κ° λ΄κΈ΄ λ¬Έμμ΄ λ°°μ΄ report, μ μ§ κΈ°μ€μ΄ λλ μ κ³  νμ kκ° λ§€κ°λ³μλ‘ μ£Όμ΄μ§ λ, κ° μ μ λ³λ‘ μ²λ¦¬ κ²°κ³Ό λ©μΌμ λ°μ νμλ₯Ό λ°°μ΄μ λ΄μ return νλλ‘ solution ν¨μλ₯Ό μμ±ν΄μ£ΌμΈμ.

### 1-1.μ νμ¬ν­
- 2 β€ id_listμ κΈΈμ΄ β€ 1,000
  - 1 β€ id_listμ μμ κΈΈμ΄ β€ 10
  - id_listμ μμλ μ΄μ©μμ idλ₯Ό λνλ΄λ λ¬Έμμ΄μ΄λ©° μνλ²³ μλ¬Έμλ‘λ§ μ΄λ£¨μ΄μ Έ μμ΅λλ€.
  - id_listμλ κ°μ μμ΄λκ° μ€λ³΅ν΄μ λ€μ΄μμ§ μμ΅λλ€.
- 1 β€ reportμ κΈΈμ΄ β€ 200,000
  - 3 β€ reportμ μμ κΈΈμ΄ β€ 21
  - reportμ μμλ "μ΄μ©μid μ κ³ νid"ννμ λ¬Έμμ΄μλλ€.
  - μλ₯Ό λ€μ΄ "muzi frodo"μ κ²½μ° "muzi"κ° "frodo"λ₯Ό μ κ³ νλ€λ μλ―Έμλλ€.
  - idλ μνλ²³ μλ¬Έμλ‘λ§ μ΄λ£¨μ΄μ Έ μμ΅λλ€.
  - μ΄μ©μidμ μ κ³ νidλ κ³΅λ°±(μ€νμ΄μ€)νλλ‘ κ΅¬λΆλμ΄ μμ΅λλ€.
  - μκΈ° μμ μ μ κ³ νλ κ²½μ°λ μμ΅λλ€.
- 1 β€ k β€ 200, kλ μμ°μμλλ€.
  - return νλ λ°°μ΄μ id_listμ λ΄κΈ΄ id μμλλ‘ κ° μ μ κ° λ°μ κ²°κ³Ό λ©μΌ μλ₯Ό λ΄μΌλ©΄ λ©λλ€.

### 1-2.μμΆλ ₯ μ

|              id_list               |                               	report                               | 	k  |   	result   |
|:----------------------------------:|:-------------------------------------------------------------------:|:---:|:-----------:|
| ["muzi", "frodo", "apeach", "neo"] | 	["muzi frodo","apeach frodo","frodo neo","muzi neo","apeach muzi"] | 	2  | 	[2,1,1,0]  |
|         ["con", "ryan"] 	          |          ["ryan con", "ryan con", "ryan con", "ryan con"]           | 	3  |   	[0,0]    |


### 1-3.μμΆλ ₯ μ μ€λͺ
μμΆλ ₯ μ #1

λ¬Έμ μ μμμ κ°μ΅λλ€.

μμΆλ ₯ μ #2

"ryan"μ΄ "con"μ 4λ² μ κ³ νμΌλ, μ£Όμ΄μ§ μ‘°κ±΄μ λ°λΌ ν μ μ κ° κ°μ μ μ λ₯Ό μ¬λ¬ λ² μ κ³ ν κ²½μ°λ μ κ³  νμ 1νλ‘ μ²λ¦¬ν©λλ€. λ°λΌμ "con"μ 1ν μ κ³ λΉνμ΅λλ€. 3λ² μ΄μ μ κ³ λΉν μ΄μ©μλ μμΌλ©°, "con"κ³Ό "ryan"μ κ²°κ³Ό λ©μΌμ λ°μ§ μμ΅λλ€. λ°λΌμ [0, 0]μ return ν©λλ€.

## λ΄ νμ΄
```python
def solution(id_list, report, k):
    answer = list(map(lambda x : 0, id_list))
    # print(answer)
    report_list = {}
    
    for index, value in enumerate(id_list):
        report_list[value] = []
        
    for index, value in enumerate(report):
        users = value.split(" ")
        if not users[0] in report_list[users[1]]:
            report_list[users[1]].append(users[0])
    
    for key in report_list:
        if len(report_list[key]) >= k:
            for value in report_list[key]:
                user_index = id_list.index(value)
                answer[user_index] += 1
    
    return answer

```

```toc

```
