<!DOCTYPE html>
<html>
<head>
<title>Test</title>
</head>

<body>

<canvas id="canvasuses" width="180" height="90">
<p>Your browser does not support the HTML5 canvas element.</p>
</canvas>

<script type="text/javascript">

var c=document.getElementById("canvasuses");

var canvOK=1;
 try {c.getContext("2d");}
 catch (er) {canvOK=0;}
 if (canvOK==1)
 {
 var ctx=c.getContext("2d");
 var grd=ctx.createLinearGradient(0,0,200,0);
 grd.addColorStop(0,"red");
 grd.addColorStop(1,"white");
 ctx.fillStyle=grd;
 ctx.fillRect(100,10,150,80);
 }

 </script>

</body>
</html>
