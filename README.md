
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>WhaleTracker</title>
<style>
*{box-sizing:border-box}
body{
margin:0;
font-family:Arial,sans-serif;
background:#080d18;
color:white;
}
header{
padding:22px;
background:#101a2c;
border-bottom:1px solid #26344b;
}
.logo{font-size:26px;font-weight:bold;color:#31d6b0}
nav{margin-top:15px;color:#aab8ca}
main{padding:20px;max-width:1000px;margin:auto}
h1{font-size:25px}
.subtitle{color:#9ba9bd}
.cards{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:12px;
margin-top:25px;
}
.card{
background:#121e30;
padding:18px;
border:1px solid #263951;
border-radius:12px;
}
.card small{color:#9ba9bd}
.card h2{color:#31d6b0}
input{
width:100%;
padding:14px;
margin:12px 0;
border-radius:8px;
border:1px solid #34445c;
background:#121e30;
color:white;
}
button{
background:#20b99a;
border:0;
padding:13px 20px;
border-radius:8px;
font-weight:bold;
cursor:pointer;
}
table{
width:100%;
margin-top:20px;
border-collapse:collapse;
background:#121e30;
}
th,td{
padding:14px 8px;
border-bottom:1px solid #263951;
text-align:center;
font-size:13px;
}
th{color:#31d6b0}
footer{
text-align:center;
padding:30px;
color:#8391a5;
}
@media(max-width:500px){
.cards{grid-template-columns:1fr}
}
</style>
</head>
<body>

<header>
<div class="logo">🐋 WhaleTracker</div>
<nav>خانه | ردیابی نهنگ‌ها | سولانا | درباره ما</nav>
</header>

<main>
<h1>ردیابی هوشمند نهنگ‌های کریپتو</h1>
<p class="subtitle">
فعالیت کیف پول‌های بزرگ و تراکنش‌های بازار را دنبال کنید.
</p>

<div class="cards">
<div class="card">
<small>شبکه فعال</small>
<h2>Solana</h2>
</div>
<div class="card">
<small>وضعیت سایت</small>
<h2>Online</h2>
</div>
<div class="card">
<small>تراکنش‌های بزرگ</small>
<h2>---</h2>
</div>
<div class="card">
<small>کیف پول‌های ردیابی‌شده</small>
<h2>---</h2>
</div>
</div>

<h2>جست‌وجوی کیف پول</h2>
<p class="subtitle">آدرس کیف پول سولانا را وارد کنید.</p>

<input id="wallet" placeholder="آدرس کیف پول Solana">

<button onclick="searchWallet()">جست‌وجو</button>

<p id="result" class="subtitle"></p>

<h2>آخرین تراکنش‌های نهنگ‌ها</h2>

<table>
<tr>
<th>شبکه</th>
<th>نوع تراکنش</th>
<th>مقدار</th>
</tr>
<tr>
<td>Solana</td>
<td>---</td>
<td>---</td>
</tr>
</table>

</main>

<footer>
WhaleTracker © 2026
<br><br>
Tracking the Giants of Crypto
</footer>

<script>
function searchWallet(){
let wallet=document.getElementById("wallet").value.trim();
let result=document.getElementById("result");

if(wallet.length===0){
result.innerText="لطفاً آدرس کیف پول را وارد کنید.";
return;
}

result.innerText="آدرس وارد شد. اتصال به سیستم ردیابی در مرحله بعد اضافه می‌شود.";
}
</script>

</body>
</html>
