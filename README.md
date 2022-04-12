
<!DOCTYPE html>
<html>
<head>
    <title>c10udz</title>
         <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1" crossorigin="anonymous">
         <script src="https://kit.fontawesome.com/6dbcb3829c.js" crossorigin="anonymous"></script><link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.15.2/css/all.css" integrity="sha384-vSIIfh2YWi9wW0r9iZe7RJPrKwp6bG+s9QZMoITbCckVJqGCCRhc+ccxNcdpHuYu" crossorigin="anonymous">
         <link rel="shortcut icon" href="https://c10udz.github.io/favicon.ico">
    <style>

@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:wght@300&family=Oswald&display=swap');

body {
  background-color: black;
 
}
#hero img {
    height: 100vh;
    width: 100%;
    background-position: absolute;
    z-index: 10;
    object-fit: cover;
}

#hero .content {
    background: rgba(0,0,0,0.7);
    height: 100%;
    width: 100%;
    z-index:20;
    position:absolute;
    top:0;
    left:0;
}

.switch {
    position:absolute;
    display: inline-block;
    width: 60px;
    height:34px;
    left: 5%;
    top:3%;
}

.switch input {
    opacity:0;
    width:0;
    height:0;
}

.slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left:0;
    right:0;
    bottom:0;
    background-color: #ccc;
    -webkit-transition: .4s;
}

.slider:before{
    position: absolute;
    content: "";
    height: 26px;
    width:26px ;
    left:4px;
    bottom: 4px;
    background-color: white;
    -webkit-transition: .4s;
}

input:checked + .slider {
    background-color: Tomato;
}

input:focus + .slider{
    box-shadow: 0 0 20px #2b78c2;
}
input:checked + .slider:before {
    transform: translateX(26px);
}
.slider.round{
    border-radius: 34px;
}
.slider.round:before {
    border-radius: 50%;
}

#clickme {
    color: #d9ddde;
    position:absolute;
    display: inline-block;
    width: 60px;
    height:34px;
    left: 5%;
    top:3%;
    text-indent: 12em;
    font-size: 18px; 
}


@import url('https://fonts.googleapis.com/css2?family=PT+Sans+Narrow:wght@700&display=swap');
#center {
font-family: 'PT Sans Narrow', sans-serif;
}

#button-text {
font-family: 'Open Sans Condensed', sans-serif;
}

#block {
  margin-left: 3px;
  margin-right:3px;
}


    </style>

</head>
<body>

<div id='hero'>

<img class="giphy" src="https://c10udz.github.io/bg2.gif">

<div class ="content d-flex align-items-center">

  <div id= "center" class ="container text-center">
    
    <h1 style="color:white; padding-bottom: 6px">c10udz</h1> 

    <span class="icons">
        <span id="block">
            <a style="color: Tomato;" href="javascript:window.open('https://discord.gg/fCgJYDCZzx', '_blank', 'toolbar=yes,scrollbars=yes,resizable=yes,top=50%,left=50%,width=1600,height=800');" target="_blank"><i class="fab fa-discord fa-2x" ></i></a>
        </span>
        <span id="block">
            <a style="color: Tomato;" href="javascript:window.open('https://www.youtube.com/channel/UC_kmPXv5sB4oNrvcl-FC5wA?view_as=subscriber', '_blank', 'toolbar=yes,scrollbars=yes,resizable=yes,top=50%,left=50%,width=1600,height=800');" target="_blank"><i class="fab fa-youtube fa-2x"></i></a>
        </span>
        <span id="block">
            <a style="color: Tomato;" href="javascript:window.open('https://github.com/c10udz', '_blank', 'toolbar=yes,scrollbars=yes,resizable=yes,top=50%,left=50%,width=1600,height=800');" target="_blank"><i class="fab fa-github fa-2x"></i></a>
        </span>
    </span>


  </div>

         <a>
      <img
        border="0"
        alt=""
        src="https://c10udz.github.io/blank.png"
        width="125"
        height="100"
        top="0"
        left="0"
        right="0"
        bottom="0"
      />
    </a>


  <div>
       <p id="button-text" class="switch" style="color:#d9ddde; margin-left:6px; margin-top: 45px;">Click me </p>
       <label class="switch">
        <input type="checkbox">
        <span class="slider round"></span>
        <audio id="myaudio"> <source src="https://c10udz.github.io/music2.mp3" type="audio/mp3"> </audio>
        </label>
    
  </div>

<script src="https://code.jquery.com/jquery-3.5.1.min.js" integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>

<script>
    $(document).ready (function(){
        var myAudio = document.getElementById("myaudio");
        var more = 0;
        $('.round').click (function(){
            if(more %2 ==0){
                $(myAudio)[0].play();
                more++;
            }
            else if(more % 2 != 0){
                $(myAudio)[0].pause();
                more++;
            }
        });
    });
</script>

</body>
</html>
