<!DOCTYPE HTML>

<html>
<head>
    <title> blood </title>

<!--Little CSS fade in -->
<style>
    
    body{
        
        margin-left: 350px;
        margin-top: 95px;
        
    }
    
      body{
       background-image: url('p2.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
     }
 
    
    img{
        height: 700px;
        
    }
    
    button{
        margin-top: 60px;
        margin-left:550px;
        background-color: ghostwhite;
        color: black;
    }

.fade-in{
  -webkit-animation: fade-in 2s ease;
  -moz-animation: fade-in ease-in-out 1s both;
  -ms-animation: fade-in ease-in-out 1s both;
  -o-animation: fade-in ease-in-out 1s both;
  animation: fade-in 1s ease;
  visibility: visible;
  -webkit-backface-visibility: hidden;
}

@-webkit-keyframes fade-in{0%{opacity:0;} 100%{opacity:1;}}
@-moz-keyframes fade-in{0%{opacity:0} 100%{opacity:1}}
@-o-keyframes fade-in{0%{opacity:0} 100%{opacity:1}}
@keyframes fade-in{0%{opacity:0} 100%{opacity:1}}

</style>
</head>
<body>

        
<!--We append on this div-->
<div id="banner-load"></div>

<!--Don't forget Jquery-->
<script type='text/javascript' src='http://ajax.googleapis.com/ajax/libs/jquery/1.8/jquery.min.js'></script>

<!--New images on load -->
<script>
//Add your images, we'll set the path in the next step
    var images = ['blood1.jpg', 'blood2.jpg', 'blood3.jpg', 'blood4.jpg', 'blood6.jpg', 'blood7.jpg' ];
    
//Build the img, then do a bit of maths to randomize load and append to a div. Add a touch off css to fade them badboys in all sexy like.
    $('<img class="fade-in" src="images/' + images[Math.floor(Math.random() * images.length)] + '">').appendTo('#banner-load');
</script>

 <button type="submit"  onClick="location.reload()">click</button>
    
</body>
</html>
