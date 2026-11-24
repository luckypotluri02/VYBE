# VYBE
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Saffron & Stone | Modern Indian Kitchen</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet">
<style>
:root {
  --ink: #211b17;
  --cream: #faf5ed;
  --orange: #c65d32;
  --muted: #766b61;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  background: var(--cream);
  color: var(--ink);
  font-family: 'DM Sans', sans-serif;
}

a {
  text-decoration: none;
  color: inherit;
}

.nav {
  height: 76px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 7%;
  background: #fffaf3;
  position: sticky;
  top: 0;
  z-index: 5;
  border-bottom: 1px solid #eadfd2;
}

.brand {
  font: 700 25px 'Playfair Display';
  letter-spacing: -.5px;
}

.brand span {
  color: var(--orange);
}

.links {
  display: flex;
  gap: 28px;
  font-size: 14px;
  color: #51483f;
}

.links a:hover {
  color: var(--orange);
}

.navbtn, .btn {
  background: var(--orange);
  color: white;
  padding: 13px 21px;
  border-radius: 4px;
  font-weight: 700;
  font-size: 13px;
  display: inline-block;
}

.hero {
  min-height: 590px;
  display: grid;
  grid-template-columns: 1.02fr .98fr;
  align-items: center;
  padding: 65px 7%;
  gap: 50px;
  background: linear-gradient(90deg, #faf5ed 0%, #faf5ed 55%, #f2e5d6 55%);
}

.eyebrow {
  color: var(--orange);
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 2px;
  text-transform: uppercase;
}

.hero h1 {
  font: 700 clamp(42px, 5vw, 68px)/1.06 'Playfair Display';
  margin: 17px 0;
}

.hero p {
  color: var(--muted);
  line-height: 1.8;
  max-width: 470px;
}

.hero img {
  width: 100%;
  height: 440px;
  object-fit: cover;
  border-radius: 48% 48% 5px 5px;
  box-shadow: 20px 20px 0 #e5c7a7;
}

.actions {
  display: flex;
  gap: 15px;
  align-items: center;
  margin-top: 28px;
}

.ghost {
  font-size: 13px;
  font-weight: 700;
  border-bottom: 1px solid var(--ink);
  padding: 10px 0;
}

.section {
  padding: 85px 7%;
}

.center {
  text-align: center;
}

.section h2 {
  font: 700 42px 'Playfair Display';
  margin: 10px 0 12px;
}

.sub {
  color: var(--muted);
  line-height: 1.7;
}

.menu {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
  margin-top: 38px;
}

.dish {
  background: white;
  padding: 13px;
  border-radius: 8px;
  box-shadow: 0 8px 30px #35200c0b;
}

.dish img {
  width: 100%;
  height: 205px;
  object-fit: cover;
  border-radius: 5px;
}

.dishrow {
  display: flex;
  justify-content: space-between;
  gap: 10px;
  margin: 15px 3px 4px;
  font-weight: 700;
}

.dish p {
  margin: 5px 3px 12px;
  color: var(--muted);
  font-size: 13px;
}

.price {
  color: var(--orange);
}

.offer {
  background: #2b3025;
  color: #fff;
  padding: 60px 8%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 25px;
}

.offer h2 {
  font: 700 36px 'Playfair Display';
  margin: 8px 0;
}

.offer p {
  color: #d4d6cb;
}

.offer .btn {
  background: #e8a56f;
  color: #211b17;
}

.reviews {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-top: 35px;
}

.review {
  background: #fff;
  padding: 25px;
  border-radius: 7px;
  line-height: 1.7;
  color: #62574e;
}

.review b {
  display: block;
  color: var(--ink);
  margin-top: 15px;
}

.stars {
  color: #d58a39;
  letter-spacing: 3px;
}

.footer {
  background: #1d211b;
  color: #e9e5dc;
  padding: 45px 7%;
  display: flex;
  justify-content: space-between;
  gap: 25px;
  flex-wrap: wrap;
}

.footer p {
  color: #bdb9af;
  font-size: 13px;
}

.footer a {
  color: #e9a16d;
}

@media(max-width: 800px) {
  .links { display: none; }
  .hero { grid-template-columns: 1fr; padding-top: 50px; }
  .hero img { height: 320px; }
  .menu, .reviews { grid-template-columns: 1fr 1fr; }
  .offer { display: block; }
  .section { padding: 65px 6%; }
}

@media(max-width: 520px) {
  .menu, .reviews { grid-template-columns: 1fr; }
  .nav { padding: 0 5%; }
  .hero { padding: 45px 6%; }
  .hero h1 { font-size: 45px; }
  .section h2 { font-size: 34px; }
}
</style>
</head>
<body>

<nav class="nav">
  <a class="brand" href="#">Saffron <span>&</span> Stone</a>
  <div class="links">
    <a href="#story">Our Story</a>
    <a href="#menu">Menu</a>
    <a href="#reviews">Reviews</a>
    <a href="#visit">Visit Us</a>
  </div>
  <a class="navbtn" href="#visit">Book a Table</a>
</nav>

<header class="hero">
  <div>
    <div class="eyebrow">A little spice. A lot of soul.</div>
    <h1>Tradition served with a modern twist.</h1>
    <p>Discover thoughtful Indian cooking, seasonal ingredients and warm hospitality. Your table is waiting.</p>
    <div class="actions">
      <a class="btn" href="#menu">Explore the menu</a>
      <a class="ghost" href="#story">Discover our story ↗</a>
    </div>
  </div>
  <img src="https://images.unsplash.com/photo-1546833999-b9f581a1996d?auto=format&fit=crop&w=1100&q=85" alt="Indian thali meal with colourful dishes">
</header>

<section class="section center" id="story">
  <div class="eyebrow">Made with heart</div>
  <h2>Good food brings us together.</h2>
  <p class="sub">At Saffron & Stone, familiar flavours meet fresh ideas. We source seasonal produce<br>and prepare every plate with care, patience and a generous pinch of joy.</p>
</section>

<section class="section" id="menu" style="background:#f1e8dc">
  <div class="center">
    <div class="eyebrow">From our kitchen</div>
    <h2>Guest favourites</h2>
    <p class="sub">A few delicious reasons to pull up a chair.</p>
  </div>
  <div class="menu">
    <article class="dish">
      <img src="https://images.unsplash.com/photo-1565557623262-b51c2513a641?auto=format&fit=crop&w=800&q=85" alt="Butter chicken curry">
      <div class="dishrow"><span>Smoky Butter Chicken</span><span class="price">₹320</span></div>
      <p>Slow-cooked tomato gravy, cream and house spices.</p>
    </article>
    <article class="dish">
      <img src="https://images.unsplash.com/photo-1589302168068-964664d93dc0?auto=format&fit=crop&w=800&q=85" alt="Biryani served in a bowl">
      <div class="dishrow"><span>Hyderabadi Dum Biryani</span><span class="price">₹280</span></div>
      <p>Fragrant basmati, herbs and a signature dum finish.</p>
    </article>
    <article class="dish">
      <img src="https://images.unsplash.com/photo-1601050690597-df0568f70950?auto=format&fit=crop&w=800&q=85" alt="Indian samosas">
      <div class="dishrow"><span>Golden Samosa Plate</span><span class="price">₹140</span></div>
      <p>Crisp pastry, spiced potato and mint chutney.</p>
    </article>
  </div>
</section>

<section class="offer">
  <div>
    <div class="eyebrow" style="color:#e8a56f">A reason to celebrate</div>
    <h2>Make your next meal memorable.</h2>
    <p>Enjoy a complimentary dessert with any two main courses this week.</p>
  </div>
  <a class="btn" href="#visit">Plan your visit</a>
</section>

<section class="section center" id="reviews">
  <div class="eyebrow">Kind words</div>
  <h2>What guests are saying</h2>
  <div class="reviews">
    <div class="review">
      <div class="stars">★★★★★</div>“Beautiful flavours, generous portions and a lovely atmosphere.”<b>— Ananya R.</b>
    </div>
    <div class="review">
      <div class="stars">★★★★★</div>“The biryani is comforting, aromatic and absolutely worth coming back for.”<b>— Kiran M.</b>
    </div>
    <div class="review">
      <div class="stars">★★★★★</div>“Friendly service and a menu with something for everyone.”<b>— Priya S.</b>
    </div>
  </div>
</section>

<footer class="footer" id="visit">
  <div>
    <div class="brand">Saffron <span>&</span> Stone</div>
    <p>Thoughtful Indian food, made for sharing.</p>
  </div>
  <div>
    <b>Find us</b>
    <p>MG Road, Vijayawada, Andhra Pradesh</p>
    <p>Tue–Sun · 12:00 PM – 10:30 PM</p>
  </div>
  <div>
    <b>Reservations</b>
    <p>+91 98765 43210</p>
    <a href="mailto:hello@saffronstone.example">hello@saffronstone.example</a>
  </div>
</footer>

</body>
</html>
```[cite: 1]
