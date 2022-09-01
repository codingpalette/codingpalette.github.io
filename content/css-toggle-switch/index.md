---
emoji: 👻
title: CSS 토글 버튼 toggle switch 만들기
date: '2022-08-30 00:00:00'
author: coding-palette
tags: css
categories: css
---

css를 이용해서 토글 스위치를 만들어 보겠습니다.

![img1.jpg](img1.jpg)

## 1.HTML

```html
<div class="toggle_btn_container"> 
    <div class="toggle_btn_box"> 
        <input class="toggle_input " id="toggle_btn" type="checkbox" />
        <label class="toggle_label" for="toggle_btn"></label> 
    </div> 
</div>
```

## 2.CSS
```css
.toggle_btn_container {  
    padding: 10px;  
    box-sizing: border-box;  
    background: #767676;
}

.toggle_input {
    display: none;
}

.toggle_input + .toggle_label {
    outline: 0;
    display: block;
    width: 4em;
    height: 2em;
    position: relative;
    cursor: pointer;
    user-select: none;
}

.toggle_input + .toggle_label:after,
.toggle_input + .toggle_label:before {
    position: relative;
    display: block;
    content: '';
    width: 50%;
    height: 100%;
}

.toggle_input + .toggle_label:after {
    left: 0;
}

.toggle_input + .toggle_label:before {
    display: none;
}

.toggle_input:checked + .toggle_label:after {
    left: 50%;
}

.toggle_input + .toggle_label {
    background: #b8b8b8;
    border-radius: 2em;
    padding: 2px;
    transition: all 0.4s ease;
    box-sizing: border-box;
}

.toggle_input + .toggle_label:after {
    border-radius: 50%;
    background: #fff;
    transition: all 0.2s ease;
}

.toggle_input:checked + .toggle_label {
    background: #36ec73;
}
```

## 3.JavaScript

```js
const toggle_btn = document.querySelector('#toggle_btn');
const toggle_label = document.querySelector('.toggle_label');

toggle_btn.addEventListener('change' , function(){
    console.log(toggle_btn.checked)
})
```

실제 코드 적용 확인하기

[사이트가기](https://jsfiddle.net/tqa36crg/)


```toc

```