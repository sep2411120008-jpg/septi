<!DOCTYPE html>
<html>
<head>
    <title>TOEFL Practice App</title>
    <style>
        body {
            font-family: Arial;
            text-align: center;
            background-color: #f0f8ff;
        }
        .container {
            background: white;
            padding: 20px;
            width: 50%;
            margin: auto;
            border-radius: 10px;
            box-shadow: 0 0 10px gray;
        }
        button {
            padding: 10px;
            margin: 5px;
            width: 100px;
        }
    </style>
</head>

<body>
    <div class="container">
        <h2>Mini TOEFL Practice</h2>

        <p id="question">She ____ to school every day.</p>

        <button onclick="checkAnswer('go')">go</button>
        <button onclick="checkAnswer('goes')">goes</button>
        <button onclick="checkAnswer('gone')">gone</button>

        <h3 id="result"></h3>
        <h3>Score: <span id="score">0</span></h3>
    </div>

<script>
let score = 0;

function checkAnswer(answer){
    if(answer === "goes"){
        document.getElementById("result").innerHTML = "Correct!";
        score += 10;
    } else {
        document.getElementById("result").innerHTML = "Wrong!";
    }
    document.getElementById("score").innerHTML = score;
}
</script>

</body>
</html>
