# html-of-clock-hotel.ng-internship


<!DOCTYPE html>

<title>hotel.ng stage 1</title>
<link rel ="stylesheet" href="hnng.css">

<html>
<head>
        <script>
                function startTime() {
                    var today = new Date();
                    var h = today.getHours();
                    var m = today.getMinutes();
                    var s = today.getSeconds();
                    m = checkTime(m);
                    s = checkTime(s);
                    document.getElementById('txt').innerHTML =
                    h + ":" + m + ":" + s;
                    var t = setTimeout(startTime, 500);
                }
                function checkTime(i) {
                    if (i < 10) {i = "0" + i};  // add zero in front of numbers < 10
                    return i;
                }
                </script>
                
</head>

<body>
    <body onload="startTime()">
        
        <div id="container">
                <img src="MacBook Pro.jpg">
                <div id="txt"></div>
               
        </div>
        


</body>

