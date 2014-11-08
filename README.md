SimpleGallery_jQuery
====================
<!DOCTYPE html>
<head>
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>

<style>
body{
background-color: #5F9EA0;
}
img{
height:150px;
box-shadow: 0 0 10px rgba(0,0,0,0.5);
opacity:0.5;
}
div{
text-align: center;
align: botton;
}
</style>

<title>gallery</title>
<h1>Gallery</h1>
</head>
<body>
<div>
<img src="img1.jpg"/>
<img src="img2.jpg"/>
<img src="img3.jpg"/>
</div>
<script>
$(document).ready(function(){
  $("img").click(function(){
    $(this).animate({
      left:'250px',
      opacity:'1',
      height:'300px'
    }, 1000);
	
	$("img").not(this).animate({
      right:'250px',
      opacity:'0.5',
	  height:'150px'
  }, 1000);
});
});
</script> 

</body>
</html>
