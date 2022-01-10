# frontend-
This is the sample front end page for a begginer
*CSS STYLES.

img{
  width:50px;
}
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,300;0,400;0,500;0,600;1,800&display=swap');

*{
 box-sizing: border-box;
margin: 0;
padding: 0;
font-family: "poppins", sans-serif;
} 
:root{
  --overlay-color:#03a9f4;
}
.showcase{
  position: absolute;
  right:0;
  width: 100%;
  min-height:100vh;
  padding: 100px;
  display: flex;
  justify-content: space-between;
  align-items:center;
  background: black;
  color:floralwhite;
  z-index: 2;
}
.showcase.active{
  right: 300px;
}
.showcase header {
position: absolute;
top:0;
left:0px;
width:100%;
padding: 40px 100px;
z-index: 1000;
display: flex;
align-items: center;
justify-content: space-between;
}
.logo {
  text-transform: uppercase;
  cursor: pointer;
  color: black;
}
.toggle{
  position: relative;
  width: 60px;
  height: 60px;
  background: url('menu.png');
  background-repeat:no-repeat;
  background-size:30px ;
  background-position: center;
  cursor: pointer;
}

.toggle.active{
  background: url('close.png');
  background-repeat: no-repeat;
  background-size: 25px;
  background-position: center;
}

.showcase video{
  position: absolute;
  top: 0;
  left:0;
  width:100%;
  height:100%;
  object-fit: cover;
  opacity:0.8;
}

.overlay{
position:absolute;
top:0;
left:0;
width:100%;
height:100%;
background:mediumspringgreen;
mix-blend-mode: overlay;
}
.text{
  position:relative;
  color: black; 
  text-align:left;
} 

.text h2{
  font-size: 5em;
  font-weight:1em;
  line-height: 1em;
  text-transform: uppercase;
} 

.text h3{
  font-size: 4em;
  font-weight: 700;
  line-height: 1em;
  text-transform: uppercase;
} 

.text p{
  font-size: 1.1em;
  margin:20px 0;
  font-weight: 400;
  max-width: 700px;
} 

.text a{
  display: inline-block;
  font-size: 1em;
  background: floralwhite;
  padding:10px 30px;
  text-decoration:none;
  color: black;
  margin-top: 10px;
  text-transform: uppercase;
  letter-spacing: 2px;
  transition: 0.2s;
} 

.text a:hover{
  letter-spacing: 6px;
} 

.social{
  position: absolute;
  bottom: 20px;
  z-index: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
} 

.social li{
  list-style: none;
}

.social li a{
  display:inline-block;
  filter: invert(1);
  margin-right: 20px;
  transform:scale(0.5);
  transition: 0.5s;
}

.social li a:hover{
  transform: scale(0.5) translateY(-15px);
} 
.menu{
  position: absolute;
  top:0;
  right:0;
  width:300px;
  height:100px;
  display:flex;
  align-items: center;
  justify-content: center;
}
.menu ul{
  position: relative;
  list-style: none;
}

.menu ul li a{
  text-decoration: none;
  font-size: 24px;
  color:black;
}

.menu ul li a:hover{
  color:var(--overlay--color);
}
@media(max-width:991px) {
  .showcase,
  .showcase header{
    padding:40px;
  }

  .text h2{
    font-size: 3em;   
  } 

  .text h3{
    font-size:2
  } 
  
  
  **HTML
  
  
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <title>weight Lossing</title>
</head>
<body>
  <section class="showcase">
    <header>
    <h2 class="logo">HEALTH</h2>
    <div class="toggle"></div>
  </header> 
  
  <video src="fitness.mp4" muted loop autoplay> </video>
   
  <div clss="overlay"></div> 

  <div class="text"> 
    <h2>Never Give Up </h2>
    <h3>Lossing Your Weight</h3>
    <p>The most important component of an effective weight-management program must be the prevention of unwanted weight gain from excess body fat</p>
  <a href="#">Explore</a>
  </div>
<ul class="social">
  <li><a href="#"><img src="facebook.png" alt=""></a></li>
  <li><a href="#"><img src="twitwe.png" alt=""></a></li>
  <li><a href="#"><img src="instagram.png" alt=""></a></li>
</ul>
</section> 

<div class="menu">
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">NEWS</a></li>
    <li><a href="#">DESTINATION</a></li>
    <li><a href="#">BLOG</a></li>
    <li><a href="#">CONTACT</a></li>
  </ul>
</div>
</body>
</html>
