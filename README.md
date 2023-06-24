<!DOCTYPE html>
<html lang="en">

<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
        * {
            margin: 0%;
            padding: 0%;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            width: 100%;
            height: 100vh;
            justify-content: center;
            align-items: center;
            display: flex;
            background: linear-gradient(rgb(0, 0, 0), rgb(96, 105, 118));
        }
        
        .calculater {
            border-radius: 16px;
            border: 1px solid;
            padding: 20px;
            background: transparent;
            box-shadow: 0px 3px 16px rgb(96, 105, 118, 0.5);
        }
        
        #inputBox {
            background: transparent;
            padding: 20px;
            font-size: 40px;
            width: 315px;
            margin: 10px;
            border: none;
            text-align: right;
            border-radius: 8px;
            box-shadow: 0px 0px 15px rgb(96, 105, 118, 0.5);
            cursor: pointer;
            color: #ffff;
        }
        
        .inputBox::placeholder {
            color: #ffff;
        }
        
        .btn {
            width: 60px;
            border: none;
            height: 60PX;
            margin: 10PX;
            border-radius: 10px;
            box-shadow: 0px 0px 15px rgb(96, 105, 118, 0.5);
            background: transparent;
            color: #ffff;
            font-size: 20px;
        }
        
        .eq {
            background-color: chocolate;
        }
        
        .operator {
            color: rgb(41, 212, 138);
            width: 60px;
            border: none;
            height: 60PX;
            margin: 10PX;
            border-radius: 10px;
            box-shadow: 0px 0px 15px rgb(96, 105, 118, 0.5);
            background: transparent;
            font-size: 20px;
        }
    </style>


    <title> Calculater </title>



</head>

<body>
    <form>
        <div class="calculator">
            <input type="text" placeholder="0" id="inputBox" name="display">

            <div>
                <input type="button" value="AC" onclick="display.value = ''" class="operator">
                <input type="button" value="DE" onclick=" display.value = display.value.toString().slice(0,-1)" class="operator">
                <input type="button" value="." onclick="display.value += '.'" class="operator">
                <input type="button" value="/" onclick="display.value += '/'" class="operator">
            </div>
            <div>
                <input type="button" value="9" onclick="display.value += '9'" class="btn">
                <input type="button" value="8" onclick="display.value += '8'" class="btn">
                <input type="button" value="7" onclick="display.value += '7'" class="btn">
                <input type="button" value="X" onclick="display.value += '*'" class="operator">
            </div>
            <div>
                <input type="button" value="6" onclick="display.value += '6'" class="btn">
                <input type="button" value="5" onclick="display.value += '5'" class="btn">
                <input type="button" value="4" onclick="display.value += '4'" class="btn">
                <input type="button" value="-" onclick="display.value += '-'" class="operator">

            </div>
            <div>
                <input type="button" value="3" onclick="display.value += '3'" class="btn">
                <input type="button" value="2" onclick="display.value += '2'" class="btn">
                <input type="button" value="1" onclick="display.value += '1'" class="btn">
                <input type="button" value="+" onclick="display.value += '+'" class="operator">

            </div>
            <div>
                <input type="button" value="0" onclick="display.value += '0'" class="btn">
                <input type="button" value="00" onclick="display.value += '00'" class="btn">
                <input type="button" value="." onclick="display.value += '.'" class="btn">
                <input type="button" value="=" class="eq operator fbg" onclick="display.value = eval(display.value)">

            </div>



        </div>


    </form>
</body>

</html>
