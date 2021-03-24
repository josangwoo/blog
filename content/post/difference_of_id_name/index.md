+++
author = "Sangwoo Jo"
title = "HTML - name, id, class 속성 차이"
date = "2021-03-23"
description = ""
categories = [
    "HTML"
]
tags = [
    "HTML",
    "CSS"
]
image = "html.png"
+++

### 1. name

* `<form>` 태그 요소의 value 속성의 값을 서버로 전송하기 위한 속성입니다.
* CSS에 활용 불가능합니다.

```html
<form action="sign_up.php" method="post">
    <input type="hidden" name="check" value="ok">
    ...
</form>
```

### 2. id

* 페이지에서 고유한 요소 식별을 목적으로 사용합니다.
* CSS에서 선택자로 활용됩니다.

```html
<form>
    <label for="user-name">사용자 이름<label>
    <input type="text" id="user-name">
    </form>
```
### 3. class

* 성격이 동일한 요소들을 그룹으로 묶는 목적으로 사용합니다.
* CSS에서 선택자로 활용됩니다.

```html
<h2 class="bluetext">제목</h2>
<p clas="bluetext">내용</p>
```

```css
/*CSS*/
.bluetext {
    color:blue;
}
```