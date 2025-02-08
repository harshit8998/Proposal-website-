# Proposal-website-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Marry Me?</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <audio autoplay loop>
        <source src="love-song.mp3" type="audio/mp3">
    </audio>

    <div class="container">
        <h1>My Love,</h1>
        <p class="message">
            From the moment I met you, I knew you were the one.  
            Every smile, every moment, every heartbeat—it's all for you.  
            You are my best friend, my love, and my everything.  
        </p>
        <p class="question">Will you marry me?</p>

        <button id="yesBtn">Yes, I Will!</button>
        <button id="noBtn">No</button>

        <div id="response"></div>
    </div>

    <script src="script.js"></script>
</body>
</html>body {
    font-family: 'Arial', sans-serif;
    background: linear-gradient(to right, #ff4b2b, #ff416c);
    color: white;
    text-align: center;
    margin: 0;
    padding: 0;
}

.container {
    margin-top: 100px;
}

h1 {
    font-size: 3em;
    font-weight: bold;
}

.message {
    font-size: 1.5em;
    margin: 20px auto;
    width: 60%;
}

.question {
    font-size: 2em;
    font-weight: bold;
    margin: 30px 0;
}

button {
    padding: 15px 30px;
    font-size: 1.5em;
    margin: 10px;
    border: none;
    cursor: pointer;
    transition: 0.3s;
    border-radius: 5px;
}

#yesBtn {
    background-color: gold;
    color: black;
}

#noBtn {
    background-color: white;
    color: black;
}

button:hover {
    transform: scale(1.1);
}

#response {
    font-size: 2em;
    font-weight: bold;
    margin-top: 20px;
}document.getElementById("yesBtn").addEventListener("click", function() {
    document.getElementById("response").innerHTML = "Yay! I can't wait to spend forever with you! ❤️";
});

document.getElementById("noBtn").addEventListener("mouseover", function() {
    this.style.position = "absolute";
    this.style.top = Math.random() * window.innerHeight + "px";
    this.style.left = Math.random() * window.innerWidth + "px";
});
