<!DOCTYPE html>
<html lang="he">
<head>
  <meta charset="UTF-8">
  <title>משחק Simon</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background: #f0f0f0;
      direction: rtl;
    }
    #gameContainer {
      margin: 50px auto;
      width: 300px;
    }
    .simonButton {
      width: 140px;
      height: 140px;
      display: inline-block;
      margin: 5px;
      border: 5px solid #555;
      border-radius: 15px;
      cursor: pointer;
      opacity: 0.8;
    }
    /* עיצוב הכפתורים בצבעים השונים */
    #green {
      background-color: green;
    }
    #red {
      background-color: red;
    }
    #yellow {
      background-color: yellow;
    }
    #blue {
      background-color: blue;
    }
    /* אפקט כאשר הכפתור "זורח" */
    .active {
      opacity: 1;
      filter: brightness(150%);
    }
    #message {
      margin: 20px;
      font-size: 1.2em;
    }
    #startButton {
      padding: 10px 20px;
      font-size: 1em;
      cursor: pointer;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <h1>משחק Simon</h1>
  <div id="gameContainer">
    <div id="message">לחצי על "התחל" כדי לשחק!</div>
    <button id="startButton">התחל</button>
    <div>
      <div id="green" class="simonButton"></div>
      <div id="red" class="simonButton"></div>
    </div>
    <div>
      <div id="yellow" class="simonButton"></div>
      <div id="blue" class="simonButton"></div>
    </div>
  </div>

  <script>
    // מערך הצבעים
    const colors = ["green", "red", "yellow", "blue"];
    let sequence = [];      // הרצף שהמחשב יוצר
    let userSequence = [];  // הרצף שהמשתמש מזין
    let level = 0;
    let acceptingInput = false;  // האם המערכת מקבלת לחיצות מהמשתמש

    const messageEl = document.getElementById("message");
    const startButton = document.getElementById("startButton");

 
    function flashButton(color) {
      const button = document.getElementById(color);
      button.classList.add("active");
      setTimeout(() => {
        button.classList.remove("active");
      }, 500);
    }

    
    function playSequence() {
      acceptingInput = false;
      userSequence = [];
      let i = 0;
      const interval = setInterval(() => {
        flashButton(sequence[i]);
        i++;
        if (i >= sequence.length) {
          clearInterval(interval);
          acceptingInput = true;
          messageEl.textContent = "תורך לשחק!";
        }
      }, 800);
    }

    
    function addColorToSequence() {
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      sequence.push(randomColor);
    }

   
    function startGame() {
      sequence = [];
      level = 0;
      messageEl.textContent = "צפי לרצף...";
      nextLevel();
    }

     
    function nextLevel() {
      level++;
      messageEl.textContent = "רמה " + level + ". צפי לרצף...";
      addColorToSequence();
      setTimeout(playSequence, 1000);
    }

    
    function handleUserInput(color) {
      if (!acceptingInput) return;
      userSequence.push(color);
      flashButton(color);

      
      const currentIndex = userSequence.length - 1;
      if (userSequence[currentIndex] !== sequence[currentIndex]) {
        messageEl.textContent = "טעות! נגמר המשחק. לחצי על 'התחל' כדי לנסות שוב.";
        acceptingInput = false;
        return;
      }

     
      if (userSequence.length === sequence.length) {
        messageEl.textContent = "מעולה! רמה הבאה...";
        acceptingInput = false;
        setTimeout(nextLevel, 1000);
      }
    }

   
    colors.forEach(color => {
      document.getElementById(color).addEventListener("click", () => {
        handleUserInput(color);
      });
    });

    
    startButton.addEventListener("click", startGame);
  </script>
</body>
</html>
