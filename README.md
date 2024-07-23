
const inputValue= document.getElementById("user-input");
const number = document.querySelectorAll(".Number").forEach(function(item){
item.addEventListener("click",function(e){
if(inputValue.innerText === "NaN"){
inputValue.innerText ="";
}
if(inputValue.innerText === "0"){
    inputValue.innerText = "";
}
//inputValue.innerText += innerHTML.trim();
});
});

function mul(a,b){
    return a*b;
}
document.getElementById("user-input").innerHTML = mul(4,5);
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="/calculator/style.css" rel="stylesheet">
<script type="javascript" src="/calculator/script.js"></lscript>

</head>
<body>
    
    <div class="container">
<div class="calc-text">
    <p name="user-input" id="user-input">0</p>
</div>
<div class="calc-keys">
<button type="button"  class="key-other">AC</button>
<button type="button"  class="key-other">DEL</button>
<button type="button"  class="key-other">%</button>
<button type="button"  class="key-operate">/</button>
<button type="button"  class="Number">7</button>
<button type="button"  class="Number">8</button>
<button type="button"  class="Number">9</button>
<button type="button"  class="key-operate">*</button>
<button type="button"  class="Number">4</button>
<button type="button"  class="Number">5</button>
<button type="button"  class="Number">6</button>
<button type="button"  class="key-operate">+</button>
<button type="button"  class="Number">1</button>
<button type="button"  class="Number">2</button>
<button type="button"  class="Number">3</button>
<button type="button"  class="key-operate">-</button>
<button type="button"  class="key-zero">0</button>
<button type="button"  class="Number">.</button>
<button type="button"  class="key-operate">=</button>


</div>
    </div>
  <!--  <script>
        function mul(a,b){
    return a*b;
}
document.getElementById("user-input").innerHTML = mul(4,5);
    </script>-->
</body>
</html>
*{
    margin: 0;
padding: 0;
font-family: Arial, Helvetica, sans-serif;
box-sizing: border-box;
}
body{
background-color: blueviolet;
min-height: 100vh;
display: flex;
align-content: center;
justify-content: center;
}
.container{
    width: 350px;
background-color: black;
padding: 25px;
border-radius: 10px;
margin: 40px;
}
.calc-text{
    margin-bottom: 25px;
padding-left: 5px;

}
.calc-text p{
    width: 280px;
font-size: 1.5rem;
background: transparent;
color: ghostwhite;
text-align: end;
border: none;
outline: none;
word-wrap: break-word;
word-break: break-all;
}
.calc-keys{
display: grid;
grid-template-columns: repeat(4,1fr);
grid-row-gap: 15px;
grid-column-gap: 10px;

}
button{
    border-radius: 70px;
width: 65px;
height: 65px;
font-size: 1.5rem;
border: none;
cursor: pointer;
}
button:active,
button:focus{
filter: brightness(120%);
}
.key-zero{
    grid-column: span 2;
    width: 150px;
height: 60px;
}
.key-other{
    color: chartreuse;
}
.key-operate{
    background-color: chartreuse;

}
