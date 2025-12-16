<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>パスワード認証</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #f3f3f3;
      font-family: system-ui, sans-serif;
    }
    .box {
      background: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 8px 20px rgba(0,0,0,.15);
      width: 320px;
      text-align: center;
    }
    input {
      width: 100%;
      padding: 10px;
      font-size: 16px;
      margin: 15px 0;
    }
    button {
      width: 100%;
      padding: 10px;
      font-size: 16px;
      cursor: pointer;
    }
    .msg {
      color: red;
      margin-top: 10px;
      min-height: 1em;
    }
  </style>
</head>
<body>

  <div class="box">
    <h2>パスワードを入力してください</h2>
    <input type="password" id="pw" placeholder="パスワード">
    <button onclick="check()">送信</button>
    <div id="msg" class="msg"></div>
  </div>

  <script>
    function check() {
      const pw = document.getElementById("pw").value;

      if (pw === "1122") {
        // ★ 今回はこのURLでOK ★
        location.href = "https://sites.google.com/g.miyazaki-c.ed.jp/411/%E5%A5%BD%E3%81%8D%E3%81%AA%E6%9B%B2";
      } else {
        document.getElementById("msg").textContent =
          "パスワードが違います";
      }
    }
  </script>

</body>
</html>
