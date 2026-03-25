89จิตวิทยา
index. html. 
git/
/* style.css */
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0f172a;
  color: white;
  transition: 0.3s;
}

.light {
  background: #f1f5f9;
  color: black;
}

header {
  text-align: center;
  padding: 80px 20px;
  background: linear-gradient(135deg,#1e293b,#020617);
}

h1 {
  font-size: 40px;
}

.section {
  max-width: 900px;
  margin: auto;
  padding: 40px 20px;
}

.card {
  background: #1e293b;
  padding: 20px;
  margin: 20px 0;
  border-radius: 12px;
  cursor: pointer;
  transition: 0.3s;
}

.card:hover {
  transform: scale(1.05);
}

.btn {
  display: inline-block;
  padding: 12px 20px;
  background: #38bdf8;
  color: black;
  border-radius: 8px;
  text-decoration: none;
  margin: 10px 5px;
}

.social a {
  display: inline-block;
  margin: 5px 10px;
  color: #38bdf8;
  text-decoration: none;
  font-weight: bold;
}

textarea {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
}// script.js

function toggleMode() {
  document.body.classList.toggle("light");
}

function showPage(page) {
  const pages = ["home", "chapters", "c1", "c2"];
  pages.forEach(p => {
    const el = document.getElementById(p);
    if(el) el.style.display = "none";
  });
  const target = document.getElementById(page);
  if(target) target.style.display = "block";
}<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<title>89sam1book</title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<header>
<h1>89sam1book</h1>
<p>เข้าใจตัวเองในแบบที่คุณไม่เคยรู้มาก่อน</p>
<button onclick="toggleMode()">🌙 Dark Mode</button>
<a class="btn" onclick="showPage('chapters')">📖 เริ่มอ่าน</a>
</header>

<!-- HOME -->
<div id="home" class="section">
<h2>🧠 Psychebook คืออะไร</h2>
<p>หนังสือจิตวิทยาที่ช่วยให้คุณเข้าใจความคิด อารมณ์ และตัวตนของตัวเอง</p>

<h3>🔥 Highlights</h3>
<ul>
<li>เข้าใจตัวเองลึกขึ้น</li>
<li>จัดการอารมณ์ได้</li>
<li>อ่านง่าย ใช้ได้จริง</li>
</ul>
</div>

<!-- CHAPTERS -->
<div id="chapters" class="section" style="display:none">
<h2>📖 Chapters</h2>

<div class="card" onclick="showPage('c1')">
<h3>Chapter 1</h3>
<p>ทำไมเราคิดมาก</p>
</div>

<div class="card" onclick="showPage('c2')">
<h3>Chapter 2</h3>
<p>วงจรของอารมณ์</p>
</div>

<h3>🎬 วิดีโอแนะนำ</h3>
<iframe width="100%" height="200" src="https://www.youtube.com/embed/4WXs3sKu41I" frameborder="0" allowfullscreen></iframe>
</div>

<!-- CHAPTER 1 -->
<div id="c1" class="section" style="display:none">
<h2>ทำไมเราคิดมาก</h2>
<p>คุณไม่ได้คิดมากเกินไป แต่คุณ “หยุดคิดไม่ได้”</p>

<h3>🧠 คำถาม</h3>
<p>คุณคิดเรื่องอะไรซ้ำ ๆ ?</p>
<textarea placeholder="พิมพ์ reflection ของคุณ..."></textarea>

<button onclick="showPage('chapters')">← กลับ</button>
</div>

<!-- CHAPTER 2 -->
<div id="c2" class="section" style="display:none">
<h2>วงจรของอารมณ์</h2>
<p>อารมณ์มาแล้วก็ไป แต่การตอบสนองคือสิ่งสำคัญ</p>

<h3>🧠 คำถาม</h3>
<p>คุณตอบสนองอารมณ์ยังไง?</p>
<textarea placeholder="พิมพ์ reflection ของคุณ..."></textarea>

<button onclick="showPage('chapters')">← กลับ</button>
</div>

<!-- ABOUT -->
<div class="section">
<h2>👤 About</h2>
<p>ผมสร้าง Psychebook เพื่อช่วยให้คนเข้าใจตัวเองและใช้ชีวิตได้ดีขึ้น</p>
</div>

<!-- CTA + Email -->
<div class="section">
<h2>🚀 สมัคร / ดาวน์โหลด / ติดตาม</h2>
<form action="https://formspree.io/f/your-id" method="POST">
<input type="email" name="email" placeholder="ใส่อีเมล">
<button type="submit">สมัคร</button>
</form>
</div>

<!-- SOCIAL -->
<div class="section">
<h2>🌍 ติดตามเรา</h2>
<div class="social">
<a href="https://www.linkedin.com/in/sam-phongphaew-ab2111347" target="_blank">LinkedIn</a>
<a href="https://www.youtube.com/@Ebook1book" target="_blank">YouTube</a>
<a href="https://www.facebook.com/" target="_blank">Facebook</a>
<a href="https://www.instagram.com/" target="_blank">Instagram</a>
<a href="https://www.tiktok.com/" target="_blank">TikTok</a>
<a href="https://wa.me/" target="_blank">WhatsApp</a>
<a href="https://www.twitter.com/" target="_blank">Twitter</a>
</div>

<h3 style="margin-top:30px;">📖 เว็บไซต์หลัก</h3>
<p style="text-align:center;">
<a href="https://tawatchai999.github.io/89sam1book" target="_blank">👉 เข้าอ่าน Psychebook</a>
</p>
</div>

<script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>89 LAWS Official | Sam Tawatchai Phongphaew</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>89 LAWS OF SUCCESS</h1>
        <p>กฎแห่งความสำเร็จ ความมั่งคั่ง และการตื่นรู้ โดย ธวัชชัย ผ่องแผ้ว</p>
        <div class="header-btns">
            <button class="btn-mode" onclick="toggleMode()">🌙 โหมดกลางคืน/สว่าง</button>
            <a href="#collection" class="btn">📖 คอลเลกชัน</a>
            <a href="#shop" class="btn">🛒 สั่งซื้อ</a>
        </div>
    </header>

    <section id="collection" class="section">
        <h2 class="section-title">📚 The Complete 89 LAWS Series</h2>
        <div class="book-grid">
            <div class="book-item"><img src="e8aac390-26fe-11f1-9f1d-1195122641c3 (1).png" alt="เล่ม 1"><h4>เล่ม 1: จิตวิทยาสร้างเงิน</h4></div>
            <div class="book-item"><img src="copilot_image_1773642215633.jpeg" alt="เล่ม 2"><h4>เล่ม 2: กฎแห่งการศึกษา</h4></div>
            <div class="book-item"><img src="copilot_image_1773642469260.jpeg" alt="เล่ม 3"><h4>เล่ม 3: กฎแห่งความคิด</h4></div>
            <div class="book-item"><img src="copilot_image_1773642778304.jpeg" alt="เล่ม 4"><h4>เล่ม 4: กฎแห่งอำนาจ</h4></div>
            <div class="book-item"><img src="image_1773642262390.jpeg" alt="เล่ม 5"><h4>เล่ม 5: กฎแห่งความมั่งคั่ง</h4></div>
            <div class="book-item"><img src="copilot_image_1773642172678.jpeg" alt="เล่ม 6"><h4>เล่ม 6: ความยิ่งใหญ่ของชีวิต</h4></div>
        </div>
    </section>

    <section class="section">
        <h2 class="section-title">🎥 เจาะลึกบทเรียนจาก 89 LAWS</h2>
        <div class="video-grid">
            <div class="video-card card">
                <div class="video-wrapper"><iframe src="https://www.youtube.com/embed/c60LXavAHAI" allowfullscreen></iframe></div>
                <h4>ทำไมเราถึงคิดมาก?</h4>
            </div>
            <div class="video-card card">
                <div class="video-wrapper"><iframe src="https://www.youtube.com/embed/Nj1qQg1JQyI" allowfullscreen></iframe></div>
                <h4>กฎแห่งความสำเร็จ</h4>
            </div>
            <div class="video-card card">
                <div class="video-wrapper"><iframe src="https://www.youtube.com/embed/oqd_QUlarXM" allowfullscreen></iframe></div>
                <h4>พลังแห่งการตื่นรู้</h4>
            </div>
        </div>
    </section>

    <section class="section">
        <h2 class="section-title">🌍 มาตรฐานความสำเร็จระดับสากล</h2>
        <div class="stats-container">
            <div class="stat-card card">
                <span class="stat-number">10M+</span>
                <p>ยอดขายรวมทั่วโลก</p>
            </div>
            <div class="stat-card card">
                <span class="stat-number">55+</span>
                <p>ภาษาที่ได้รับการแปล</p>
            </div>
        </div>
        <div class="grid-2-col">
            <div class="category-block card">
                <h3 class="cat-title">🌍 Global Bestsellers</h3>
                <p><strong>Surrounded by Idiots:</strong> 1.5M+ sold worldwide</p>
                <p><strong>The Magic of Thinking Big:</strong> Mindset Classic</p>
            </div>
            <div class="category-block card">
                <h3 class="cat-title">🇹🇭 Recommended in Thailand</h3>
                <p><strong>12 Rules for Life:</strong> Life Principles</p>
                <p><strong>Never Split the Difference:</strong> Negotiation</p>
            </div>
        </div>
    </section>

    <section id="shop" class="section">
        <h2 class="section-title">🛒 สั่งซื้อหนังสือ</h2>
        <div class="card promo-card">
            <span class="badge">PROMO</span>
            <h3>89 LAWS Complete Set (6 เล่ม)</h3>
            <p class="price-big">5,900 บาท</p>
            <button class="btn" onclick="addToCart('bundle_set')">🛒 สั่งซื้อครบชุด</button>
        </div>
        <div class="cart-section card">
            <h3>🧺 ตะกร้าสินค้า: <span id="total-price">0</span> บาท</h3>
            <div id="cart-list"></div>
            <a href="https://www.paypal.com/paypalme/TAWATCHAIPHONGPHAEW" target="_blank" class="btn payment-btn">💳 ชำระเงินผ่าน PayPal</a>
        </div>
    </section>

    <footer class="section">
        <div class="card policy-card" style="text-align: center;">
            <p>© 2026 89sam1book สงวนสิทธิ์โดย <strong>ธวัชชัย ผ่องแผ้ว</strong></p>
            <p style="font-size: 0.8rem; opacity: 0.7;">ห้ามคัดลอก ทำซ้ำ หรือเผยแพร่โดยไม่ได้รับอนุญาต</p>
        </div>
    </footer>

    <script src="script.js"></script>
    
    
</html>
:root {
    --bg: #0f172a; --card: #1e293b; --text: #f1f5f9; --primary: #fbbf24;
}
body { margin: 0; font-family: 'Inter', sans-serif; background: var(--bg); color: var(--text); line-height: 1.6; }
body.light { --bg: #f8fafc; --card: #ffffff; --text: #1e293b; }

header { text-align: center; padding: 60px 20px; border-bottom: 2px solid var(--primary); }
.section { max-width: 1000px; margin: 0 auto; padding: 40px 20px; }
.section-title { text-align: center; color: var(--primary); margin-bottom: 30px; }
.card { background: var(--card); padding: 20px; border-radius: 12px; margin-bottom: 20px; border: 1px solid rgba(251,191,36,0.1); }

/* Grids */
.book-grid, .video-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
.book-item img { width: 100%; border-radius: 8px; border: 1px solid var(--primary); transition: 0.3s; }
.book-item:hover img { transform: scale(1.05); }

/* Video */
.video-wrapper { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px; }
.video-wrapper iframe { position: absolute; top:0; left:0; width:100%; height:100%; border:none; }

/* Stats & Shop */
.stats-container { display: flex; gap: 20px; margin-bottom: 20px; }
.stat-number { font-size: 2.5rem; font-weight: 800; color: var(--primary); display: block; }
.btn { background: var(--primary); color: #000; padding: 10px 25px; border-radius: 50px; font-weight: bold; border: none; cursor: pointer; text-decoration: none; display: inline-block; }
.price-big { font-size: 3rem; color: var(--primary); font-weight: 800; }
.payment-btn { width: 100%; text-align: center; margin-top: 15px; }

@media (max-width: 768px) { .stats-container, .grid-2-col { flex-direction: column; display: block; } }
const products = {
    bundle_set: { name: "89 LAWS Complete Set (6 เล่ม)", price: 5900 }
};

let cart = JSON.parse(localStorage.getItem('cartData')) || [];

function toggleMode() { document.body.classList.toggle("light"); }

function addToCart(id) {
    const item = products[id];
    const index = cart.findIndex(c => c.id === id);
    if (index > -1) cart[index].qty++;
    else cart.push({ ...item, id: id, qty: 1 });
    save();
}

function render() {
    const list = document.getElementById('cart-list');
    const total = document.getElementById('total-price');
    if(!list) return;
    list.innerHTML = '';
    let sum = 0;
    cart.forEach(i => {
        sum += i.price * i.qty;
        list.innerHTML += `<p>${i.name} x${i.qty} - ${(i.price*i.qty).toLocaleString()}.-</p>`;
    });
    total.innerText = sum.toLocaleString();
}

function save() {
    localStorage.setItem('cartData', JSON.stringify(cart));
    render();
}

render();


<!---
Tawatchai999/Tawatchai999 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at youoid-tr
anssion&sca_esv=db94c4351747130410624&ei=KhgjaODsJbnf2roP6cuq8QI&oq=www.github%2Fthawatchai999
#my life  teke.  
https: GitHub/thawatchaii999
