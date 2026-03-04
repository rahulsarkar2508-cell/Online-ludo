<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online Ludo Game</title>

<style>
body{
  text-align:center;
  font-family:Arial;
  background:#f2f2f2;
}

h1{
  margin-top:20px;
}

.board{
  width:320px;
  height:320px;
  margin:20px auto;
  display:grid;
  grid-template-columns:repeat(3,1fr);
  grid-template-rows:repeat(3,1fr);
  border:5px solid black;
}

.box{
  border:2px solid black;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:22px;
  font-weight:bold;
}

.red{background:red; color:white;}
.green{background:green; color:white;}
.yellow{background:yellow;}
.blue{background:blue; color:white;}

button{
  padding:10px 25px;
  font-size:18px;
  margin-top:15px;
  cursor:pointer;
}

#dice{
  font-size:25px;
  margin-top:15px;
}
</style>
</head>

<body>

<h1>🎲 My Online Ludo 🎲</h1>

<div class="board">
  <div class="box red">R</div>
  <div class="box"></div>
  <div class="box green">G</div>
  <div class="box"></div>
  <div class="box">🎯</div>
  <div class="box"></div>
  <div class="box yellow">Y</div>
  <div class="box"></div>
  <div class="box blue">B</div>
</div>

<button onclick="rollDice()">Roll Dice</button>

<div id="dice">Dice: ?</div>

<script>
function rollDice(){
  var number = Math.floor(Math.random()*6)+1;
  document.getElementById("dice").innerHTML = "Dice: " + number;
}
</script>

</body>
</html>
