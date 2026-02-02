<!DOCTYPE html>
<html>
<head>
  <title>Student Login</title>
  <style>
    body {
      font-family: Arial;
      background: #f2f2f2;
    }
    .box {
      width: 300px;
      margin: 100px auto;
      background: white;
      padding: 20px;
      text-align: center;
      border-radius: 5px;
    }
    input {
      width: 90%;
      padding: 8px;
      margin: 5px;
    }
    button {
      padding: 8px 15px;
    }
  </style>
</head>

<body>
  <div class="box">
    <h2>Student Login</h2>

    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">

    <button onclick="login()">Login</button>

    <p id="result"></p>
  </div>

  <script>
    function login() {
      var u = document.getElementById("username").value;
      var p = document.getElementById("password").value;

      if (u === "pranav" && p === "1234") {
        document.getElementById("result").innerHTML =
          "✅ Login Successful <br>Name: Pranav Joshi <br>Branch: Computer Engineering";
      } else {
        document.getElementById("result").innerHTML =
          "❌ Invalid Username or Password";
      }
    }
  </script>
</body>
</html># student-login-website
