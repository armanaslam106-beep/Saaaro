<!DOCTYPE html>
<html lang="ur">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy 20th Birthday Sarah! 🎉🎂</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c 0%, #ff7eb3 100%);
      overflow: hidden;
      position: relative;
    }

    /* Floating Balloons & Hearts */
    .bg-element {
      position: absolute;
      animation: float 6s infinite linear;
      z-index: 1;
      pointer-events: none;
    }

    @keyframes float {
      0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
      100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
    }

    /* Main Container */
    .container {
      width: 90%;
      max-width: 420px;
      min-height: 520px;
      background: rgba(255, 255, 255, 0.92);
      border-radius: 25px;
      padding: 30px 25px;
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
      text-align: center;
      position: relative;
      z-index: 10;
      backdrop-filter: blur(8px);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    /* Page Styles */
    .page {
      display: none;
      animation: fadeIn 0.6s ease-in-out forwards;
    }

    .page.active {
      display: block;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(15px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .icon-box {
      font-size: 65px;
      margin-bottom: 15px;
      animation: bounce 2s infinite;
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    h1 {
      color: #d63384;
      font-size: 26px;
      margin-bottom: 12px;
      font-weight: 700;
    }

    h2 {
      color: #6f42c1;
      font-size: 20px;
      margin-bottom: 15px;
    }

    p {
      color: #495057;
      font-size: 16px;
      line-height: 1.6;
      margin-bottom: 15px;
    }

    .highlight {
      color: #e63946;
      font-weight: bold;
    }

    /* Page Navigation Dots & Buttons */
    .nav-container {
      margin-top: 20px;
    }

    .dots {
      display: flex;
      justify-content: center;
      gap: 8px;
      margin-bottom: 15px;
    }

    .dot {
      width: 10px;
      height: 10px;
      background-color: #ccc;
      border-radius: 50%;
      transition: 0.3s;
    }

    .dot.active {
      background-color: #d63384;
      width: 22px;
      border-radius: 10px;
    }

    .btn-group {
      display: flex;
      justify-content: space-between;
      gap: 10px;
    }

    button {
      padding: 12px 20px;
      border: none;
      border-radius: 25px;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s ease;
      flex: 1;
    }

    .next-btn {
      background: linear-gradient(45deg, #d63384, #fd7e14);
      color: white;
      box-shadow: 0 4px 12px rgba(214, 51, 132, 0.3);
    }

    .next-btn:hover {
      transform: scale(1.03);
    }

    .prev-btn {
      background-color: #e9ecef;
      color: #495057;
    }

    .hidden {
      visibility: hidden;
    }
  </style>
</head>
<body>

  <!-- Floating Elements Container -->
  <div id="bg-container"></div>

  <div class="container">
    <div>
      <!-- PAGE 1: Intro / Grand Welcome -->
      <div class="page active" id="page1">
        <div class="icon-box">🎉✨</div>
        <h1>Happy 20th Birthday!</h1>
        <h2>Dear Sarah ❤️</h2>
        <p>آج 16 نومبر کا دن بہت خاص ہے! <br>آپ کی زندگی کے خوبصورت <b>20 ویں سال</b> کا آغاز مبارک ہو۔</p>
        <p>آپ کے لیے ایک چھوٹا سا سرپرائز تیار کیا ہے، دیکھنے کے لیے آگے بڑھیں... ✨</p>
      </div>

      <!-- PAGE 2: The Special Day (16 Nov) -->
      <div class="page" id="page2">
        <div class="icon-box">📅🎂</div>
        <h1>16th November</h1>
        <h2>ایک خوبصورت شروعات</h2>
        <p>آج کے دن دنیا میں ایک بہت ہی پیاری اور خوبصورت روح آئی تھی۔</p>
        <p>20 سال پہلے کا یہ دن آپ کی فیملی اور ہم سب کے لیے بے شمار خوشیاں لے کر آیا تھا۔ <span class="highlight">آپ واقعی بہت سپیشل ہیں! 💖</span></p>
      </div>

      <!-- PAGE 3: Entering 20s Chapter -->
      <div class="page" id="page3">
        <div class="icon-box">👑🌟</div>
        <h1>Welcome to Chapter 20</h1>
        <h2>20 سال کا خوبصورت سفر</h2>
        <p>Teens کا سفر مکمل ہوا اور اب آپ اپنی زبردست <b>20s</b> کی عمر میں قدم رکھ رہی ہیں!</p>
        <p>دعاء ہے کہ یہ نیا سال آپ کی زندگی میں نہ ختم ہونے والی کامیابی، صحت، اور ڈھیروں خوشیاں لائے۔ ✨</p>
      </div>

      <!-- PAGE 4: Love & Appreciation Message -->
      <div class="page" id="page4">
        <div class="icon-box">💖🌸</div>
        <h1>You Are So Special!</h1>
        <h2>پیار اور محبت بھرا پیغام</h2>
        <p>سارہ! آپ کی مسکراہٹ، آپ کا انداز اور آپ کا ساتھ زندگی کا سب سے بہترین احساس ہے۔</p>
        <p>آپ کی موجودگی سے ہی آس پاس کا ماحول خوشگوار ہو جاتا ہے۔ ہمیشہ یونہی مسکراتی رہیں! 🌹</p>
      </div>

      <!-- PAGE 5: Birthday Wishes & Blessings -->
      <div class="page" id="page5">
        <div class="icon-box">🎁🎈</div>
        <h1>My Birthday Wishes</h1>
        <h2>دلی دعا و خواہشات</h2>
        <p>اللہ تعالیٰ آپ کو زندگی کے ہر موڑ پر کامران کرے، آپ کے ہر خواب کو پورا کرے اور آپ کو کبھی کوئی غم نہ ملے۔</p>
        <p>آپ کی ہنسی ہمیشہ قائم رہے! 🤲✨</p>
      </div>

      <!-- PAGE 6: Final Surprise / Love Confession -->
      <div class="page" id="page6">
        <div class="icon-box">🎂❤️</div>
        <h1>Happy Birthday Sarah!</h1>
        <h2>I Love You So Much! 💖</h2>
        <p>آپ میری زندگی کا سب سے پیارا اور انمول حصہ ہیں۔</p>
        <p>ہزاروں سال جیو اور ہمیشہ میرے ساتھ مسکراتی رہو! <br><span class="highlight">Once again, Happy 20th Birthday! 🎉🎂</span></p>
      </div>
    </div>

    <!-- Page Navigation Control -->
    <div class="nav-container">
      <div class="dots">
        <span class="dot active"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>
      <div class="btn-group">
        <button class="prev-btn hidden" id="prevBtn" onclick="changePage(-1)">واپس</button>
        <button class="next-btn" id="nextBtn" onclick="changePage(1)">آگے دیکھیں ➔</button>
      </div>
    </div>
  </div>

  <script>
    let currentPage = 1;
    const totalPages = 6;

    function changePage(direction) {
      document.getElementById(`page${currentPage}`).classList.remove('active');
      currentPage += direction;

      if (currentPage < 1) currentPage = 1;
      if (currentPage > totalPages) currentPage = totalPages;

      document.getElementById(`page${currentPage}`).classList.add('active');
      updateNav();
    }

    function updateNav() {
      // Update Dots
      const dots = document.querySelectorAll('.dot');
      dots.forEach((dot, index) => {
        if (index === currentPage - 1) {
          dot.classList.add('active');
        } else {
          dot.classList.remove('active');
        }
      });

      // Update Prev Button
      const prevBtn = document.getElementById('prevBtn');
      if (currentPage === 1) {
        prevBtn.classList.add('hidden');
      } else {
        prevBtn.classList.remove('hidden');
      }

      // Update Next Button Text on last page
      const nextBtn = document.getElementById('nextBtn');
      if (currentPage === totalPages) {
        nextBtn.innerText = "Enjoy Your Day! 🎉";
        nextBtn.style.background = "linear-gradient(45deg, #28a745, #20c997)";
      } else {
        nextBtn.innerText = "آگے دیکھیں ➔";
        nextBtn.style.background = "linear-gradient(45deg, #d63384, #fd7e14)";
      }
    }

    // Floating Background Elements
    function createBgElements() {
      const container = document.getElementById('bg-container');
      const items = ['🎈', '🎂', '💖', '✨', '🌸', '🎁', '🎉'];

      setInterval(() => {
        const el = document.createElement('div');
        el.classList.add('bg-element');
        el.innerText = items[Math.floor(Math.random() * items.length)];
        el.style.left = Math.random() * 100 + 'vw';
        el.style.fontSize = (Math.random() * 20 + 15) + 'px';
        el.style.animationDuration = (Math.random() * 3 + 4) + 's';
        container.appendChild(el);

        setTimeout(() => {
          el.remove();
        }, 6000);
      }, 350);
    }

    createBgElements();
  </script>
</body>
</html>
