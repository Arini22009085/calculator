# calculator

###index.html
```
<html>
    <head>
        <meta name="viewport" content="width=device-width,initial-scale=1.0">
        <title>calculator</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div class="container">
            <div class="calculator">
                <form>
                    <div class="display">
                        <input type="text" name="display">
                    </div>
                    <div>
                        <input type="button" value="AC" onclick="display.value ='' " class="opration" >
                        <input type="button" value="DE" onclick="display.value = display.value.toString().slice (0,-1)" class="opration">
                        <input type="button" value="." onclick="display.value +='.' " class="opration">
                        <input type="button" value="/" onclick="display.value +='/' " class="opration">

                    </div>
                    <div>
                        <input type="button" value="7" onclick="display.value +='7' ">
                        <input type="button" value="8" onclick="display.value +='8' ">
                        <input type="button" value="9" onclick="display.value +='9' ">
                        <input type="button" value="*" onclick="display.value +='*' " class="opration">

                    </div>
                    <div>
                        <input type="button" value="4" onclick="display.value +='4' ">
                        <input type="button" value="5" onclick="display.value +='5' ">
                        <input type="button" value="6" onclick="display.value +='6' ">
                        <input type="button" value="-" onclick="display.value +='-' " class="opration">

                    </div>
                    <div>
                        <input type="button" value="1" onclick="display.value +='1' ">
                        <input type="button" value="2" onclick="display.value +='2' ">
                        <input type="button" value="3" onclick="display.value +='3' ">
                        <input type="button" value="+" onclick="display.value +='+' " class="opration">

                    </div>
                    <div>
                        <input type="button" value="00" onclick="display.value +='00' ">
                        <input type="button" value="0" onclick="display.value +='0' ">
                        <input type="button" value="=" onclick="display.value=eval(display.value)"class="equal">
                    </div>
                </form>
            </div>
        </div>
    </body>
</html>
```
style.css

```
*{
    margin:0;
    padding:0;
    font-family:'poppins',sans-serif;
    box-sizing:border-box;
}
.container
{
    width:100%;
    height:100vh;
    background: gray;
    display: flex;
    align-items: center;
    justify-content: center;
}
.calculator
{
    background: #3a4452;
    padding:20px;
    border-radius: 10px;;
}
.calculator form input{
    border:0;
    outline:0;
    width:60px;
    height:60px;
    border-radius: 10px;
    box-shadow: -8px -8px 15px rgba(255,255,255,0.1),5px 5px 15px rgba(0,0,0,0.2);
    background:transparent;
    font-size: 20px;
    color: #fff;
    cursor:pointer;
    margin:10px;
}
form .display
{
    display:flex;
    justify-content: flex-end;
    margin:20px 0;
}
form .display input
{
    text-align: right;
    flex:1;
    font-size: 45px;
    box-shadow:none;
}
form input.equal
{
    width: 145px;
}
form input.opration
{
    color:#33ffd8;
}
```
###OUTPUT:

![Screenshot (29)](https://github.com/Arini22009085/calculator/assets/119643315/9b5d7dfd-aab9-456b-9917-06750c883196)

![Screenshot (30)](https://github.com/Arini22009085/calculator/assets/119643315/7da2929a-36a2-4067-9c6a-1cc01ab566ed)
