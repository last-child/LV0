## 01. Text 태그

<br>   

```html
<h2>오감도</h2>
<p><b>첫번째</b> 아이가 <strong>기쁘다</strong>고 합니다.</p>
<p><i>두번째</i> 아이가 <em>화난다</em>고 합니다.</p>
<p><u>세번째</u> 아이가 <ins>슬프다</ins>고 합니다.</p>
<p><s>네번째</s> 아이가 <del>즐겁다</del>고 합니다.</p>
```

<br>   
<img src="https://github.com/last-child/FE/assets/98595054/8514ac7c-003c-4934-a989-6cc60b5260fa" height="200px">

<BR>   
<BR>   
<BR>   
<BR>   
<BR>   

## 02. Link 태그

<br>   

```html
<ul>
  <li><a href="http://www.naver.com" target="_self">네이버</a></li>
  <li><a href="http://www.google.co.kr" target="_blank">구글</a></li>
  <li><a href="index.html">홈으로</a></li>
</ul>
```

<br>   

#### \<a\> 태그의 target 속성은 링크된 문서가 어디에 열릴지를 지정한다.
#### 속성 값이 '_self'이면 현재 페이지가 새로운 내용으로 대체된다.
#### 속성 값이 '_blank'이면 링크된 문서가 새로운 창에서 열리게 된다.

<BR>   
<BR>   
<BR>   
<BR>   
<BR>   

## 03. Media 태그

<br>   

```html
<img src="lemon.png" alt="레몬" title="노란 과일" width="300px" height="300px">
```

<br>   

```html
<audio autoplay controls loop>
  <source src="audio.mp3" type="audio/mp3">
  <source src="audio.ogg" type="audio/ogg">
</audio>
```

<br>   

```html
<video autoplay loop muted width="300" height="300">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
</video>
```

<br>    

#### \<img\> 태그의 alt 속성은 이미지가 표시되지 않을 때 대체하는 텍스트 설명을 지정한다.
#### title 속성은 이미지 위에 마우스 포인터를 올려놓을 때 나타나는 텍스트 설명을 지정한다.

<br>   

#### 브라우저마다 지원하는 멀티미디어 파일의 포맷이 달라, 콘텐츠가 특정 브라우저에서 호환되지 못할 수 있다.
#### 멀티미디어 콘텐츠를 가능한 많은 브라우저에 제공하기 위해 여러 포맷의 파일을 준비하고,
#### 위와 같은 방식으로 \<source\> 태그를 \<audio\> 태그나 \<video\> 태그 내에 명시한다.

<br>   

#### controls 속성은 사용자에게 오디오나 비디오를 제어할 수 있는 인터페이스를 제공한다.
#### 해당 속성이 없으면 사용자는 재생, 일시 정지, 볼륨 조절 등의 제어 기능을 이용할 수 없다.

<br>   
<br>   
<br>   
<br>   
<br>   

## 04. Table 태그

<br>   

```html
<table>
  <thead>
    <tr>
      <th>국가</th> <th>수도</th> <th>인구 (만명)</th> <th>면적 (만km²)</th> <th>공용어</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>대한민국</td> <td>서울</td> <td>5,178</td> <td>10.0</td> <td>한국어</td>
    </tr>
    <tr>
      <td>일본</td> <td>도쿄</td> <td>12,596</td> <td>37.8</td> <td>일본어</td>
    </tr>
    <tr>
      <td>미국</td> <td>워싱턴 D.C.</td> <td>33,189</td> <td>952.5</td> <td rowspan="3">영어</td>
    </tr>
    <tr>
      <td>영국</td> <td>런던</td> <td>6,664</td> <td>24.4</td>
    </tr>
    <tr>
      <td>호주</td> <td>캔버라</td> <td>2,549</td> <td>769.2</td>
    </tr>
  </tbody>
</table>
```

<br>   

![image](https://github.com/last-child/FE/assets/98595054/858b9ba2-c9f9-4a18-a81e-579e2b9d74c0)
