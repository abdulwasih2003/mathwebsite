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
    <title>Mathematical Calculations</title>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color:rgb(1, 0, 12);
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
}
.content {
  display: block;
  width: 100%;
  background-color: #3d484d;
  min-height: 500px;
  margin-top: 150px;
}
.content2{
    display: block;
    width: 100%;
    background-color: #3d484d;
    min-height: 500px;
    margin-top: 150px;
    margin-bottom: 150px;
}
h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
}
.formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;

}
.by{
    text-align: center;
    color: rgb(245, 240, 240);
}
    </style>
    
</head>
<body>
    <div class="container">
        <div class="content">
            <h1><B>Area of Triangle</B></h1>
            <form>
                <div class=formelement>
                    <lable for="aedit">Base:</lable>
                    <input type="text" id="aedit" value="0">
                    <lable for="aedit">Meters</lable>
                </div><br>
                <div class=formelement>
                    <lable for="bedit">Height:</lable>
                    <input type="number" id="bedit" value="0">
                    <lable for="aedit">Meters</lable>
                </div><br>
                <div class=formelement>
                    <input type="button" value="Calculate Area" id="calbutton">
                </div><br>
                <div class=formelement>
                    <lable for="cedit">Area:</lable>
                    <input type="number" id="cedit" readonly="0">
                    <lable for="aedit">Meter<sup>2</sup></lable>
                </div><br>
                <div class=formelement>
                    Formula : Area = (Base*Height)/2
                </div>
            </form>
        </div>
        <script>
            function validate() {
                var user1=document.getElementsById("aedit").value;
                var user1=document.getElementsById("bedit").value;
                var re= /^\d+$/;
                if(re.test(user1)){
                    return true
                }
                else{
                    alert("Enter a valid input");
                    user2.style.border="red solid 3px";
                    return false;
                }
            }
        </script>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton");
            button.addEventListener("click",function(){
                var atext,btext,ctext;
                var aval,bval,cval;
                atext=document.querySelector("#aedit");
                btext=document.querySelector("#bedit");
                ctext=document.querySelector("#cedit");

                aval=parseInt(atext.value);
                bval=parseInt(btext.value);
                cval=0.5*aval*bval;
                ctext.value=""+cval;
            });
        </script>
        <div class="content2">
            <h1><B>Volume of Cone</B></h1>
            <form>
                <div class="formelement">
                  <lable for="radiusedit">Radius:</lable>
                  <input type="number" id="radiusedit" value="0">
                  <lable for="aedit">Meters</lable>
                </div><br>
                <div class="formelement">
                  <lable for="heightedit">Height:</lable>
                  <input type="number" id="heightedit" value="0">
                  <lable for="aedit">Meters</lable>
                </div><br>
                <div class="formelement">
                  <input type="button" value="Calculate Volume" id="calbutton">
                </div><br>
                <div class="formelement">
                  <lable for="volumeedit">Volume:</lable>
                  <input type="number" id="volumeedit" readonly="0">
                  <lable for="aedit">Meter<sup>3</sup></lable>
                </div><br>
                <div class="formelement">
                Formula : Volume=(π*Radius<sup>2</sup>*Height)/3
                </div><br>
                
            </form>
    
            </div>
        </div>
        <script>
            function validate() {
                var user1=document.getElementsById("radiusedit").value;
                var user1=document.getElementsById("heightedit").value;
                var re= /^\d+$/;
                if(re.test(user1)){
                    return true
                }
                else{
                    alert("Enter a valid input");
                    user2.style.border="red solid 3px";
                    return false;
                }
            }
        </script>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton");
          button.addEventListener("click",function(){
            
              var radiustext,heighttext,volumetext;
              var aval,bval,cval;
    
              radiustext=document.querySelector("#radiusedit");
              heighttext=document.querySelector("#heightedit");
              volumetext=document.querySelector("#volumeedit");
      
              aval=parseInt(radiustext.value);
              bval=parseInt(heighttext.value);
              cval=3.14*aval*aval*bval/3;
              ctext.value=""+cval;
        
      
            });
                  
        </script>     

     <footer> <p class="by"><B>Developed by : Syed Abdul Wasih H </B></p></footer>
</body>
</html>
~~~

## OUTPUT:

![output](1.png)
![output](2.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
