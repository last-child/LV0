## 01. Text

<br>   

```css
h2 {
  text-align: center;
  text-decoration: underline;
}

p {
  font-family: Georgia, "Malgun Gothic", serif;
  font-size: 20px;
  font-weight: bold;
  font-style: italic;
  line-height: 130%;
}
```

<br>   

```css
a:link {
  color: royalblue;
}

a:visited {
  color: #eb17af;
}

a:hover {
  color: rgb(19, 146, 36);
}

a:active {
  color: rgba(241, 227, 255, 55);
}
```

<br>   
<br>   
<br>   
<br>   
<br>   

## 02. Background

<br>   

```css
#stage {
  background-color: aliceblue;
  background-image: url("images/idol.png");
  background-repeat: no-repeat;
  background-position: center top;
  background-attachment: fixed;
  background-size: contain;
}
```

<br>   

#### background-position 속성을 통해 배경 이미지의 위치를 지정할 수 있다.
#### 속성 값이 `left bottom`이면 배경 이미지를 요소의 왼쪽 하단에 배치한다.
#### 속성 값이 `100px 50px`이면 요소의 왼쪽 상단 모서리로부터 오른쪽으로 100px, 아래로 50px 떨어진 지점에 배치된다.

<br>   

#### background-size 속성을 통해 배경 이미지의 크기를 지정할 수 있다.
#### 속성 값이 `cover`이면 요소의 긴 축에 맞춰 이미지를 조정한다. 이미지가 요소를 완전히 채울 수 있지만, 이미지의 일부가 잘릴 수 있다.
#### 속성 값이 `contain`이면 요소의 짧은 축에 맞춰 이미지를 조정한다. 이미지가 온전히 보여질 수 있지만, 요소에 빈 공간이 생길 수 있다.
#### 속성 값이 `50% 75%`이면 요소 너비의 50%, 요소 높이의 75% 크기로 이미지를 조정한다.

<br>   
<br>   
<br>   
<br>   
<br>   

## 03. Box Model

<br>   

```css
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

#round {
  width: 200px;
  height: 100px;
  border: 5px solid black;
  border-radius: 10px;
  padding: 25px 30px 15px 10px;
  margin: 10px 0;
}
```

<br>   
 
#### box-sizing 속성을 통해 요소의 길이(widht, height)가 계산되는 방식을 조정할 수 있다.
#### 속성 값이 기본 값인 `content-box`이면 요소의 길이는 내용(content)의 지정된 길이만큼 계산한다.
#### 요소의 전체 크기는 패딩(padding)과 테두리(border)를 추가하기 때문에 지정 값보다 커질 수 있다.

<br>   

#### 속성 값이 `border-box`이면 요소의 길이는 패딩(padding)과 테두리(border)도 포함한다.
#### 이때 내용(content)의 실제 길이는 지정된 길이에서 패딩이나 테두리를 제외한 값이 된다.
#### 요소에 패딩과 테두리를 추가해도 요소의 전체 크기를 지정 값만큼 설계할 수 있다.
