<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Book With NaJah B</title>  
  
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Poppins:wght@300;500;600&display=swap" rel="stylesheet">  
  
<style>  
body{  
margin:0;  
font-family:Poppins;  
background:#fbf3ef;  
color:#4b2f2f;  
}  
  
header{  
padding:70px 20px;  
text-align:center;  
background:linear-gradient(135deg,#ffd1dc,#f3d6c6,#e7c9b8);  
}  
  
header h1{  
font-family:Playfair Display;  
font-size:50px;  
margin:0;  
}  
  
.section{  
padding:40px 20px;  
max-width:1000px;  
margin:auto;  
}  
  
.card{  
background:white;  
padding:20px;  
border-radius:18px;  
margin-bottom:20px;  
box-shadow:0 8px 20px rgba(0,0,0,0.08);  
}  
  
select,input{  
width:100%;  
padding:10px;  
margin-top:10px;  
border-radius:10px;  
border:1px solid #e6c7b8;  
}  
  
.price{  
font-weight:bold;  
color:#d45c7a;  
margin-top:10px;  
}  
  
.deposit{  
background:#ff5c9a;  
color:white;  
padding:15px;  
display:block;  
text-align:center;  
border-radius:15px;  
margin-top:15px;  
text-decoration:none;  
}  
  
</style>  
</head>  
  
<body>  
  
<header>  
<h1>Book With NaJah B 💕</h1>  
</header>  
  
<!-- SERVICES -->  
<section class="section">  
  
<h2>Services</h2>  
  
<div class="card">  
<h3>Silk Press</h3>  
<p>$55 </p>  
</div>  
  
<div class="card">  
<h3>Quick Weave</h3>  
  
<select id="quickWeave" onchange="calc()">  
<option value="65">Quick Weave - $65+</option>  
<option value="75">Quick Weave + Braids - $75+</option>  
</select>  
  
<label>  
<input type="checkbox" id="quickDesign"> Add Designs (+$5)  
</label>  
  
<p class="price" id="quickPrice">Price: $65</p>  
</div>  
  
</section>  
  
<!-- BRAIDS -->  
<section class="section">  
  
<div class="card">  
<h3>Knotless Braids</h3>  
  
<select id="knotless">  
<option value="65">Large - $65</option>  
<option value="75">Medium - $75</option>  
<option value="85">Small - $85</option>  
</select>  
  
<label><input type="checkbox" id="knotlessLen"> Add Length (+$5)</label>  
  
<p class="price" id="knotlessPrice">Price: $65</p>  
</div>  
  
<div class="card">  
<h3>Boho Braids</h3>  
  
<select id="boho">  
<option value="75">Large - $75</option>  
<option value="85">Medium - $85</option>  
<option value="95">Small - $95</option>  
</select>  
  
<label><input type="checkbox" id="bohoLen"> Add Length (+$5)</label>  
  
<p class="price" id="bohoPrice">Price: $75</p>  
</div>  
  
</section>  
  
<!-- BOOKING FORM -->  
<section class="section">  
  
<h2>Book Your Appointment</h2>  
  
<div class="card">  
  
<input type="text" id="name" placeholder="Full Name">  
<input type="text" id="phone" placeholder="Phone Number">  
  
<label>Select Date</label>  
<input type="date" id="date">  
  
<h3>Upload Inspiration</h3>  
<input type="file">  
  
<a class="deposit" href="https://cash.app/$najahb" onclick="sendInfo()">  
Pay $10 Deposit  
</a>  
  
</div>  
  
</section>  
  
<script>  
  
function calc(){  
  
// quick weave  
let q = parseInt(document.getElementById("quickWeave").value);  
if(document.getElementById("quickDesign").checked) q += 5;  
document.getElementById("quickPrice").innerText = "Price: $" + q;  
  
// knotless  
let k = parseInt(document.getElementById("knotless").value);  
if(document.getElementById("knotlessLen").checked) k += 5;  
document.getElementById("knotlessPrice").innerText = "Price: $" + k;  
  
// boho  
let b = parseInt(document.getElementById("boho").value);  
if(document.getElementById("bohoLen").checked) b += 5;  
document.getElementById("bohoPrice").innerText = "Price: $" + b;  
}  
  
function sendInfo(){  
  
let name = document.getElementById("name").value;  
let phone = document.getElementById("phone").value;  
let date = document.getElementById("date").value;  
  
if(!name || !phone || !date){  
alert("Please fill out name, phone, and date before paying deposit.");  
}  
}  
  
document.querySelectorAll("select, input").forEach(e=>{  
e.addEventListener("change", calc);  
});  
  
</script>  
  
</body>  
</html>  
  
<a class="deposit" href="confirm.html" onclick="saveBooking()">  
After $10 Deposit  
</a>  
  
<script>  
function saveBooking(){  
  
let booking = {  
name: document.getElementById("name").value,  
phone: document.getElementById("phone").value,  
date: document.getElementById("date").value  
};  
  
if(!booking.name || !booking.phone || !booking.date){  
alert("Fill out name, phone, and date first.");  
return event.preventDefault();  
}  
  
localStorage.setItem("booking", JSON.stringify(booking));  
  
}  
</script>  
  
<!DOCTYPE html>  
<html>  
<head>  
<title>Confirm Booking</title>  
  
<link href="[https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;600&display=swap](https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;600&display=swap)" rel="stylesheet">  
  
<style>  
body{  
margin:0;  
font-family:Poppins;  
background:#fbf3ef;  
text-align:center;  
padding:50px;  
}  
  
.card{  
background:white;  
padding:25px;  
border-radius:20px;  
max-width:500px;  
margin:auto;  
box-shadow:0 8px 20px rgba(0,0,0,0.1);  
}  
  
button{  
background:#ff5c9a;  
color:white;  
padding:15px 25px;  
border:none;  
border-radius:15px;  
margin-top:20px;  
cursor:pointer;  
}  
  
</style>  
</head>  
  
<body>  
  
<div class="card">  
  
<h2>Confirm Your Booking 💕</h2>  
  
<p id="info"></p>  
  
<p>  
After paying your $10 deposit on Cash App <b>$najahb</b>,  
click confirm below.  
</p>  
  
</div>  
  
<script>  
  
let data = JSON.parse(localStorage.getItem("booking"));  
  
document.getElementById("info").innerHTML =  
"Name: " + data.name + "<br>" +  
"Phone: " + data.phone + "<br>" +  
"Date: " + data.date;  
  
function confirmBooking(){  
localStorage.setItem("status", "confirmed");  
alert("Booking confirmed! You will be contacted soon.");  
window.location.href = "index.html";  
}  
  
</script>  
  
</body>  
</html> <p>  
Send $10 deposit to:  
<br>  
<a href="https://cash.app/$NaJahBurgess" target="_blank">  
https://cash.app/$NaJahBurgess  
</a>  
</p>  
  
<button onclick="confirmBooking()">  
I Sent Deposit — Confirm Booking  
</button>  
