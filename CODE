<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SmartFix Hub | Book Trusted Repairs</title>
  <style>
    body{margin:0;font-family:Arial,Helvetica,sans-serif;background:#0e0e1a;color:#fff}
    header{padding:20px 40px;background:#111122;display:flex;justify-content:space-between;align-items:center}
    header h1{color:#f5b942;margin:0}
    nav a{color:#fff;margin-left:20px;text-decoration:none;font-weight:600}
    .hero{padding:80px 20px;text-align:center;background:linear-gradient(135deg,#1f4068,#162447)}
    .hero h2{font-size:2.5rem;margin-bottom:10px}
    .hero p{max-width:700px;margin:auto;font-size:1.1rem}
    section{padding:60px 20px;max-width:1100px;margin:auto}
    h3.section-title{text-align:center;color:#f5b942;font-size:2rem;margin-bottom:30px}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:25px}
    .card{background:#1b1b2f;padding:20px;border-radius:10px}
    .card h4{color:#f5b942}
    .booking{background:#111122;padding:30px;border-radius:12px}
    label{display:block;margin-top:15px}
    select,input{width:100%;padding:10px;margin-top:5px;border-radius:6px;border:none}
    button{margin-top:20px;padding:12px 20px;background:#f5b942;border:none;border-radius:6px;font-size:1rem;font-weight:bold;cursor:pointer}
    button:hover{opacity:.9}
    .result{margin-top:20px;background:#1b1b2f;padding:15px;border-radius:8px;display:none}
    footer{background:#0b0b14;padding:30px;text-align:center;font-size:.9rem}
  </style>
</head>
<body>

<header>
  <h1>SmartFix Hub</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#book">Book Repair</a>
    <a href="#how">How It Works</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero">
  <h2>Trusted Electronics Repair, Made Simple</h2>
  <p>Find verified technicians, see repair cost before booking, and get your device repaired at home.</p>
</div>

<section>
  <h3 class="section-title">Why SmartFix Hub?</h3>
  <div class="grid">
    <div class="card"><h4>Verified Technicians</h4><p>Only background-checked and rated repair experts.</p></div>
    <div class="card"><h4>Transparent Pricing</h4><p>Know the estimated cost before repair starts.</p></div>
    <div class="card"><h4>Repair Warranty</h4><p>7–30 days warranty on all repairs.</p></div>
  </div>
</section>

<section id="book">
  <h3 class="section-title">Book a Repair</h3>
  <div class="booking">
    <label>Select Device</label>
    <select id="device">
      <option>Phone</option>
      <option>Laptop</option>
      <option>TV</option>
      <option>Fan</option>
    </select>

    <label>Select Problem</label>
    <select id="problem">
      <option>Not Working</option>
      <option>Screen Broken</option>
      <option>Noise Issue</option>
      <option>No Display</option>
    </select>

    <label>Your City</label>
    <input type="text" id="city" placeholder="Enter your city" />

    <button onclick="estimateRepair()">Get Price & Technician</button>

    <div class="result" id="result"></div>
  </div>
</section>

<section id="how">
  <h3 class="section-title">How It Works</h3>
  <div class="grid">
    <div class="card"><h4>1. Choose Item</h4><p>Select the device you want to repair.</p></div>
    <div class="card"><h4>2. Select Problem</h4><p>Tell us what's wrong.</p></div>
    <div class="card"><h4>3. See Price</h4><p>Get an estimated repair cost.</p></div>
    <div class="card"><h4>4. Get Repaired</h4><p>Home repair or pickup & drop.</p></div>
  </div>
</section>

<footer id="contact">
  <p><strong>SmartFix Hub</strong></p>
  <p>Team Jupiter | IT–Twinning | NIET | IMPERIA Tech Fest</p>
  <p>Before buying new, give repair one chance.</p>
</footer>

<script>
  function estimateRepair(){
    const device=document.getElementById('device').value;
    const problem=document.getElementById('problem').value;
    const city=document.getElementById('city').value;

    if(city.trim()===''){alert('Please enter your city');return}

    let price=0;
    if(device==='Phone') price=1200;
    if(device==='Laptop') price=2000;
    if(device==='TV') price=1800;
    if(device==='Fan') price=600;

    const tech=['Ravi Kumar','Aman Singh','Suresh Verma'];
    const assignedTech=tech[Math.floor(Math.random()*tech.length)];

    const result=document.getElementById('result');
    result.style.display='block';
    result.innerHTML=`
      <h4>Repair Details</h4>
      <p><strong>Device:</strong> ${device}</p>
      <p><strong>Problem:</strong> ${problem}</p>
      <p><strong>Estimated Cost:</strong> ₹${price}</p>
      <p><strong>Technician:</strong> ${assignedTech} (Verified)</p>
      <p><strong>Service:</strong> Home repair / Pickup & Drop</p>
      <p><strong>Warranty:</strong> 7–30 Days</p>
    `;
  }
</script>

</body>
</html>
