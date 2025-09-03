# Ex02 Commercial Website
## Date:03-09-2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Solace Skin — Skincare</title>
  <meta name="description" content="Solace Skin — premium skincare for all skin types." />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg: #fce9d8;
      --card: #ffffff;
      --muted:#6b6b6b;
      --text:#0b0b0b;
      --accent:#c84b7b;
      --accent-2:#ff7fbf;
      --shadow: 0 8px 30px rgba(11,11,11,.06);
      --radius: 14px;
      --maxw: 1200px;
    }
    body{font-family:Inter,system-ui; margin:0; background:var(--bg); color:var(--text);}
    .container{max-width:var(--maxw);margin:0 auto;padding:28px}
    header{padding:18px 0}
    .nav{display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:48px;height:48px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:grid;place-items:center;color:#fff;font-weight:700}
    nav a{margin-left:18px;color:var(--muted);text-decoration:none;font-weight:600}
    .btn{background:var(--accent);color:#fff;padding:8px 14px;border-radius:10px;border:none;font-weight:600;cursor:pointer}

    .hero{text-align:center;margin-top:24px}
    .hero-card{background:#fff3ee;border-radius:18px;padding:36px;box-shadow:var(--shadow);display:inline-block}
    .hero h1{font-size:34px;margin:0 0 8px}

    .section-title{margin:40px 0 20px;font-size:22px;color:var(--accent);font-weight:700}

    .products{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:18px}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:var(--shadow);border:1px solid rgba(11,11,11,.05);text-align:center}
    .product-title{font-weight:700;margin:12px 0 8px}
    .meta-list{margin:0;padding-left:18px;color:var(--muted);font-size:14px;text-align:left}
    .product-image{width:100%;border-radius:12px;object-fit:cover;height:150px}
    footer{margin-top:48px;padding:36px 0;color:var(--muted)}
    .footer-grid{display:flex;justify-content:space-between;flex-wrap:wrap}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo">SS</div>
        <div>
          <div style="font-weight:800">Solace Skin</div>
          <div style="font-size:12px;color:var(--muted)">By Hari Priya</div>
        </div>
      </div>
      <nav>
        <a href="#products">Shop</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
      <button class="btn">Cart</button>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div class="hero-card">
        <h1>Glow like never before</h1>
        <p>Elevate your skin with Solace Skin — skincare tailored for every skin type.</p>
      </div>
    </section>

    <div id="products">
      <!-- Cleansing -->
      <div class="section-title">🧴 Cleansing</div>
      <div class="products">
        <div class="card">
          <img src="images/oilwash.png" alt="Cleanser" class="product-image">
          <div class="product-title">Face Wash - Oily</div>
          <ul class="meta-list"><li>Oil-control / Gel-based</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹299</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/drywash.png" alt="Face Wash - Dry" class="product-image">
          <div class="product-title">Face Wash - Dry</div>
          <ul class="meta-list"><li>Hydrating / Cream-based</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹319</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/comwash.png" alt="Face Wash - Combination" class="product-image">
          <div class="product-title">Face Wash - Combination</div>
          <ul class="meta-list"><li>Gentle foam / Gel-based</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹309</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/cleanser.png" alt="Cleanser" class="product-image">
          <div class="product-title">Cleanser</div>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/water.png" alt="Micellar Water" class="product-image">
          <div class="product-title">Micellar Water</div>
          <div style="margin:8px 0;font-weight:600;">₹449</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
      </div>

      <!-- Hydration & Moisturizing -->
      <div class="section-title">🌸 Hydration & Moisturizing</div>
      <div class="products">
        <div class="card">
          <img src="images/oilymoi.png" alt="Moisturizer - Oily" class="product-image">
          <div class="product-title">Moisturizer - Oily</div>
          <ul class="meta-list"><li>Oil-free gel/cream</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/drymoi.png" alt="Moisturizer - Dry" class="product-image">
          <div class="product-title">Moisturizer - Dry</div>
          <ul class="meta-list"><li>Rich cream/lotion</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹449</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/commoi.png" alt="Moisturizer - Combination" class="product-image">
          <div class="product-title">Moisturizer - Combination</div>
          <ul class="meta-list"><li>Lightweight gel-cream</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹429</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/ncdry.png" alt="Night Cream - Dry" class="product-image">
          <div class="product-title">Night Cream - Dry</div>
          <ul class="meta-list"><li>Deep repairing cream</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹499</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/ncoily.png" alt="Night Cream - Oily/Combo" class="product-image">
          <div class="product-title">Night Cream - Oily</div>
          <ul class="meta-list"><li>Lightweight night gel</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹459</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/face mist.png" alt="Face Mist" class="product-image">
          <div class="product-title">Face Mist / Hydrating Spray</div>
          <div style="margin:8px 0;font-weight:600;">₹349</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/lip balm.png" alt="Lip Balm" class="product-image">
          <div class="product-title">Lip Balm</div>
          <div style="margin:8px 0;font-weight:600;">₹199</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/hand.png" alt="Hand Cream" class="product-image">
          <div class="product-title">Hand Cream</div>
          <div style="margin:8px 0;font-weight:600;">₹299</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/body.png" alt="Body Lotion" class="product-image">
          <div class="product-title">Body Lotion</div>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
      </div>

      <!-- Treatment & Targeted Care -->
      <div class="section-title">🌟 Treatment & Targeted Care</div>
      <div class="products">
        <div class="card">
          <img src="images/oily serum - Copy.png" alt="Face Serum - Oily" class="product-image">
          <div class="product-title">Face Serum - Oily</div>
          <ul class="meta-list"><li>Niacinamide, Salicylic Acid</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹499</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/dry serum.png" alt="Face Serum - Dry" class="product-image">
          <div class="product-title">Face Serum - Dry</div>
          <ul class="meta-list"><li>Hyaluronic Acid, Vitamin E</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹529</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/com serum.png" alt="Face Serum - Combo" class="product-image">
          <div class="product-title">Face Serum - Combination</div>
          <ul class="meta-list"><li>Vitamin C, Hyaluronic + Niacinamide</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹549</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/face oil.png" alt="Face Oil" class="product-image">
          <div class="product-title">Face Oil - Dry </div>
          <div style="margin:8px 0;font-weight:600;">₹599</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/eye cream.png" alt="Eye Cream" class="product-image">
          <div class="product-title">Eye Cream</div>
          <div style="margin:8px 0;font-weight:600;">₹449</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/acne.png" alt="Acne Spot Treatment" class="product-image">
          <div class="product-title">Acne Spot Treatment - Oily</div>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/neck.png" alt="Neck Cream" class="product-image">
          <div class="product-title">Neck Cream</div>
          <div style="margin:8px 0;font-weight:600;">₹449</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
      </div>

      <!-- Masks & Exfoliation -->
      <div class="section-title">🌿 Masks & Exfoliation</div>
      <div class="products">
        <div class="card">
          <img src="images/ex oily.png" alt="Exfoliator - Oily" class="product-image">
          <div class="product-title">Exfoliator / Scrub - Oily</div>
          <ul class="meta-list"><li>Oil-control scrub with salicylic</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹349</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/ex dry.png" alt="Exfoliator - Dry" class="product-image">
          <div class="product-title">Exfoliator / Scrub - Dry</div>
          <ul class="meta-list"><li>Gentle cream-based scrub</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹369</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/ex com.png" alt="Exfoliator - Combo" class="product-image">
          <div class="product-title">Exfoliator / Scrub Combination</div>
          <ul class="meta-list"><li>Mild exfoliating scrub</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹359</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/clay.png" alt="Clay Mask" class="product-image">
          <div class="product-title">Clay Mask / Charcoal Mask - Oily</div>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/sheet.png" alt="Sheet Mask" class="product-image">
          <div class="product-title">Sheet Mask - All Skin Types</div>
          <div style="margin:8px 0;font-weight:600;">₹299</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/sleep.png" alt="Sleeping Mask" class="product-image">
          <div class="product-title">Sleeping Mask - All skin Types</div>
          <div style="margin:8px 0;font-weight:600;">₹499</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/scrub.png" alt="scrub" class="product-image">
          <div class="product-title">Body Scrub</div>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
      </div>

      <!-- Sun & Protection -->
      <div class="section-title">☀️ Sun Protection</div>
      <div class="products">
        <div class="card">
          <img src="images/sun oil.png" alt="Sunscreen - Oily" class="product-image">
          <div class="product-title">Sunscreen - Oily</div>
          <ul class="meta-list"><li>Matte finish, oil-free</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹399</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/sun dry.png" alt="Sunscreen - Dry" class="product-image">
          <div class="product-title">Sunscreen - Dry</div>
          <ul class="meta-list"><li>Hydrating, moisturizing formula</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹429</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
        <div class="card">
          <img src="images/sun com.png" alt="Sunscreen - Combo" class="product-image">
          <div class="product-title">Sunscreen - Combination</div>
          <ul class="meta-list"><li>Lightweight, non-clogging</li></ul>
          <div style="margin:8px 0;font-weight:600;">₹419</div>
          <button class="btn" style="width:100%;">Add to Cart</button>
        </div>
      </div>
    </div>

    <footer>
      <div class="footer-grid">
        <div>
          <div style="font-weight:800">Solace Skin</div>
          <div class="meta">© <span id="year"></span></div>
        </div>
        <div class="meta">Terms • Privacy • Returns</div>
      </div>
    </footer>
  </main>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
```

## OUTPUT
<img width="1888" height="481" alt="image" src="https://github.com/user-attachments/assets/353bf8b0-1039-46cb-b77c-66120e28af34" />
<img width="1861" height="909" alt="image" src="https://github.com/user-attachments/assets/80e45978-eb67-4ed5-b78c-7b3f06b36f64" />
<img width="1871" height="914" alt="image" src="https://github.com/user-attachments/assets/ed63df87-920c-474e-82b7-b77bdd5bc42e" />
<img width="1866" height="912" alt="image" src="https://github.com/user-attachments/assets/464878c5-fac3-43ed-b860-d14e7df3b6d5" />
<img width="1877" height="907" alt="image" src="https://github.com/user-attachments/assets/b1a903ed-b970-4e96-b6e5-2bbb28b9934d" />
<img width="1873" height="724" alt="image" src="https://github.com/user-attachments/assets/569cdd86-e87a-4934-8b07-ccf52aa7b328" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
