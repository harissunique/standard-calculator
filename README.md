# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
Use the code of html design the standard calculator 

### Step 2:
Change the settings.py to allow the from all hosts 


### Step 3:
Use the attractive colours 


### Step 4:
write the different code for operators

### Step 5:
Validate the html code 

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Calculator</title>
        
        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>

        <style>
          
            .calculator-container {
                width: 400px;
                background-color:rgb(141, 176, 23);
                margin: 0 auto; 
                margin-top: 90px;
                text-align: center;
                
            }

           
            button {
                width: 50px;
                height: 50px;
                margin: 10px; 
                font-size: 20px; 
                
                background-color: black; 
                color: white; 
                border: none;
            }

          
            #result {
                
       background-color:#79efe1;
    text-align: right;
    padding-right: 50px;
    font-size: 20px;
    margin-bottom: 20px; 
    border: solid rgb(213, 98, 98) 0.5px;
    color: rgb(73, 56, 165);
    width: 348px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 10px;
                color:white;
                font-size: 50px;
            }
            .redd {
                background-color: rgb(221, 88, 88);
            }
            .bluee {
                
                background-color: rgb(94, 214, 244);
            }
            body {
                background-color: rgb(207, 58, 167);
            }
        </style>

    </head>
<body>
    <div class="calculator-container">
        <h1>CALCULATOR</h1>
        <div id="result">0</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">&radic;</button> </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </body>
</html
```

## OUTPUT:
![](./file1.png)
![](./file2.png)

## Result:
The Program for design a standard calculator using the html is exectued successfully.
