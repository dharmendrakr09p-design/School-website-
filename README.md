# School-website-<!DOCTYPE html>
<html>
<head>
<title>Patna City Central School</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Arial;}

body{
background:#111;
color:white;
scroll-behavior:smooth;
}

/* NAVBAR */
nav{
position:fixed;
width:100%;
display:flex;
justify-content:space-between;
padding:15px 40px;
background:rgba(0,0,0,0.8);
z-index:1000;
}

nav h2{color:gold;}
nav ul{display:flex;list-style:none;}
nav ul li{margin-left:20px;}
nav ul li a{
color:white;
text-decoration:none;
transition:0.3s;
}
nav ul li a:hover{color:gold;}

/* HERO VIDEO */
.hero{
position:relative;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
overflow:hidden;
}

.hero video{
position:absolute;
width:100%;
height:100%;
object-fit:cover;
z-index:-1;
}

.hero h1{
font-size:50px;
color:gold;
animation:glow 2s infinite alternate;
}

@keyframes glow{
from{text-shadow:0 0 10px gold;}
to{text-shadow:0 0 30px red;}
}

.btn{
margin-top:20px;
padding:12px 30px;
background:gold;
border:none;
border-radius:25px;
color:black;
cursor:pointer;
transition:0.3s;
}
.btn:hover{
background:red;
color:white;
transform:scale(1.1);
}

/* SECTION */
section{
padding:80px 20px;
text-align:center;
}

.card{
background:#1a1a1a;
padding:25px;
margin:20px;
border-radius:15px;
display:inline-block;
width:280px;
transition:0.4s;
border:1px solid gold;
}
.card:hover{
transform:translateY(-10px);
box-shadow:0 0 20px gold;
}

/* FORM */
input, select{
width:80%;
padding:10px;
margin:10px;
border-radius:8px;
border:none;
}

/* MAP */
iframe{
width:90%;
height:300px;
border-radius:15px;
margin-top:20px;
}

/* FOOTER */
footer{
background:black;
padding:20px;
text-align:center;
color:gray;
}

@media(max-width:768px){
.hero h1{font-size:30px;}
.card{width:90%;}
}
</style>
</head>

<body>

<nav>
<h2>PCS</h2>
<ul>
<li><a href="#home">Home</a></li>
<li><a href="#about">About</a></li>
<li><a href="#admission">Admission</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>

<div class="hero" id="home">
<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4" type="video/mp4">
</video>

<div>
<h1>Patna City Central School</h1>
<p>Excellence | Discipline | Success</p>
<button class="btn">Admission Open 2026</button>
</div>
</div>

<section id="about">
<h2>About Our School</h2>
<p>Patna City Central School provides modern smart education with advanced facilities and experienced faculty.</p>

<div class="card">
<h3>Smart Classes</h3>
<p>Digital boards & modern learning.</p>
</div>

<div class="card">
<h3>Sports Complex</h3>
<p>Large playground & indoor games.</p>
</div>

<div class="card">
<h3>Library</h3>
<p>Rich academic book collection.</p>
</div>
</section>

<section id="admission">
<h2>Online Admission Form</h2>
<input type="text" placeholder="Student Name"><br>
<input type="text" placeholder="Parent Name"><br>
<select>
<option>Select Class</option>
<option>Nursery</option>
<option>1 to 5</option>
<option>6 to 8</option>
<option>9 to 12</option>
</select><br>
<input type="text" placeholder="Mobile Number"><br>
<button class="btn">Submit Application</button>
</section>

<section id="contact">
<h2>Our Location</h2>
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3918.933386663814!2d77.60741437488542!3d12.97159899088638!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bae1678b6b6b6b7%3A0xabcdef1234567890!2sSchool!5e0!3m2!1sen!2sin!4v1690000000000"></iframe>
</section>

<footer>
© 2026 Patna City Central School | Designed by Aditya
</footer>

</body>
</html>
