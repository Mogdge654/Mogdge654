<!DOCTYPE html>
<html>
<head>
  <title>Click Counter</title>
  <style>
    body {
      background-color: #f2f2f2;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    button {
      background-color: blue;
      border: none;
      color: white;
      padding: 15px 32px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
      font-size: 16px;
      margin: 4px 2px;
      cursor: pointer;
    }
    #counter {
      font-size: 48px;
      color: #4CAF50;
      text-align: center;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <button id="click-me">Click Me</button>
  <div id="counter">0</div>
  <script>
    var count = 0;
    var button = document.getElementById("click-me");
    var counter = document.getElementById("counter");
    button.addEventListener("click", function() {
      count++;
      counter.innerHTML = count;
    });
  </script>
</body>
</html>
