# Event-Driven-Programming---Buttons
Event Driven Programming - Buttons
<!DOCTYPE html>
<!--This is a webpage made to fulfil assignment for CS102, 
    Event Driven Programming - Buttons Sanyerlis Camacaro     sancamac@uat.edu-->
    
<!--head-->

<head>
    <!--link js and style file-->
    <script src="programming buttons.js"></script>
    <link href="style.css" rel="stylesheet" type="text/css" />
    <!--title-->
    </title>

</head>


<body>
    <!--A table to put logo and title on same line-->
    <table>
        <!--table data-->
        <td><img src="UATspaceLogo-1.jpg"></td>
        <td style = "font-family: fantasy; font-weight: bold; font-size: x-large;"><h1></h1>UAT Space Program</h1></td>
    </table>   
<!--a border, a width, and a class style for the table-->
    <table border="2" id="data" width="40%" class="mainTable">
        <!--make the colums equal-->
        <col style="width: 20%">
        <col style="width: 20%">
        <!--table header-->
        <thead>
            <!--table rows font and alignment to the left-->
            <tr style = "font-family: fantasy;">
                <th align="left">Data Type</th>
                <th align="left">Reading</th>
            </tr>
        </thead>
        <!--body of the table-->
        <tbody>
            <tr id= "seconds"><td>Time Elapsed:</td><td>15 seconds</td></tr>
            <tr id= "latitude"><td>Latitude:</td><td>0</td></tr>
            <tr id= "longitude"><td>Longitude:</td><td>0</td></tr>
            <tr id= "gps_altitude"><td>GPS Altitude:</td><td>0</td></tr>
            <tr id= "BMP_sensor_alt"><td>BMP Sensor Altitude:</td><td>30383.04</td></tr>
            <tr id= "BMP_sensor_press"><td>BMP Sensor Pressure:</td><td>2.34</td></tr>
            <tr id= "BMP_sensor_temp"><td>BMP Sensor Temperature:</td><td>0</td></tr>
            <tr id= "dig_sensor_temp"><td>Digital Sensor Temperature:</td><td>24.12</td></tr>
            <tr id= "CSS_sensor_temp"><td>CSS Sensor Temperature:</td><td>25</td></tr>
            <tr id= "CSS_sensor_eCO2"><td>CSS Sensor eCO2:</td><td>400</td></tr>
            <tr id= "UV"><td>UV:</td><td>0</td></tr>
            <tr id= "accel_x"><td>Accel X:</td><td>-0.87</td></tr>
            <tr id= "accel_y"><td>Accel Y:</td><td>-0.02</td></tr>
            <tr id= "accel_z"><td>Accel Z:</td><td>9.61</td></tr>
            <tr id= "mag_x"><td>Magnetic X:</td><td>0.13</td></tr>
            <tr id= "mag_y"><td>Magnetic Y:</td><td>0.57</td></tr>
            <tr id= "gyro_x"><td>Gyro X:</td><td>4.66</td></tr>
            <tr id= "gyro_y"><td>Gyro Y:</td><td>0.01</td></tr>
            <tr id= "gyro_z"><td>Gyro Z:</td><td>-0.4</td></tr>
        </tbody>
    </table>
    
    <br>
    <br>
    <!--start and stop and button-->
    <button id="startButton" class="strtButton" onclick="start();">Start</button>
    <button id="stopButton" class="stpButton" onclick="stop();">Stop</button>
    <br>

    
</body>

</html>

body {
    background-color: white;
    background-image: linear-gradient(90deg, white 0%, rgb(57, 107, 160));
}

.mainTable {
    font-family: Helvetica;
    font-weight: bold;
}

.strtButton {
    background-color:rgb(131, 129, 129);
    width: 100px;
    height: 30px;
    border-radius: 12px;
    border-color:black;
    font-size: large;
    font-weight: bold;

}

.stpButton {
    background-color: rgb(131, 129, 129);
    width: 100px;
    height: 30px;
    border-radius: 12px;
    border-color:black;
    font-size: large;
    font-weight: bold;
}

//function for start button
function start(){
    document.getElementById("startButton").disabled = true;
    document.getElementById("stopButton").disabled = false;
    }
    //function for stop button
    function stop(){
        document.getElementById("stopButton").disabled = true;
        document.getElementById("startButton").disabled = false;
    }
    
