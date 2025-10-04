# portofolio_wids
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portofolio Widdd</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: #b3e5fc;
      color: #003366;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      overflow: hidden;
      transition: background-color 1s;
    }
    h1 {
      font-size: 4em;
      margin: 0;
      animation: fadeIn 2s ease;
    }
    p {
      font-size: 1.5em;
      margin: 10px 0 30px;
      animation: fadeIn 2s ease 0.5s;
    }
    button {
      background-color: #0288d1;
      border: none;
      color: white;
      padding: 15px 40px;
      border-radius: 25px;
      font-size: 1.2em;
      cursor: pointer;
      transition: transform 0.3s, background-color 0.3s;
      animation: fadeIn 2s ease 1s;
    }
    button:hover {
      transform: scale(1.05);
      background-color: #01579b;
    }
    .slide {
      opacity: 0;
      position: absolute;
      transition: opacity 1s;
    }
    .active {
      opacity: 1;
      position: relative;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    a {
      color: #01579b;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div id="slide1" class="slide active">
    <h1>PORTOFOLIO</h1>
    <p>wids</p>
    <button onclick="nextSlide()">Masuk</button>
  </div>

  <div id="slide2" class="slide">
    <h1>Akun & Link</h1>
    <p>
      <a href="https://drive.google.com/drive/folders/1Ebx5MAKmqIXkakxHdGOW3N1IkJsnjHU5" target="_blank">Google Drive</a><br>
      <a href="https://www.tiktok.com/@mang_yy?_t=ZS-90GOrGefzqE&_r=1" target="_blank">TikTok</a>
    </p>
  </div>

  <script>
    function nextSlide() {
      document.getElementById('slide1').classList.remove('active');
      document.getElementById('slide2').classList.add('active');
      document.body.style.backgroundColor = '#a7ffeb';
    }
  </script>
</body>
</html>
