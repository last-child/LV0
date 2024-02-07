## 01. Form 태그 (1)

<br>   

```html
<form action="server_url" method="post" enctype="multipart/form-data">
  <fieldset>
    <legend>필수 정보</legend>
    ...
  </fieldset>

  <fieldset>
    <legend>부가 정보</legend>
    ...
  </fieldset>

  <input type="reset" value="가입 취소">
  <input type="submit" value="가입 완료">
</form>
```

<br>   

#### \<form\> 태그의 method 속성이 'get'으로 지정될 경우, 폼 데이터가 URL을 통해 서버에 전송된다.
#### GET 요청으로 받은 리소스는 캐시에 저장되며, 해당 리소스의 URL은 북마크(즐겨찾기)로 저장될 수 있다.
#### 브라우저는 동일한 GET 요청이 다시 발생할 때 서버에 요청하지 않고 캐시에서 리소스를 가져온다.
#### GET 요청은 웹 페이지 로딩 시간을 줄일 수 있지만, 요청 데이터가 URL에 노출되어 보안에 취약하다. 
#### 또한 URL 길이에 제한이 있으므로 GET 요청은 대용량 데이터를 전송하기에 적합하지 않다.

<br>   

#### method 속성이 'post'로 지정될 경우, 폼 데이터가 HTTP 요청 본문(body)에 포함되어 서버에 전송된다.
#### POST 요청은 URL에 요청 데이터가 노출되지 않으므로, GET 요청에 비해 안전하다.
#### 동일한 POST 요청이 여러 번 실행될 때마다 브라우저는 서버에 새로운 요청을 보낸다.
#### 서버는 동일한 POST 요청을 여러 번 수신하더라도 각각의 요청을 별개의 요청으로 처리한다.

<br>   
<br>   
<br>   
<br>   
<br>   

## 02. Form 태그 (2)

<br>   

```html
<fieldset>
  <legend>필수 정보</legend>
  <table>
    <tr>
      <td class="left">아이디</td>
      <td class="right"><input type="text" id="userId" name="userId" required></td>
    </tr>
    <tr>
      <td class="left">비밀번호</td>
      <td class="right"><input type="password" id="userPw" name="userPw" required></td>
    </tr>
    <tr>
      <td class="left">비밀번호 확인</td>
      <td class="right"><input type="password" id="confirmPw" required></td>
    </tr>
    <tr>
      <td class="left">이름</td>
      <td class="right"><input type="text" id="userName" name="userName" value="홍길동" required></td>
    </tr>
  </table>
</fieldset>
```

<br>   

#### 사용자의 입력이나 선택에 따라 입력 필드의 value 값이 변경된다.
#### 사용자가 폼을 제출하면, 하위 입력 필드의 name과 value 쌍이 서버로 전송된다.
#### 서버는 name 값을 키로 사용하여, 대응하는 value를 추출하여 처리한다.

<br>   
<br>   
<br>   
<br>   
<br>   

## 03. Form 태그 (3)

<br>   

```html
<fieldset>
  <legend>부가 정보</legend>
  <table>
    <tr>
      <td class="left">이메일</td>
      <td class="right">
        <input type="text" id="userEmail" name="userEmail"> @
        <select id="emailOption" name="emailOption">
          <option value="gmail.com">gmail.com</option>
          <option value="naver.com">naver.com</option>
          <option value="daum.net">daum.net</option>
        </select>
      </td>
    </tr>
    <tr>
      <td class="left">성별</td>
      <td class="right">
        <label><input type="radio" name="gender" value="male" checked> 남자</label>
        <label><input type="radio" name="gender" value="female" checked> 여자</label>
      </td>
    </tr>
    <tr>
      <td class="left">지망</td>
      <td class="right">
        <label><input type="checkbox" name="field" value="fe"> 프론트엔드</label>
        <label><input type="checkbox" name="field" value="be"> 백엔드</label>
        <label><input type="checkbox" name="field" value="dba"> DBA</label>
      </td>
    </tr>
    <tr>
      <td class="left">사진</td>
      <td class="right"><input type="file" id="photo" name="photo"></td>
    </tr>
    <tr>
      <td class="left">자기소개</td>
      <td class="right"><textarea id="intro" name="intro" cols="50" rows="5"></textarea></td>
    </tr>
  </table>
</fieldset>
```

<br>   

<img src="https://github.com/last-child/FE/assets/98595054/b8eb732e-f5b4-4d05-8f2c-8e93b310285a" width="600px">
