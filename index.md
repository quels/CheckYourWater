<!DOCTYPE html>
<html>
  <head>
    <link href="https://fonts.googleapis.com/css?family=Supermercado+One" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Encode+Sans+Semi+Expanded" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Courgette" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Philosopher" rel="stylesheet">

    <style media="screen">
    .alert {

position: fixed;
left: 23%;
top: 77%;

    }
.Logo {
background-color: #e6ecff;
width: 1355px;
height: 60px;

}
    .LogoT {
font-family: 'Supermercado One', cursive;
font-size: 40px;

    }
body {
  background-image: url("http://dullahansoft.com/pixel/wp-content/uploads/2015/03/water.png");
}
    .info {
      background-color: white;
    position: fixed;
    top: 35%;
    left: 10%;



    }
    table, th, td {
        border: 3px solid black;
        font-size: 48px ;
        font-family: 'Philosopher', sans-serif;

    }
    .updateb {
      font-size: 30px;
      position: fixed;
      left:15%;
      top:77%;
      color: green;


    }
    </style>
  <link rel="stylesheet" type="text/css" href="Style_home.css">
<script type="text/javascript" href="script.js">

</script>
    <title>Check Your Water</title>
  </head>
  <body background="background.png">
<center>
    <div class="Logo">
    <h1 class = "LogoT">Check Your Water ☻</h1>
    </div>
  </center>
    <div class="info">
      <button class="updateb" type="button" onclick="update()">Update</button>
      <table>
  <tr>
    <th>Parameter</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>TSS</td>
    <td id=Tss></td>
  </tr>
  <tr>
    <td>pH</td>
    <td id=pH></td>
  </tr>
  <tr>
    <td>Ec</td>
    <td id=Ec></td>
  </tr>
</table>
    </div>

<script type="text/javascript">
function update() {
var pH = Math.floor((Math.random() * 10) + 3);
document.getElementById("pH").innerHTML = pH + ("(mol/L)");

var Ec = Math.floor((Math.random() * 4) + 1);
document.getElementById("Ec").innerHTML = Ec + (" (mS)");

var Tss = Math.floor((Math.random() * 100) + 300);
document.getElementById("Tss").innerHTML = Tss + (" (mg/L)");
}

</script>
  </body>
</html>
