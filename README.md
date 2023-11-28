# CALCULATOR-TASK1

## Develop a calculator app that performs basic math operations.

## Code:

### calcu.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="tyle.css">
    <title>Calculator</title>
</head>

<body>
    <div id="container">
        <h1>Calculator</h1>

        <div id="calculator">
            <input type="text" name="screen" id="screen">
            <table>
                <tr>
                    <td><button>(</button></td>
                    <td><button>)</button></td>
                    <td><button>C</button></td>
                    <td><button>%</button></td>
                </tr>
                <tr>
                    <td><button>7</button></td>
                    <td><button>8</button></td>
                    <td><button>9</button></td>
                    <td><button>X</button></td>
                </tr>
                <tr>
                    <td><button>4</button></td>
                    <td><button>5</button></td>
                    <td><button>6</button></td>
                    <td><button>-</button></td>
                </tr>
                <tr>
                    <td><button>1</button></td>
                    <td><button>2</button></td>
                    <td><button>3</button></td>
                    <td><button>+</button></td>
                </tr>
                <tr>
                    <td><button>0</button></td>
                    <td><button>.</button></td>
                    <td><button>/</button></td>
                    <td><button>=</button></td>
                </tr>
            </table>
        </div>
    </div>

</body>
<script src="index.js"></script>

</html>
```
### index.js
```
let screen = document.getElementById('screen');
buttons = document.querySelectorAll('button');
let screenValue = '';
for (item of buttons) {
    item.addEventListener('click', (e) => {
        buttonText = e.target.innerText;
        console.log('Button text is ', buttonText);
        if (buttonText == 'X') {
            buttonText = '*';
            screenValue += buttonText;
            screen.value = screenValue;
        }
        else if (buttonText == 'C') {
            screenValue = "";
            screen.value = screenValue;
        }
        else if (buttonText == '=') {
            screen.value = eval(screenValue);
        }
        else {
            screenValue += buttonText;
            screen.value = screenValue;
        }

    })
}
```
### tyle.css
```
#container{
    text-align: center;
    margin-top:100px;
    padding-left:200px;
    padding-right:200px;
}

#table{
    margin: auto;

}

input{
    border-radius: 21px;
    border: 10px solid #FFA6F9;
    font-size:52px;
    height: 65px;
    width: 456px;
}

button{
    border-radius: 30px;
    font-size: 35px;
    background: #FFA6F9;
    width: 102px;
    height: 90px;
    margin: 6px;
}

#calculator{ 
    border: 15px solid #6B4669;
    background-color:#A63491;
    padding: 23px;
    border-radius: 53px;
    display: inline-block;
    
}
h1{
    font-size: 50px;
    font-family:Javanese Text, Courier, monospace;
    font-style:italic;
}
```
## Output :
### addition :
![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/0ba5efca-80ab-43a7-9e8d-d1d796039581)
![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/d1dc0460-1768-4c46-a7a8-b26b514f3089)

### Subraction:
![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/9fa24c50-4707-4dac-a655-cb00e25511e0)

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/702592ab-a5f9-47a8-9477-02d0167a0639)

### Multiplication :

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/5c76d7e0-9586-4734-bd74-7b9897290633)

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/95f5e413-123b-45b7-858e-18a0197603f0)

### Division (Remainder):

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/bb96b468-90be-4e6d-ae72-e45f4ae1c7dd)

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/7878c9e2-d7a0-4f16-95ac-ff2a5c059350)

### Division(Quotient):

![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/db2c9b5e-01b8-42df-a4bb-f13264795eac)


![image](https://github.com/naveenaakumarasamy/CALCULATOR-TASK1/assets/113497406/078da691-c3ce-4e0f-9e5e-1bc1eb5e2de4)
