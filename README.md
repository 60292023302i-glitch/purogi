<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>パスワードページ</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .box {
      background: #fff;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 300px;
      text-align: center;
    }
    input {
      width: 100%;
      padding: 8px;
      margin: 10px 0;
      font-size: 16px;
    }
    button {
      padding: 8px 16px;
      font-size: 16px;
      cursor: pointer;
    }
    .error {
      color: red;
      margin-top: 10px;
    }
  </style>
</head>
<body>

  <div class="box">
    <h2>パスワードを入力してください</h2>

    <input type="password" id="password" placeholder="パスワード">
    <button onclick="checkPassword()">送信</button>

    <div id="error" class="error"></div>
  </div>

  <script>
    function checkPassword() {
      const pass = document.getElementById("password").value;

      if (pass === "1122") {
       https://sites.google.com/d/16MZ6zpuLuNSCkhpKjl60iIiz7j5ZfiTd/p/1PuH5NHkmC2d29A_sNyrLUixanNgtPEDW/edit
        window.location.href = "https://sites.google.com/view/yuta-room/趣味";
      } else {
        document.getElementById("error").textContent =
          "パスワードが違います";
      }
    }
  </script>

</body>
</html>
