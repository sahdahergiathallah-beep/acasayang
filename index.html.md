<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8">  
  <title>Valentine 💘</title>  
  <style>  
    body {  
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
      height: 100vh;  
      display: flex;  
      justify-content: center;  
      align-items: center;  
      font-family: 'Comic Sans MS', cursive;  
      text-align: center;  
    }  
  
    h1 {  
      color: #b3003b;  
    }  
  
    .buttons {  
      margin-top: 20px;  
    }  
  
    button {  
      padding: 12px 25px;  
      font-size: 20px;  
      border: none;  
      border-radius: 30px;  
      cursor: pointer;  
      transition: all 0.3s ease;  
      margin: 10px;  
    }  
  
    #yesBtn {  
      background-color: #ff3366;  
      color: white;  
    }  
  
    #noBtn {  
      background-color: #ffffff;  
      color: #ff3366;  
      border: 2px solid #ff3366;  
    }  
  </style>  
</head>  
<body>  
  
  <div>  
    <h1 id="text">will u be my valentine aca?</h1>  
  
    <div class="buttons">  
      <button id="yesBtn" onclick="yesClick()">Yes 💖</button>  
      <button id="noBtn" onclick="noClick()">No 😢</button>  
    </div>  
  </div>  
  
  <script>  
    let yesSize = 20;  
  
    function noClick() {  
      yesSize += 10;  
      document.getElementById("yesBtn").style.fontSize = yesSize + "px";  
    }  
  
    function yesClick() {  
      document.getElementById("text").innerText = "are u sure aca?";  
      document.querySelector(".buttons").innerHTML = "";  
    }  
  </script>  
  
</body>  
</html>  
