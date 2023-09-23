<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Suleyman calculator</title>
    <style>
        body {display:flex; height:100vh; margin: 0;}
        #calculator{border-radius: 15px; display: table; padding: 40px; box-shadow: 0 0 10px #666; border: 10px; margin: auto;}
        button, input {width: 50px; height: 40px; box-shadow: 2px 2px 0 #666; border: 1px solid #666; border-radius: 5px; margin: 5px;}
        button:active{box-shadow: 0 0 5px #666; }
        #equal {width: 115px;background-color: rgb(255, 68, 0);}
        input{
            width: 93%;
            box-shadow: inset 2px 2px 0 #666;
            background-color: rgb(255, 255, 255);
            text-align: right;
            box-sizing: border-box;
            padding-right: 20px;
        }

    </style>
</head>

<body>
   <div id="calculator">
    <div>
        <input type="text" id="display">
    </div>
    <div>
        <button onclick="ClearC()" id="Clear">C</button>
        <button>^</button>
        <button onclick="bolmeC()" id="bolme">/</button>
    </div>
    <div>
        <button onclick="sevenC()" id="seven">7</button>
        <button onclick="eightC()" id="eight">8</button>
        <button onclick="nineC()" id="nine">9</button>
        <button onclick="vurmaC()" id="vurma">*</button>
    </div>
    <div>
        <button onclick="fourC()" id="four">4</button>
        <button onclick="fiveC()" id="five">5</button>
        <button onclick="sixC()" id="six">6</button>
        <button onclick="minusC()" id="minus">-</button> 
    </div>
    <div>
        <button onclick="oneC()" id="one">1</button>
        <button onclick="twoC()" id="two">2</button>
        <button onclick="threeC()" id="three">3</button>
        <button onclick="plusC()" id="plus">+</button>
    </div>
        <div>
        <button onclick="nokteC()" id="nokte">.</button>
        <button onclick="zeroC()" id="zero">0</button>
        <button onclick="calc()" id="equal">=</button>
    </div>
   </div>
    <script>
    const display = document.getElementById('display')
    const equal = document.getElementById('equal')
    const five = document.getElementById('five')
    const plus = document.getElementById('plus')
    const six = document.getElementById('six')
    const minus = document.getElementById('minus')
    const four = document.getElementById('four')
    const one = document.getElementById('one')
    const two = document.getElementById('two')
    const three = document.getElementById('three')
    const nokte = document.getElementById('nokte')
    const zero = document.getElementById('zero')
    const vurma = document.getElementById('vurma')
    const nine = document.getElementById('nine')
    const eight = document.getElementById('eight')
    const seven = document.getElementById('seven')
    const bolme = document.getElementById('bolme')
    const Clear = document.getElementById('Clear')
    function calc() {
     display.value = eval(display.value)
 
    }
    function fiveC() {
        display.value = display.value + five.innerHTML
    }
    function plusC() {
        display.value = display.value + plus.innerHTML
    }
    function sixC() {
        display.value += six.innerHTML
    }
    function minusC() {
        display.value += minus.innerHTML
    }
    function fourC() {
        display.value += four.innerHTML
    }
    function oneC() {
        display.value += one.innerHTML
    }
    function twoC() {
        display.value += two.innerHTML
    }
    function threeC() {
        display.value += three.innerHTML
    }
    function nokteC() {
        display.value += nokte.innerHTML
    }
    function zeroC() {
        display.value += zero.innerHTML
    }
    function vurmaC() {
        display.value += vurma.innerHTML
    }
    function nineC() {
        display.value += nine.innerHTML
    }
    function eightC() {
        display.value += eight.innerHTML
    }
    function sevenC() {
        display.value += seven.innerHTML
    }
    function bolmeC() {
        display.value += bolme.innerHTML
    }
    function ClearC() {
        display.value = ''
    }
    
    </script>
</body>

</html>
