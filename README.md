# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MATHEMATICS CALCULATION</title>
    <style>
        * {
  box-sizing: border-box;
  font-family:  georgia, Arial, Helvetica, sans-serif;
}
body {
  background-color: #a2d5c6;
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
  padding-top: 30px;
  padding-left: 300px;
}
.content {
  display:block;
  width: 500px;
  background-color:#e52165;
  min-height: 300px;
  font-size: 20px;
}
h1{
    text-align: center;
    padding-top: 25px;
}
.formelement{
    text-align: center;
    margin-top: 5px;
    margin-bottom: 5px;
}
.footer {
  display: inline-block;
  width: 100%;
  height: 40px;
  background-color:#5c3c92;
  text-align:right;
  padding-top: 60px;
  margin: 0px 0px 0px 0px;
  color: #000000;
}
    </style>
</head>
<body>
    <div class="container">
        <div class="content">
            <h1>AREA OF RECTANGLE</h1>
            <form>
                <div class="formelement">
                    <label for="bedit">LENGTH   :</label>
                        <input type="text" name="base" id="bedit" value="0"/> <label>cm</label>
                </div>
                <div class="formelement">
                    <label for="hedit">WIDTH :</label>
                        <input type="text" name="height" id="hedit" value="0"/> <label>cm</label>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="addbutton"/>
                </div>
                <div class="formelement">
                    <label for="cedit">Area :</label>
                        <input type="text" id="cedit" value="0" readonly/> <label>cm<sup>2</sup></label>
                <div>
                   Formula is : A=length*width
                </div>        
                </div>
                <div class="footer">
                 Developed by Dhanashree
                  </div>
            </form>
            </div>
    </div>
    <script type="text/javascript">
        var button;
        button=document.querySelector("#addbutton");
        button.addEventListener("click",function(){
            var btext,htext,ctext;
            var bval,hval,cval;
            btext=document.querySelector("#bedit");
            htext=document.querySelector("#hedit");
            ctext=document.querySelector("#cedit");
            bval=parseInt(btext.value);
            hval=parseInt(htext.value);
            cval=0.5*bval*hval;
            ctext.value=""+cval;
            var namefield
            var bedit,reg,res;
            namefield=document.querySelector("#bedit");
            bedit = namefield.value;
            reg = new RegExp("[0-9].[0-9]");
            res = bedit.match(reg);
            if(res==null)
            {
                alert("Please Enter a valid Number");
            }
            else{
                alert("Answer is");
            }
            var namefield
            var hedit,reg,res;
            namefield=document.querySelector("#hedit");
            hedit = namefield.value;
            reg = new RegExp("[0-9].[0-9]");
            res = hedit.match(reg);
            if(res==null)
            {
                alert("Please Enter a valid Number");
            }
            else{
                alert("Answer is");
            }
            
            });

 </script>
    </br>
    <div class="container">
        <div class="content">
            <h1>AREA OF TRIANGLE</h1>
            <form>
                <div class="formelement">
                    <label for="Redit">HEIGHT    :</label>
                        <input type="text" id="Redit" value="0"/> <label>cm</label>
                </div>
                <div class="formelement">
                    <label for="Hedit">BASE :</label>
                        <input type="text" id="Hedit" value="0"/> <label>cm</label>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="vbutton"/>
                </div>
                <div class="formelement">
                    <label for="vedit">AREA :</label>
                        <input type="text" id="vedit" value="0" readonly/> <label>cm<sup>2</sup></label>
                <div class="formelement">
                formula is : A=HEIGHT*BASE/2          
                </div>
                    
</div>
                <div class="footer">
                    Developed by Dhanashree
                     </div>
            </form>
 </div>
    </div>
    <script type="text/javascript">
        var button;
        button=document.querySelector("#vbutton");
        button.addEventListener("click",function(){
            var Rtext,Htext,vtext;
            var Rval,Hval,vval;
            Rtext=document.querySelector("#Redit");
            Htext=document.querySelector("#Hedit");
            vtext=document.querySelector("#vedit");
            Rval=parseInt(Rtext.value);
            Hval=parseInt(Htext.value);
            vval=3.14*Rval*Rval*Hval*0.3;
            vtext.value=""+vval;
            var namefield
            var Redit,reg,res;
            namefield=document.querySelector("#Redit");
            Redit = namefield.value;
            reg = new RegExp("[0-9].[0-9]");
            res = Redit.match(reg);
            if(res==null)
            {
                alert("Please Enter a valid Number");
            }
            else{
                alert("Anawer is");
            }
            var namefield
            var hedit,reg,res;
            namefield=document.querySelector("#Hedit");
            Hedit = namefield.value;
            reg = new RegExp("[0-9].[0-9]");
            res = Hedit.match(reg);
            if(res==null)
            {
                alert("Please Enter a valid Number");
            }
            else{
                alert("Answer is");
            }
            
        });
</script>

</body>
</html>
~~~
## OUTPUT:

![output](.//PC.jpeg)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
