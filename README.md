 Technologywala
 
 

<html lang="en">

<head>
  <meta charset="utf-8">
  <meta content="width=device-width, initial-scale=1.0" name="viewport">

  <title>the learing digitel marketing</title>
  <meta name="robots" content="noindex, nofollow">
  <meta content="" name="description">
  <meta content="" name="keywords">

 


<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
body {font-family: "Lato", sans-serif;}

/* Style the tab */
.tab {
  float: left;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
  width: 30%;
  height: 300px;
}

/* Style the buttons inside the tab */
.tab button {
  display: block;
  background-color: inherit;
  color: black;
  padding: 22px 16px;
  width: 100%;
  border: none;
  outline: none;
  text-align: left;
  cursor: pointer;
  font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current "tab button" class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  float: left;
  padding: 0px 12px;
  border: 1px solid #ccc;
  width: 70%;
  border-left: none;
  height: 300px;
  display: none;
}

/* Clear floats after the tab */
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Hover Tabs</h2>
<p>Move the mouse over a button inside the tabbed menu:</p>

<div class="tab">
  <button class="tablinks" onmouseover="openCity(event, 'London')">London</button>
  <button class="tablinks" onmouseover="openCity(event, 'Paris')">Paris</button>
  <button class="tablinks" onmouseover="openCity(event, 'Tokyo')">Tokyo</button>
</div>

<div id="London" class="tabcontent">
  <h3>London</h3>
  <p>London is the capital city of England.</p>
</div>

<div id="Paris" class="tabcontent">
  <h3>Paris</h3>
  <p>Paris is the capital of France.</p> 
</div>

<div id="Tokyo" class="tabcontent">
  <h3>Tokyo</h3>
  <p>Tokyo is the capital of Japan.</p>
</div>

<div class="clearfix"></div>

<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
   
</body>
</html> 

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
</style>
</head>
<body>

<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="img_nature_wide.jpg" style="width:100%">
  <div class="text">Caption Text</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="img_snow_wide.jpg" style="width:100%">
  <div class="text">Caption Two</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="img_mountains_wide.jpg" style="width:100%">
  <div class="text">Caption Three</div>
</div>

<a class="prev" onclick="plusSlides(-1)">❮</a>
<a class="next" onclick="plusSlides(1)">❯</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>

<script>
let slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
}
</script>

</body>
</html> 


<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Impact Bootstrap Template Demo</title>
  <meta name="robots" content="noindex, nofollow">
    <link rel="stylesheet" href="https://bootstrapmade.com/assets/css/demo.css?v=5.0">
  </head>

<body>
  <header id="header">

    <div class="logo">
      <a href="https://bootstrapmade.com/" rel="home" title="Bootstrap Templates | Premium & Free Download" title="Back to BootstrapMade Homepage"><img alt="BootstrapMade" src="https://bootstrapmade.com/assets/img/logo.png"></a>
    </div>
    <div class="preview-devices">
      <ul>
        <li class="preview-test preview-devices-active" id="preview-test-desktop" title="Desktop preview of the  Impact template"><a href=""><svg class="icon icon-preview"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#preview"/></svg></a></li>
        <li class="preview-test" id="preview-test-tablet" title="Tablet preview of the Impact template"><a href=""><svg class="icon icon-tablet"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#tablet"/></svg></a></li>
        <li class="preview-test" id="preview-test-mobile" title="Mobile preview of the Impact template"><a href=""><svg class="icon icon-smartphone"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#smartphone"/></svg></a></li>
      </ul>
    </div>

    <div class="current-template">
              <a href="https://bootstrapmade.com/demo/Gp/" title="Previous Template: Gp" target="_top"><svg class="icon icon-chevron-left"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#chevron-left"/></svg></a>
            <a class="template-home" href="https://bootstrapmade.com/impact-bootstrap-business-website-template/" title="Impact Template Home Page">Impact</a>
            <a href="https://bootstrapmade.com/demo/PhotoFolio/" title="Next Template: PhotoFolio" target="_top"><svg class="icon icon-chevron-right"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#chevron-right"/></svg></a>
          </div>
    
    <div class="navigate">
      <a href="https://bootstrapmade.com/demo/templates/Impact/" target="_top" title="Hide the demo bar"><svg class="icon icon-external-link"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#external-link"/></svg></a>
      <a class="download" href="https://bootstrapmade.com/impact-bootstrap-business-website-template/#download" title="Download the Impact Template"><svg class="icon icon-download"  fill="currentColor"><use xlink:href="https://bootstrapmade.com/assets/img/icons.svg#download"/></svg> <span>Free Download</span></a>
    </div>

  </header>


  <div id="preview">
    <iframe id="preview-frame" class="preview-desktop" src="https://bootstrapmade.com/demo/templates/Impact/" frameborder="0"></iframe>
  </div>
