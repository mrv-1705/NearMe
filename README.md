# Ex04 Places Around Me
## Date: 14-04-24

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{margin:0;}
    </style>
    <script>
        function coordinate(event){
            let x= event.clientX;
            let y=event.clientY;
            document.getElementById('text1').value=x;
            document.getElementById('text2').value=y;
        }
    </script>
</head>
<body>
    <h1 align="center" style="color: red;">EXP4</h1> <br>
    <h2 align="center" style="color: green;">Kurapati Vishnu Vardhan Reddy(212223040103)</h2>
    <br>
   <img src="map.png" width="1485" height="650" alt="" 
    usemap="#MapNew" onmousemove="coordinate(event)"> 
    <map name="MapNew">
        <area shape="rect" coords="480,347,622,390" href="https://saveetha.ac.in" alt="" title="Saveetha">
        <area shape="rect" coords="848,402,964,434" href="https://dmice.ac.in/" alt="" title="Dmi">
        <area shape="rect" coords="400,163,520,190" href="https://apollocollegeofeducation.ac.in/" alt="" title="Apollo College Of Education">
        <area shape="rect" coords="1365,110,1484,137" href="https://www.sreesasthaarts.in/" alt="" title="sree sastha arts">
    </map>
    <br>
   <center> x-coordinate
    <input type="text" name="" id="text1"></center>
    <br>
    <br>
   <center> y-coordinate
    <input type="text" name="" id="text2"></center>
</body>
</html>
```

## OUTPUT
![alt text](mapoutput.png)






## RESULT
The program for implementing image maps using HTML is executed successfully.
