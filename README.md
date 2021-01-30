# Cor-de-Fundo-Switch-
Simple buton to change the BackGround color.



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="style.css">
    <title>Change background color on Click</title>
</head>
<body>
    <div id="container">
    </div>
    <button id="button">Click me to change the color!</button>

    <script src="main.js"></script>
</body>
</html>

====================================================



#container {
    margin: auto;
    height: 500px;
    width: 500px;
    margin-top: 50px;
    background-color: blue;
}

#button {
    display: block;
    margin: auto;
    margin-top: 30px;
    width: 250px;
    height: 50px;
}


====================================================



//Colors array
let colors = ['blue', 'yellow', 'black', 'red', 'brown', 'orange'];

//get button
let button = document.getElementById('button');

//add event listener
button.addEventListener('click', function(){
    //randomizer
    var randomColor = colors[Math.floor(Math.random() * colors.length)]
    //get container
    let container = document.getElementById('container');

    container.style.background = randomColor;
})



