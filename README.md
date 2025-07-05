# Aditya-FF-tournament
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Register | Aditya FF Tournament</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    body {
      background-color: #0f0f0f;
      font-family: 'Segoe UI', sans-serif;
      color: white;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 400px;
      margin: auto;
      padding: 30px 20px;
    }

    h2 {
      color: #ff3d3d;
      font-size: 28px;
      margin-bottom: 30px;
    }

    input, select {
      width: 100%;
      padding: 14px;
      margin: 10px 0;
      border-radius: 12px;
      background: #1b1b1b;
      border: none;
      color: white;
      font-size: 15px;
    }

    .phone-wrapper {
      display: flex;
      gap: 10px;
      align-items: center;
    }

    .phone-wrapper select {
      width: 30%;
      background: #1b1b1b;
      color: white;
    }

    .phone-wrapper input {
      width: 70%;
    }

    .password-wrapper {
      position: relative;
    }

    .show-btn {
      position: absolute;
      right: 15px;
      top: 50%;
      transform: translateY(-50%);
      color: #ff3d3d;
      font-size: 14px;
      cursor: pointer;
    }

    .promo-wrapper {
      display: flex;
      gap: 10px;
    }

    .promo-wrapper input {
      flex: 1;
    }

    .promo-wrapper button {
      background-color: #ff8c00;
      border: none;
      padding: 14px 18px;
      border-radius: 10px;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }

    .terms {
      font-size: 12px;
      margin: 20px 0;
      color: #aaa;
      text-align: center;
    }

    .terms b {
      color: white;
    }

    .btn-signup {
      width: 100%;
      padding: 15px;
      background-color: #e8002f;
      border: none;
      border-radius: 30px;
      font-weight: bold;
      font-size: 16px;
      color: white;
      cursor: pointer;
      margin-top: 10px;
    }

    .login-link {
      text-align: center;
      margin-top: 15px;
      font-size: 14px;
    }

    .login-link a {
      color: #ff3d3d;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="container">
    <h2>Create new,<br>Account</h2>

    <input type="text" placeholder="First Name">
    <input type="text" placeholder="Last Name">
    <input type="text" placeholder="Username">

    <div class="phone-wrapper">
      <select>
        <option value="+91">&#x1F1EE;&#x1F1F3; +91</option>
      </select>
      <input type="tel" placeholder="Phone Number">
    </div>

    <input type="email" placeholder="Email">

    <div class="password-wrapper">
      <input type="password" placeholder="Password" id="password">
      <span class="show-btn" onclick="togglePassword()">Show</span>
    </div>

    <div class="promo-wrapper">
      <input type="text" placeholder="Promo Code (Optional)">
      <button>APPLY</button>
    </div>

    <p class="terms">
      By Registering, I agree to Aditya FF Tournament’s <b>Terms and Conditions</b> and <b>Privacy Policy</b>
    </p>

    <button class="btn-signup">SIGN UP</button>

    <p class="login-link">
      Already have an account? <a href="#">LOGIN</a>
    </p>
  </div>

  <script>
    function togglePassword() {
      const input = document.getElementById('password');
      if (input.type === 'password') {
        input.type = 'text';
      } else {
        input.type = 'password';
      }
    }
  </script>

</body>
</html>
