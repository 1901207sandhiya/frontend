# frontend
frontend of shopping website
<html lang="en">
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>lindo beauty care </title>
<style>
*{
box-sizing:border-box;
}
body {
background-color:FF7F50;
  font-family: verdana, Helvetica, verdana;
  margin: 0;
}
.mySlides {
display: none
}
img {
vertical-align: middle;
}
.slideshow-container {
  max-width: 1450px;
  position: relative;
  margin: auto;
}
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
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}


.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}


.text {
  color:#DC143C ;

 font-family: "Sofia", sans-serif;
  font-size: 70px;
  padding: 8px 12px;
  position: absolute;
  top: 25px;
  width: 100%;
  text-align: center;
}
.smalltext{
font-family: "Lucida Console", "Courier New", monospace;
 color:black ;
  font-size:40px;
  padding: 8px 12px;
  position: absolute;
  bottom: 10px;
  width: 100%;
  text-align: center;
}

.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}


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


.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
header {
  align:center;
  padding: 20px;
  text-align: center;
  font-size:25px;
background-color:FF7F50	;
color:white;
  }
.header h1 {
  font-size: 40px;
}
.section
{
font-size:25px;
}
.navbar {
  overflow: hidden;
  background-color:#DC143C ;
  position: sticky;
  position: -webkit-sticky;
  top: 0;
}
.navbar a {
  float: left;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 20px;
  text-decoration: none;
}
.navbar a.right {
  float: right;
}
.navbar a:hover {
  background-color:F0FFF0 ;
  color: black;
}
.navbar a.active {
  background-color:E9967A ;
  color: white;
}
.h2{
  font-size:80px;
}
.row {  
   background-image: url('');
  display: -ms-flexbox; /* IE10 */
  display: flex;
  -ms-flex-wrap: wrap; /* IE10 */
  flex-wrap: wrap;
}
.side {
  -ms-flex: 30%; 
  flex: 30%;
  background-color:F0FFF0 ;
  padding: 20px;
}
.main {   
  -ms-flex: 70%; 
  flex: 70%;
  background-color:cornsilk;
  padding: 20px;
}
#more {
display: none;
}
.footer {
  padding: 20px;
  text-align: center;
  background-color:black;
  color:white;
}
@media screen and (max-width: 700px) {
  .row {   
    flex-direction: column;
  }
}
@media screen and (max-width: 500px) {
  .navbar a {
    float: none;
    width: 50%;
  }

a
{
color:orange;
}

</style>
</head>
<body>
<h2><center><b>LINDO BEAUTY CARE</></b></center></h2>
<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="https://www.skincenterofsouthmiami.com/wp-content/uploads/2018/06/Skin-Center-of-South-Miami-Facials-and-Skin-Care.jpg" width="100%">
  
<div class="smalltext"> Handmade products with love and care</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="https://images.squarespace-cdn.com/content/v1/5e74e2d8c4808e25fd715035/1585151769806-60TUML5D9Q2XE804UTB8/HawthornHandmadeSkincare-02.jpg?format=2500w" style="width:100%">
  <div class="text">SKIN CARE PRODUCTS</div>
<div class="smalltext"> Handmade products with love and care</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="https://i.pinimg.com/originals/2b/1f/56/2b1f56097e6a23c5a7e59d30485ab81f.jpg" heigth="80%" width="100%">
  <div class="text">HAIR CARE PRODUCTS</div>
<div class="smalltext"> Handmade products with love and care</div>
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
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
<div class="navbar">

  
  <a href="LINDOBEAUTYCARE.html" class="active">Home</a>
  <a href="skin.html">skin care products</a>
  <a href="haircareproducts.html">hair care products</a>
  <a href="aboutus.html" >About us</a>
</div>
<div class="row">
  <div class="side">
    <h2>TOP SELLING PRODUCTS</h2>
  <img src="https://www.lindobeautycare.in/product-images/15.jpeg/369677000000043124/700x700" class="center" style="width:90%;height:20%;">CHARCOAL SOAP<br><br>

<img src="https://www.lindobeautycare.in/product-images/11.jpeg/369677000000043116/700x700" class="center" style="width:90%;height:20%;">SKIN GLOW SERUM
<img src="https://www.lindobeautycare.in/product-images/0T0A0683.JPG/369677000000072115/300x300" class="center" style="width:90%;height:20%;"> HAIR GROWTH OIL
<img src="https://www.lindobeautycare.in/product-images/2.jpeg/369677000000043096/300x300" class="center" style="width:90%;height:20%;">MAGIC LOTION

     </div>
  <div class="main">
    <h2>SKIN CARE BLOGS</h2>
   <section><i><img src="https://cdn.shopify.com/s/files/1/0034/7901/1441/articles/How_To_Beauty_Four-206-over-counter-dark-spot-correctors-homepage-1280x720_400x.jpg?v=1612590320" width=50% height=20%><br>
We have all been exposed to acne, blackheads, and dark spots at least once in our lifetime. While the former two are easily treatable and are not stubborn to get rid of, a dark spot indeed occurs on your skin for an extended stay.<br>

Dark spots, also known as hyperpigmentation, are the spots on our skin that may be caused by many reasons. Some of them are:
<ol>
<li><b>Acne:</b> We have all been a victim of acne, and we all are very well aware that it does not just look ugly when it arrives and stays, but sometimes it also leaves behind a  reminder of its existence. That dark spot is often extensively challenging to remove.</li>
<li><b>Hormonal changes:</b> Hormonal changes can take a significant toll on some, no matter how natural it is. A type of skin pigmentation, Melasma appears as dark patches on the cheeks or forehead.</li>
<li><b>Excessive sunburn:</b> The harmful UV rays have their way to affect our skin so brutally that these scars stay on the skin certainly for years. Be it sun spots, hyperpigmentation, liver spots, or solar lentigines, these spots make the affected ones, cry for help.</li>
<li><b>Inflammation: </b>When riding a bike, or just strolling down the road and unexpectedly kissing the earth, or trying a new recipe in the kitchen and burning your side, our incompetent self sometimes take a violent spill. These reckless incidents may cause an unpleasant scar on our face or body, which may be extremely difficult to treat.</li>
These spots are so stubborn to treat sometimes that it may take years to bid them goodbye, leaving us exasperated and oblivious as to what measures to take.</i></section><a href="https://www.lindobeautycare.in/products/aloe-vera-gel/369677000000038867">Product Recommanded for dark spots</a><br><br>
   
   <section><i><img src="https://cdn.shopify.com/s/files/1/0034/7901/1441/articles/Loreal-Paris-BMAG-Article-10-Things-You-Shouldnt-Do-If-You-Have-Oily-Skin-D_400x.jpg?v=1603700677" width=50% height=20%><br>
Toners and mists for oily skin are a great blessing. People with oily skin must definitely indulge in a skincare routine where toner plays the ace. It not only sets the skin but is also successful in controlling the sebum production that proves to be a boon for oily skin holders. Like Toner, mist is an underrated product too yet crucial in providing your oily skin a bright glow while keeping it non-greasy.<br>
Deyga Organics has formulated toners and mists considering the need of every skin type. Some of them best designed for oily skin are;<br>

Basil Toner: Oily skin is more prone to acnes. Basil being a natural detoxifier, banishes acnes along with endowing a sheer radiance to your face.<br>

<ol><li><b>Tea tree Facial Toner:</b> It deeply cleans your skin by kicking out impurities responsible for clogged pores. Healthy, glowing and clear skin is not far away when Tea tree toner plays!</li>

<li><b>Lemon Mist: </b>Lemon mist is a ‘must’ in the good books of oily skin especially. It controls oil, battles blemishes, dark spots and pigmentation like a pro.</li>

<li><b>Ylang Ylang Mist:</b> Ylang Ylang is the most effective remedy for oily skin. This toner refreshes skin through and through along with safeguarding it against pollution from penetrating your skin</li>.</i></section><br><br>
<a href="https://www.lindobeautycare.in/products/activated-charcoal-soap/369677000000042162">Products Recommended for oily skin</a>
  </div>
</div>



<div class="footer">
  <P><u>General Information</u><br><br>
  <p><U><b>Conact us on <br> 9999963668<b></U></p>
  
No Product Replacement After 10 Days Of Purchase</P>
<p><u>VISIT US @ </u><br><br>
<a href="https://www.instagram.com/lindo_beauty_care/?hl=en"><img src="https://i.kym-cdn.com/entries/icons/original/000/010/944/instagram.jpg" width="5%" height="5%"></a><br><br>
<a href="https://www.youtube.com/channel/UCFQ4bBzAt358kZSSzSAcPfQ"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/1280px-YouTube_full-color_icon_%282017%29.svg.png" width="5%" height="5%"></a></p>
<p> 2021 Lindo Beauty Care Pvt.Lmd,All rights reserved </p>
</div>
</body>
</body>
</html>
