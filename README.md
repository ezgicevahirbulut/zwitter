<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<link href="zwitter.css" type="text/css" rel="stylesheet" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<script>
  function myFonk(){


    var node=document.createElement("p");
    var x =document.getElementById("ad:").textContent+ document.getElementById("text").value  ;
  var textnode=document.createTextNode(x);
  node.appendChild(textnode);
  document.getElementById("aa").appendChild(node);
  }
</script>
<body>

<div class="header">
  <h1>Zwitter</h1>
  <h3>Zwitter'a Hoşgeldiniz!</h3>
</div>

<div class="topnav">
  <a href="#"><i class="fa fa-home" aria-hidden="true"></i>&nbsp;Anasayfa</a>
  <a href="#"><i class="fa fa-bell" aria-hidden="true"></i>&nbsp;Bildirimler</a>
  <a href="#"><i class="fa fa-envelope" aria-hidden="true"></i>&nbsp;Mesajlar</a>
  Arama:
  <input type="text">
</div>

<div class="row">
  <div class="column side" sytle="background-color:#aaa";>
      <div class="center">
          <img src="foto.jpg" class="circle" alt="Avatar" style="height:106px;width:106px" >
      </div>
      <div class="card round white">
        <div class="container"></div>
      </div>
    <h2 id="ad:">Ezgi:</h2>
    <p >Kullanıcı Adı:@yabanyemisi<br>
    "Eskişehir,TR"<br>
    03.06.1994</p>
  </div>
  <div  class="column middle" style="background-color:#F3C9C9";>
    <div class="row-padding">
      <div id="aa" class="col m12">
        <div class="card-2 round white">
          <div class="container padding">
            <h6 class="opacity">Bir zweet ekle:</h6>
            <input id="text" type="textbox" class="x"  placeholder="Neler oluyor?">
            <button type="button" onclick="myFonk()" style="font-size:15px">Zweetle</button>
          </div>
        </div>
      </div>
    </div>
    <button type="button" style="font-size:15px">Beğen
      <i class="fa fa-heart"></i>
    </button>
          <button type="button" style="font-size:15px">Yorum Yap!
              <i class="fa fa-comment"></i>
          </button>
    <br>
  </div>
  <div class="column side" style="background-color:#FAAAAA";>
    <h2>Kimi Takip Etmeli?</h2>
    <div class="container card-2 margin"><br>
        <img src="zymrt.jpg" alt="Avatar" class="left circle margin-right" style="width:60px;">
    <span class="right opacity"></span>
    <h4>Xxxx Yyyy</h4><br>
    <div class="row opacity">
      <div class="half">
        <button class="button block green section" title="Kabul Et" onclick="kabulet">Kabul Et<i class="fa fa-check"></i></button>
      </div>
      <div class="half">
        <button class="button block red section" title="Reddet!" onclick="reddet">Reddet!<i class="fa fa-remove"></i></button>
      </div>
    </div>
    <hr class="clear">
      </div>
  </div>
</div>
<div class="footer">
    <h2>Gündem</h2>
<p>#HelloWorld</p></div>
</body>
</html>


* {
    box-sizing: border-box;
}

body {
  margin: 0;
}

/* Style the header */
.header {
    background-color: #f1f1f1;
    padding: 25px;
    text-align: center;
    color: white;
    text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
}

/* Style the top navigation bar */
.topnav {
    overflow: hidden;
    background-color: #0ABFEC;
    float:center;
    border: 1px;
}

/* Style the topnav links */
.topnav a {
    float: left;
    display: block;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    border:1px solid gainsboro;
}

/* Change color on hover */
.topnav a:hover {
    background-color: #ddd;
    color: black;
}

/* Create three unequal columns that floats next to each other */
.column {
    float: left;
    width:33.33%;
    padding: 10px;
    height: 300px;
    position: relative;
}

/* Left and right column */
.column.side {
    width: 25%;
    position: relative;
    left: 10px;
}

/* Middle column */
.column.middle {
    width: 50%;
    position: relative;
    left:10px;
}

/* Clear floats after the columns */
.row:after {
    content: "";
    display: table;
    clear: both;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media (max-width: 600px) {
    .column.side, .column.middle {
        width: 100%;
    }
}
.footer{
    background-color: #f1f1f1;
    padding:10px;
    text-align: left;
}
div.foto{
    width:250px;
    box-shadow: 0 4px 8px 0 rgba(0,0,0, 0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
    text-align:center;
}
img{
    border-radius: 50%;
}
.x{
    border: width border-style color;
}
