<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine, Babby Ji? ❤️</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: pink;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            font-size: 2rem;
            color: red;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 1.5rem;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
        #yesBtn {
            background-color: green;
            color: white;
            transition: all 0.3s ease-in-out;
        }
        #noBtn {
            background-color: red;
            color: white;
        }
        .gif {
            margin-top: 20px;
            width: 200px;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <h1>Will You Be My Valentine, Babby Ji? ❤️</h1>
    <img src="https://media.giphy.com/media/3oz8xZvvOZRmKay4xy/giphy.gif" class="gif" alt="Cute Love GIF">
    
  <div class="buttons">
        <button id="yesBtn">Yes</button>
        <button id="noBtn">No</button>
    </div>
    <img src="https://media.giphy.com/media/JUwliZWcyDmTQZ7m9L/giphy.gif" class="gif hidden" id="finalGif" alt="Happy Love GIF">

   <script>
        let yesBtn = document.getElementById("yesBtn");
        let noBtn = document.getElementById("noBtn");
        let finalGif = document.getElementById("finalGif");
        let yesSize = 1.5;

        noBtn.addEventListener("click", () => {
            yesSize += 0.5; 
            yesBtn.style.fontSize = yesSize + "rem";
        });

        yesBtn.addEventListener("click", () => {
            alert("Yay! I knew it! ❤️");
            finalGif.classList.remove("hidden");
        });
    </script>
</body>
</html>

