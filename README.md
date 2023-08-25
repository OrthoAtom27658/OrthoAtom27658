<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Hallo ich bins eins mensch</title>
  <meta name="viewport" content="width=device-width, initial-scale=1"><link rel="stylesheet" href="./style.css">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter&family=Lato&family=Roboto+Condensed:ital,wght@0,700;1,400&display=swap');

* {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
    box-sizing: border-box;
    color: inherit;
}

body {
    height: 100vh;
    background: linear-gradient(to right, #620256, #511b72);
}


div {
    background: rgba(0, 0, 0, 0);
    width: 70vw;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    margin: 0 auto;
    padding: 30px 30px 10px;
    box-shadow: 0 0 150px -20px rgba(0, 0, 0, 0.5);
    z-index: 3;
}

P {
    font-family: "Roboto Condensed", monospace;
    color: #f5f5f5;
    margin: 0 0 20px;
    font-size: 17px;
    line-height: 1.2;
}

span {
    color: #f0c674;
}

i {
    color: #8abeb7;
}

div a {
    text-decoration: none;
}

b {
    color: #81a2be;
}

a.avatar {
    position: fixed;
    bottom: 15px;
    right: -100px;
    -webkit-animation: slide 0.5s 4.5s forwards;
            animation: slide 0.5s 4.5s forwards;
    display: block;
    z-index: 4
}

@-webkit-keyframes slide {
    from {
        right: -100px;
        transform: rotate(360deg);
        opacity: 0;
    }
    to {
        right: 15px;
        transform: rotate(0deg);
        opacity: 1;
    }
}

@keyframes slide {
    from {
        right: -100px;
        transform: rotate(360deg);
        opacity: 0;
    }
    to {
        right: 15px;
        transform: rotate(0deg);
        opacity: 1;
    }
}
  </style>
</head>
<body>
<div><p> <span>Hi!</span>: <i>I am Ortho</i></p>
</div>
<script>
var str = document.getElementsByTagName('div')[0].innerHTML.toString();
var i = 0;
document.getElementsByTagName('div')[0].innerHTML = "";

setTimeout(function() {
    var se = setInterval(function() {
        i++;
        document.getElementsByTagName('div')[0].innerHTML = str.slice(0, i) + "|";
        if (i == str.length) {
            clearInterval(se);
            document.getElementsByTagName('div')[0].innerHTML = str;
        }
    }, 10);
},0);
</script

</body>
</html>
