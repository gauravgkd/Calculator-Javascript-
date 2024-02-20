This is a Simple Calculator using HTML CSS and JS

calculator.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link rel="stylesheet" href="./Calculator.css">
  <script src="./Calculator.js"></script>
</head>
<body>
  <div>
    <h1><mark style="background-color: crimson;">Simple Calculator</mark></h1>
  </div>
  <div id="cal">
    <input type="text" id="display">
  <div class="but-container">
    <button class="button" onclick="curdisplay = ''; document.querySelector('#display').value = curdisplay;">c</button>
    <button class="button" onclick="curdisplay = curdisplay + 1; document.querySelector('#display').value = curdisplay;">1</button>
    <button class="button" onclick="curdisplay = curdisplay + 2; document.querySelector('#display').value = curdisplay;">2</button>
    <button class="button" onclick="curdisplay = curdisplay + 3; document.querySelector('#display').value = curdisplay;">3</button>
    <button class="button" onclick="curdisplay = curdisplay + 4; document.querySelector('#display').value = curdisplay;">4</button>
    <button class="button" onclick="curdisplay = curdisplay + 5; document.querySelector('#display').value = curdisplay;">5</button>
    <button class="button" onclick="curdisplay = curdisplay + 6; document.querySelector('#display').value = curdisplay;">6</button>
    <button class="button" onclick="curdisplay = curdisplay + 7; document.querySelector('#display').value = curdisplay;">7</button>
    <button class="button" onclick="curdisplay = curdisplay + 8; document.querySelector('#display').value = curdisplay;">8</button>
    <button class="button" onclick="curdisplay = curdisplay + 9; document.querySelector('#display').value = curdisplay;">9</button>
    <button class="button" onclick="curdisplay = curdisplay + 0; document.querySelector('#display').value = curdisplay;">0</button>
    <button class="button" onclick="curdisplay = curdisplay + '+'; document.querySelector('#display').value = curdisplay;">+</button>
    <button class="button" onclick="curdisplay = curdisplay + '-'; document.querySelector('#display').value = curdisplay;">-</button>
    <button class="button" onclick="curdisplay = curdisplay + '*'; document.querySelector('#display').value = curdisplay;">x</button>
    <button class="button" onclick="curdisplay = curdisplay + '/'; document.querySelector('#display').value = curdisplay;">/</button>
    <button class="button" onclick="curdisplay = eval(curdisplay); document.querySelector('#display').value = curdisplay;">=</button>
    <button class="button" onclick="curdisplay = curdisplay + '.'; document.querySelector('#display').value = curdisplay;">.</button>
  </div>
</div>
</body>
</html>

calculator.css
#cal {
  border: 5px solid black;
  border-radius: 10px;
  width: 250px;
  box-shadow:inset;
}
#display {
  margin: 10px;
  width: 85%;
  font-size: 25px;
  box-sizing: border-box;
  border-color: blue;
  border-radius: 10px;
}
.button {
  height: 40px;
  width: 40px;
  margin: 3px;
  font-family: 'Times New Roman', Times, serif;
  font-size: larger;
  font-weight: bold;
  background-color:darkturquoise;
  border-radius: 5px;
}
.but-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
body {
  margin-top: 100px;
  justify-content: center;
  display: flex;
  align-items: center;
  text-align: center;
  flex-direction: column;
  background-color: aquamarine;
}

calculator.js
let curdisplay = '';
document.querySelector('#display').value = curdisplay;
