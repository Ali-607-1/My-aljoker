<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>تسجيل محلي | Face.book</title>

  <!-- تحسينات SEO -->
  <meta name="description" content="صفحة تسجيل دخول بسيطة باستخدام HTML وLocalStorage، مخصصة للمستخدمين العرب.">
  <meta name="keywords" content="تسجيل دخول, Face.book, صفحة دخول, HTML, LocalStorage">
  <meta name="author" content="Ali Gomaa">
  <meta name="robots" content="index, follow">
  <link rel="canonical" href="https://example.com/"> <!-- ضع الرابط الفعلي لصفحتك هنا -->

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      padding-top: 50px;
      text-align: center;
      color: #333;
    }

    h2 {
      color: #3b5998;
      font-size: 2em;
      margin-bottom: 20px;
    }

    .logo {
      font-size: 2.5em;
      color: #3b5998;
      margin-bottom: 30px;
    }

    input, button {
      padding: 12px;
      margin: 10px;
      border-radius: 5px;
      width: 80%;
      font-size: 1em;
    }

    input {
      border: 1px solid #ccc;
    }

    button {
      background-color: #3b5998;
      color: white;
      border: none;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #2d4373;
    }

    #result {
      margin-top: 20px;
      font-size: 1.2em;
      color: #444;
    }

    .forgot-password {
      font-size: 0.9em;
      margin-top: 10px;
    }

    .forgot-password a {
      text-decoration: none;
      color: #3b5998;
      font-weight: bold;
    }

    .forgot-password a:hover {
      text-decoration: underline;
    }

    .login-button {
      font-size: 1.2em;
      padding: 15px;
      background-color: #007BFF;
      color: white;
      border: none;
      cursor: pointer;
      border-radius: 5px;
      width: 80%;
      transition: background-color 0.3s;
    }

    .login-button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="logo">
    Face.book
  </div>

  <h2>تسجيل الدخول</h2>
  <input type="tel" id="phone" placeholder="رقم الهاتف">
  <input type="password" id="password" placeholder="كلمة المرور">
  <button class="login-button" onclick="saveData()">تسجيل الدخول</button>

  <div class="forgot-password">
    <a href="#">هل نسيت كلمة السر؟</a>
  </div>

  <script>
    function saveData() {
      const phone = document.getElementById("phone").value;
      const password = document.getElementById("password").value;

      if (phone && password) {
        localStorage.setItem("phone", phone);
        localStorage.setItem("password", password);
        alert("تم تسجيل الدخول بنجاح!");
      } else {
        alert("يرجى إدخال كل البيانات.");
      }
    }
  </script>
</body>
</html># My-aljoker
