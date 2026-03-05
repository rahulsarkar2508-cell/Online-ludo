<script>
function rollDice() {
  var dice = Math.floor(Math.random() * 6) + 1;
  document.getElementById("diceResult").innerHTML = dice;
}
</script><!DOCTYPE html>
<html>
<head>
<title>Ludo Game</title>
<style>

body{
text-align:center;
font-family:Arial;
background:#f2f2f2;
}

#board{
width:300px;
height:300px;
margin:auto;
display:grid;
grid-template-columns:repeat(3,1fr);
grid-template-rows:repeat(3,1fr);
gap:5px;
}

.box{
background:white;
border:2px solid black;
display:flex;
align-items:center;
justify-content:center;
font-size:20px;
}

#dice{
margin-top:20px;
font-size:30px;
padding:10px 20px;
background:red;
color:white;
border:none;
border-radius:10px;
}

</style>
</head>

<body>

<h2>Ludo Dice Game</h2>

<div id="board">

<div class="box">1</div>
<div class="box">2</div>
<div class="box">3</div>

<div class="box">4</div>
<div class="box">🏠</div>
<div class="box">5</div>

<div class="box">6</div>
<div class="box">7</div>
<div class="box">8</div>

</div>

<button id="dice" onclick="rollDice()">🎲 Roll Dice</button>

<h3 id="result">Dice: 0</h3>

<script>

function rollDice(){

var dice=Math.floor(Math.random()*6)+1;

document.getElementById("result").innerHTML="Dice: "+dice;

}

</script>

</body>
</html>
<button onclick="rollDice()">Roll Dice</button>
<p id="diceResult">0</p>
