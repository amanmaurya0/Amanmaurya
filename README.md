<!DOCTYPE html>
<html>
<head>
  <title>Teen Patti Game</title>
  <style>
    body {
      font-family: Arial;
      text-align: center;
      background: green;
      color: white;
    }
    .card {
      display: inline-block;
      padding: 20px;
      margin: 10px;
      background: white;
      color: black;
      font-size: 20px;
      border-radius: 10px;
    }
    button {
      padding: 10px 20px;
      font-size: 18px;
      margin-top: 20px;
    }
  </style>
</head>

<body>

<h1>Teen Patti Game 🎴</h1>

<div id="cards"></div>

<button onclick="dealCards()">Deal Cards</button>

<script>
function getCard() {
  let cards = ["A♠","K♠","Q♠","J♠","10♠","9♠","8♠","7♠","6♠","5♠","4♠","3♠","2♠"];
  return cards[Math.floor(Math.random() * cards.length)];
}

function dealCards() {
  let output = "";
  for (let i = 0; i < 3; i++) {
    output += "<div class='card'>" + getCard() + "</div>";
  }
  document.getElementById("cards").innerHTML = output;
}
</script>

</body>
</html>![8268](https://github.com/user-attachments/assets/919de17c-88bf-4e6b-838d-759de1ec9acf)
