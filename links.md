---
layout: base
search_exclude: true
menu: nav/home.html

---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Notebook Links</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
    .btn {
      display: inline-block;
      padding: 15px 25px;
      margin: 10px;
      font-size: 1.2em;
      color: #fff;
      background-color: #ffcc33;
      border: none;
      border-radius: 5px;
      text-decoration: none;
      text-align: center;
      cursor: pointer;
    }
    .btn:hover {
      background-color: #ffd966;
    }
  </style>
</head>
<body>
  <a href="{{site.baseurl}}/image/" class="btn">Images</a>
  <a href="{{site.baseurl}}/color/" class="btn">Color Codes</a>
  <a href="{{site.baseurl}}/hex/" class="btn">Hexadecimal</a>
</body>
</html>
