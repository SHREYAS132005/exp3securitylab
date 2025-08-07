# exp3securitylab
<!DOCTYPE html>
<html>
<head>
  <title>Simple Login</title>
</head>
<body>
  <h2>Login Form</h2>
  <form onsubmit="return login()">
    Username: <input type="text" id="username"><br><br>
    Password: <input type="password" id="password"><br><br>
    <input type="submit" value="Login">
  </form>

  <p id="message"></p>

  <script>
    function login() {
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;

      // Simple hardcoded credentials (for demo only)
      if (username === "admin" && password === "1234") {
        document.getElementById("message").innerText = "Login successful!";
      } else {
        document.getElementById("message").innerText = "Invalid credentials.";
      }

      return false; // Prevent form submission
    }
  </script>
</body>
</html>
