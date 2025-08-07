# exp3securitylab
<!DOCTYPE html>
<html>
<head>
  <title>Simple Login</title>
</head>
<body>
  <h2>Login Form</h2>
  <form onsubmit="return login()">
    Username: <input type="text" id="username" placeholder="Enter username"><br><br>
    Password: <input type="password" id="password" placeholder="Enter password"><br><br>
    <input type="submit" value="Login">
  </form>

  <p id="message"></p>

  <script>
    function login() {
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;

      if (username === "shreyas" && password === "kulkarni") {
        document.getElementById("message").innerText = "Login successful!";
        document.getElementById("message").style.color = "green";
      } else {
        document.getElementById("message").innerText = "Invalid username or password.";
        document.getElementById("message").style.color = "red";
      }

      return false; // prevent form submission to keep on same page
    }
  </script>
</body>
</html>

