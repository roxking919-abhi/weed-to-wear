<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Weed to Wear – Eco Fashion from Water Hyacinth</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;900&family=Pacifico&family=Roboto:wght@400;700&family=Fira+Sans:wght@700&family=Source+Serif+4:ital,wght@1,600&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --main-bg: linear-gradient(135deg, #151c1f 0%, #243043 100%);
      --card-bg: rgba(32,42,47,0.97);
      --header-grad: linear-gradient(100deg, #6be177 22%, #243043 80%);
      --accent: #6be177;
      --accent2: #81ffc4;
      --accent3: #42cba2;
      --txt: #f4f6ed;
      --txt-muted: #bdeccb;
    }
    body {
      font-family: 'Open Sans', Arial, sans-serif;
      margin: 0;
      background: linear-gradient(-45deg, #151c1f, #243043, #19464b, #2c5f64);
      background-size: 400% 400%;
      color: var(--txt);
      min-height: 100vh;
      letter-spacing: 0.01em;
      overflow-x: hidden;
      animation: gradientMove 25s ease infinite;
    }
    @keyframes gradientMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    nav {
      background: #11171aeb;
      box-shadow: 0 8px 28px #0e564f17;
      padding: 1.2em 2em 1.05em 2em;
      color: #eaffea;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky; top: 0; z-index: 30;
      font-family: 'Montserrat', Arial, sans-serif;
      backdrop-filter: saturate(180%) blur(10px);
      border-radius: 0 0 20px 20px;
      border-bottom: 1px solid rgba(107, 225, 119, 0.4);
      transition: background-color 0.3s ease;
    }
    nav:hover { background-color: #173726cc; }
    nav div { font-size: 1.25em; letter-spacing: 0.11em; color: #a8f6c4; font-weight: 900; text-shadow: 0 0 8px #4fcb4f88; }
    nav a {
      color: var(--accent);
      margin: 0 1.3em;
      text-decoration: none;
      font-family: 'Quicksand', 'Montserrat', Arial, sans-serif;
      font-size: 1.08em;
      font-weight: 700;
      letter-spacing: 0.05em;
      transition: color 0.18s;
      position: relative;
      z-index: 50;
    }
    nav a:hover { color: var(--accent2); text-shadow: 0 0 12px #9cffc9; }
    header {
      background: var(--header-grad);
      padding: 4em 1em 3.2em 1em;
      text-align: center;
      border-bottom-left-radius: 16% 6vw;
      border-bottom-right-radius: 16% 6vw;
      box-shadow: 0 14px 40px #47d79839;
      position: relative;
      color: #fff;
      overflow: hidden;
    }
    header::before, header::after {
      content: '';
      position: absolute;
      border-radius: 50%;
      filter: blur(124px);
      opacity: 0.5;
      z-index: 1;
      animation-timing-function: linear;
      animation-iteration-count: infinite;
    }
    header::before {
      width: 280px; height: 280px; background: #6be177cc;
      top: -100px; left: -80px;
      animation: moveShape 30s linear infinite;
    }
    header::after {
      width: 400px; height: 400px; background: #1e4f4bcc;
      bottom: -140px; right: -160px;
      animation: moveShapeRev 30s linear infinite;
    }
    @keyframes moveShape {
      0% { transform: translate(0, 0) rotate(0deg); }
      100% { transform: translate(100px, 100px) rotate(360deg); }
    }
    @keyframes moveShapeRev {
      0% { transform: translate(0, 0) rotate(0deg); }
      100% { transform: translate(-80px, -70px) rotate(-360deg); }
    }
    h1, h2 {
      font-family: 'Montserrat', Arial, sans-serif;
      margin-bottom: 0.4em;
      letter-spacing: 0.04em;
      position: relative; z-index: 10;
    }
    h1 {
      font-size: 3em;
      color: #fff;
      font-family: 'Pacifico', cursive, 'Montserrat', Arial, sans-serif;
      text-shadow: 0 4px 18px #6be17733;
      font-weight: 900;
    }
    h2 {
      font-size: 1.8em;
      color: var(--accent2);
      text-shadow: 0 2px 10px #398b5b39;
      font-family: 'Fira Sans', 'Montserrat', Arial, sans-serif;
    }
    section {
      padding: 2.4em 1.5em;
      max-width: 960px;
      margin: 2.4em auto 2.6em auto;
      background: var(--card-bg);
      border-radius: 20px;
      box-shadow: 0 6px 32px #90ffa039;
      color: var(--txt);
      font-size: 1.1em;
      font-family: 'Roboto', Arial, sans-serif;
      line-height: 1.55;
      position: relative;
      overflow: hidden;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2em;
      margin-top: 1.5em;
      position: relative; z-index: 5;
    }
    .product-card {
      background: #1c272aeb;
      padding: 1.8em 1.2em 1.6em 1.2em;
      border-radius: 18px;
      box-shadow: 0 5px 28px #27e1a477;
      text-align: left;
      color: var(--txt);
      font-family: 'Source Serif 4', serif;
      border-left: 6px solid var(--accent2);
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .product-card:hover {
      transform: translateY(-8px) scale(1.04);
      box-shadow: 0 10px 48px #5cdbb29f;
    }
    .product-card h3 {
      color: var(--accent3);
      font-family: 'Fira Sans', 'Montserrat', Arial, sans-serif;
      font-weight: 700;
      letter-spacing: 0.07em;
      margin-bottom: 0.8em;
    }
    .product-card strong {
      color: var(--accent2);
      font-size: 1.22em;
      letter-spacing: 0.02em;
    }
    .button {
      display: inline-block;
      background: linear-gradient(90deg,#39e6b8 55%,#6be177 120%);
      color: #fff;
      padding: 0.95em 1.7em;
      border-radius: 5px;
      font-weight: 700;
      border: none;
      cursor: pointer;
      font-family: 'Quicksand', Arial, sans-serif;
      font-size: 1.05em;
      letter-spacing: 0.06em;
      box-shadow: 0 3px 16px #39e6b844;
      transition: background 0.18s;
      margin-top: 1.5em;
      user-select: none;
      text-align: center;
    }
    .button:hover { background: linear-gradient(90deg,#113b3a 50%,#97f9c4 120%);}
    ul, ol { margin-left: 1.3em; }
    ul li, ol li { margin-bottom: 0.85em; font-weight: 500; }
    .contact-list {
      list-style: none;
      padding-left: 0; margin: 1.4em 0;
      display: flex; flex-direction: column; gap: 0.55em;
      font-family: 'Fira Sans', sans-serif;
      font-size: 1.1em; font-weight: 700; color: var(--accent2);
    }
    .contact-list li {
      padding-left: 1.3em;
      position: relative; user-select: text;
      border-left: 3px solid var(--accent2);
      transition: background-color 0.15s;
    }
    .contact-list li:hover { background-color: rgba(107,225,119,0.15); border-color: #d8ffde;}
    .phone-icon::before { content: "📞"; display:inline-block; margin-right: .7em;}
    .email-icon::before { content: "✉️"; display:inline-block; margin-right: .7em;}
    .address-icon::before { content:"📍"; display:inline-block; margin-right: .7em;}
    form label {font-weight:700;margin-top:0.8em;display:inline-block;color:var(--accent2);font-family:'Fira Sans',sans-serif;}
    input, textarea {
      width:92%; padding:0.9em; margin-bottom:0.7em; border-radius:8px; border:1.8px solid var(--accent3);
      background:#1e292b; color:var(--txt); font-size:1em; font-family:'Roboto',Arial,sans-serif;
      transition: border-color 0.3s; resize: vertical;
    }
    input:focus, textarea:focus { outline: none; border-color: var(--accent2); box-shadow: 0 0 14px var(--accent2);}
    footer {
      background: linear-gradient(90deg,#101513 65%,#26473e 99%);
      color: #d4fde2;
      text-align: center;
      font-size: 1.1em;
      font-family: 'Montserrat', Arial, sans-serif;
      padding: 2em 1em 1.2em 1em;
      letter-spacing: 0.08em;
      border-top-left-radius: 23% 4vw;
      border-top-right-radius: 23% 4vw;
      margin-top: 3em; user-select: none;
    }
    @media (max-width:700px) {
      section { padding: 1.3em 0.7em; }
      header h1 { font-size: 2.1em; }
      .products { grid-template-columns: 1fr; }
      .contact-list { font-size: 1em; }
    }
    @media (max-width:500px) {
      header { padding: 2em 0.4em 1.6em;}
    }
    em { font-family: 'Source Serif 4', serif; color: #a1fac7; font-weight: 600;}
    ::selection { background: var(--accent2); color: #111; }
    .img-section {
      width: 100%;
      max-width: 340px;
      border-radius: 18px;
      box-shadow: 0 6px 36px #3df9b54b;
      display: block;
      margin: 2em auto 1.5em auto;
      object-fit: cover;
    }
  </style>
</head>
<body>
  <nav>
    <div style="font-size:1.13em;letter-spacing:0.08em;">🌿 Weed to Wear</div>
    <div>
      <a href="#about">About</a>
      <a href="#process">How It Works</a>
      <a href="#products">Products</a>
      <a href="#impact">Impact</a>
      <a href="#team">Team</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>
  <header>
    <h1>Turning Weeds into Wear</h1>
    <p style="font-family:'Fira Sans',sans-serif;font-size:1.15em;">
      <span style="font-size:1.2em;color:var(--accent2);font-weight:700;font-family:'Quicksand';">Eco Fashion from Water Hyacinth</span><br>
      Welcome to Weed to Wear, where aquatic weeds become sustainable, stylish products for a better India.<br>
      <em>Clean water. Empowered lives. Inspired design—crafted for you.</em>
    </p>
    <a href="#products" class="button">Shop Now</a>
  </header>
  <section id="about">
    <h2>About Weed to Wear</h2>
    <p>
      Weed to Wear transforms the invasive water hyacinth into elegant, eco-friendly products. Founded in Varanasi, our mission is to clean water, empower artisans, and offer plastic-free, biodegradable fashion rooted in community and nature.
    </p>
  </section>
  <section id="process">
    <h2>How It Works</h2>
    <ol>
      <li><strong>Harvest:</strong> Local teams remove water hyacinth, healing waterways and collecting raw material.</li>
      <li><strong>Fiber & Weave:</strong> Stalks are processed into fiber, spun and woven with cotton using heritage looms.</li>
      <li><strong>Eco Finish & Craft:</strong> Products get safe, antibacterial finishing and are hand-crafted into beautiful, sustainable goods.</li>
    </ol>
  </section>
  <section id="products">
    <h2>Our Products</h2>
    <div class="products">
      <div class="product-card">
        <h3>Eco Tote Bag</h3>
        <p>
          Vibrant, strong, and lightweight—perfect for errands or outings. Hyacinth-cotton blend, plant-dyed, artisan-stitched.
          <br><strong>₹120</strong>
        </p>
        <a href="#" class="button">Buy Now</a>
      </div>
      <div class="product-card">
        <h3>Yoga Mat</h3>
        <p>
          Gentle cushioning, non-slip, antibacterial and UV safe. Lightweight, portable, and chemical-free.
          <br><strong>₹500</strong>
        </p>
        <a href="#" class="button">Buy Now</a>
      </div>
      <div class="product-card">
        <h3>Eco Wallet</h3>
        <p>
          Slim, durable, and compostable. Unique woven design for cards and cash—carry values, not waste.
          <br><strong>₹60</strong>
        </p>
        <a href="#" class="button">Buy Now</a>
      </div>
      <div class="product-card">
        <h3>Carry-All Bag</h3>
        <p>
          Multi-purpose, sturdy, and ventilated—ideal for travel, shopping, or weekend plans.
          <br><strong>₹150</strong>
        </p>
        <a href="#" class="button">Buy Now</a>
      </div>
    </div>
  </section>
  <section id="impact">
    <h2>Impact</h2>
    <ul>
      <li><strong>Clean Rivers:</strong> Removing invasive weeds restores water life and supports local economies.</li>
      <li><strong>No Plastics:</strong> Our products are plastic-free, toxin-free, and fully compostable.</li>
      <li><strong>Empowering Women:</strong> We provide dignified work and skills for rural women artisans.</li>
    </ul>
  </section>
  <section id="team">
    <h2>Meet Our Team</h2>
    <p>
      Weed to Wear is led by school-age changemakers from Varanasi—students passionate about environment, innovation, and social good.
    </p>
    <div>
      <div style="margin-bottom: 1.1em;">
        <strong style="font-family:'Fira Sans',sans-serif;color:var(--accent3);font-size:1.13em;">Abhishek Kumar</strong> – CEO &amp; Founder<br>
        <span style="color:var(--txt-muted);font-family:'Source Serif 4',serif;">
          Abhishek leads strategy and inspires the team, blending studies with real-world action.
        </span>
      </div>
      <div style="margin-bottom: 1.1em;">
        <strong style="font-family:'Fira Sans',sans-serif;color:var(--accent3);font-size:1.13em;">Sumit Makharia</strong> – Chief Financial Officer (CFO)<br>
        <span style="color:var(--txt-muted);font-family:'Source Serif 4',serif;">
          Sumit manages finances and ensures every rupee is spent for impact.
        </span>
      </div>
      <div style="margin-bottom: 1.1em;">
        <strong style="font-family:'Fira Sans',sans-serif;color:var(--accent3);font-size:1.13em;">Pratham Tiwari</strong> – Chief Marketing Officer (CMO)<br>
        <span style="color:var(--txt-muted);font-family:'Source Serif 4',serif;">
          Pratham spreads the Weed to Wear story across schools and social media.
        </span>
      </div>
      <div style="margin-bottom: 1.1em;">
        <strong style="font-family:'Fira Sans',sans-serif;color:var(--accent3);font-size:1.13em;">Shubham Sinha</strong> – Chief Information Officer (CIO)<br>
        <span style="color:var(--txt-muted);font-family:'Source Serif 4',serif;">
          Shubham builds our digital presence and brings tech to our eco-journey.
        </span>
      </div>
    </div>
    <p style="margin-top:2em;">
      <span style="font-family:'Quicksand';color:var(--accent);font-size:1.08em;">
        Young minds, real impact—proving anyone can drive change for India's waters and rural future!
      </span>
    </p>
  </section>
  <section id="contact">
    <h2>Contact Us</h2>
    <p>
      Want to join our cause or partner with Weed to Wear? Reach out—we respond fast!
    </p>
    <ul class="contact-list">
      <li class="email-icon"><span style="color:#ffffff;font-family:'Fira Sans','Montserrat',sans-serif;">weedtowearvns123@gmail.com</span></li>
      <li class="phone-icon">8521229737</li>
      <li class="address-icon"><span style="color:var(--accent2);">Varanasi, Uttar Pradesh</span></li>
    </ul>
    <form>
      <label>Name:<br><input type="text" name="name"></label><br>
      <label>Email:<br><input type="email" name="email"></label><br>
      <label>Message:<br><textarea name="message"></textarea></label><br>
      <button type="submit" class="button">Send</button>
    </form>
  </section>
  <footer>
    &copy; 2025 Weed to Wear. Crafted with care for people and planet.
  </footer>
</body>
</html>
