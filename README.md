cam
===

<!doctype html>  
<html lang="en">  
<head>  
  <meta charset="utf-8">  
  <title>jQuery.data demo</title>  
  <style>  
  div {  
    color: blue;  
  }  
  span {  
    color: red;  
  }  
  </style>  
  <script src="//code.jquery.com/jquery-1.10.2.js"></script>  
</head>  
<body>  
   
<div>  
  The values stored were  
  <span></span>  
  and  
  <span></span>  
</div>  
   
<script>  
var div = $( "div" )[ 0 ];  
jQuery.data( div, "test", {  
  first: 16,  
  last: "4659"  
});  
$( "span:first" ).text( jQuery.data( div, "test" ).first );  
$( "span:last" ).text( jQuery.data( div, "test" ).last );  
</script>  
   
</body>  
</html>  
