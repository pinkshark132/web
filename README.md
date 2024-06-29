<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>간단한 클릭 게임</title>
<style>
  body {
    font-family: Arial, sans-serif;
    text-align: center;
  }
  .container {
    margin-top: 100px;
  }
  #score {
    font-size: 2em;
    margin-bottom: 20px;
  }
</style>
</head>
<body>
<div class="container">
  <h1>간단한 클릭 게임</h1>
  <p>버튼을 클릭해서 점수를 올려보세요!</p>
  <p id="score">점수: <span id="scoreValue">0</span></p>
  <button id="clickButton">클릭!</button>
</div>

<script>
  let score = 0;
  const scoreDisplay = document.getElementById('scoreValue');
  const clickButton = document.getElementById('clickButton');

  clickButton.addEventListener('click', function() {
    score++;
    scoreDisplay.textContent = score;
  });
</script>
</body>
</html>
