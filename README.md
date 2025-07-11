<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>FEU Login Page</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <style>
    body {
      background-color: #004d26;
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/5/54/FEU_Manila_Morayta_Building_Outline.png'); /* Replace with building outline */
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      color: white;
      font-family: Arial, sans-serif;
    }

    .login-container {
      max-width: 400px;
      margin: auto;
      margin-top: 80px;
      background-color: rgba(0, 0, 0, 0.4);
      padding: 30px;
      border-radius: 10px;
    }

    .login-container img {
      display: block;
      margin: 0 auto 20px auto;
      height: 100px;
    }

    .form-check-label {
      color: white;
    }

    .form-text a {
      color: #ccc;
      text-decoration: underline;
    }

    .bottom-links {
      text-align: center;
      margin-top: 20px;
    }

    .bottom-links a {
      color: #ccc;
      margin: 0 10px;
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <div class="login-container text-center">
    <img src="FEU-Logo-flat-version.png" alt="FEU Logo">
    
    <form id="loginForm" novalidate>
      <div class="mb-3 text-start">
        <label for="username" class="form-label">Username</label>
        <input type="text" class="form-control" id="username" required>
        <div class="invalid-feedback">Please enter your username.</div>
      </div>

      <div class="mb-3 text-start">
        <label for="password" class="form-label">Password</label>
        <input type="password" class="form-control" id="password" required>
        <div class="invalid-feedback">Please enter your password.</div>
      </div>

      <div class="form-check text-start mb-3">
        <input type="checkbox" class="form-check-input" id="staySignedIn">
        <label class="form-check-label" for="staySignedIn">Stay signed in</label>
      </div>

      <div class="mb-3 text-start">
        <a href="#" class="form-text">Forgot Password?</a>
      </div>

      <button type="submit" class="btn btn-light w-100">Log In</button>
    </form>

    <hr class="text-white my-4">

    <button class="btn btn-outline-light w-100">Login with Microsoft</button>

    <div class="bottom-links mt-4">
      <a href="#">Help</a>
      <a href="#">Privacy Policy</a>
      <a href="#">Acceptable Use Policy</a>
      <a href="#">Facebook</a>
      <a href="#">Twitter</a>
    </div>
  </div>

  <script>
    // Bootstrap form validation
    const form = document.getElementById('loginForm');

    form.addEventListener('submit', function (event) {
      if (!form.checkValidity()) {
        event.preventDefault();
        event.stopPropagation();
      }

      form.classList.add('was-validated');
    });
  </script>

</body>
</html>
