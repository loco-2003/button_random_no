<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Random Number Generator</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
    #random-number {
        font-size: 24px;
        margin-top: 20px;
    }
    #generate-btn {
        padding: 10px 20px;
        font-size: 18px;
        background-color: #4CAF50;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
    }
</style>
</head>
<body>

<h1>Random Number Generator</h1>
<button id="generate-btn">Generate Random Number</button>
<div id="random-number"></div>

<script>
document.getElementById('generate-btn').addEventListener('click', function() {
    var randomNumber = Math.floor(Math.random() * 100) + 1;
    document.getElementById('random-number').textContent = 'Random Number: ' + randomNumber;
});
</script>

</body>
</html>
