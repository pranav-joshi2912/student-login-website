<!DOCTYPE html>
<html>
<head>
  <title>Login Page</title>
</head>
<body>

<h2>Login</h2>

<form onsubmit="return checkLogin()">
  <label>Username:</label><br>
  <input type="text" id="username" required><br><br>

  <label>Password:</label><br>
  <input type="password" id="password" required><br><br>

  <button type="submit">Login</button>
</form>

<script>
function checkLogin() {
  var user = document.getElementById("username").value;
  var pass = document.getElementById("password").value;

  // demo username & password
  if (user === "pranav" && pass === "1234") {
    window.location.href = "home.html"; // पुढचं पेज
    return false;
  } else {
    alert("Username किंवा Password चुकलाय");
    return false;
  }
}
</script>

</body>
</html><!DOCTYPE html>
<html>
<head>
  <title>Home</title>
</head>
<body>

<h1>Login Successful 🎉</h1>
<p>Welcome to Home Page</p>

</body>
</html>
