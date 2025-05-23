<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Tech with Treasure</title>
  <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body, html {
      height: 100%;
      font-family: 'Raleway', sans-serif;
    }

    .background {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('https://www.worldbank.org/content/dam/photos/780x439/2017/oct-3/GFDR-2017-cover-animated.gif') no-repeat center center fixed;
      background-size: cover;
      z-index: -2;
    }

    .overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      z-index: -1;
    }

    .hero {
      text-align: center;
      padding: 80px 20px 20px;
      color: #fff;
    }

    .hero h1 {
      font-size: 3em;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 1.2em;
    }

    .section-title {
      text-align: center;
      margin-top: 40px;
      font-size: 1.8em;
      color: #fff;
    }

    .cards {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 30px 20px;
    }

    .card {
      background-color: rgba(0, 0, 0, 0.75); /* Black translucent shield */
      padding: 20px;
      border-radius: 15px;
      max-width: 280px;
      width: 100%;
      color: #fff;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.8);
    }

    .card h3 {
      color: #00d1ff;
      margin-bottom: 10px;
    }

    .explore-button {
      display: block;
      margin: 20px auto 40px;
      padding: 12px 30px;
      font-size: 16px;
      font-weight: bold;
      background-color: #00d1ff;
      color: #000;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .explore-button:hover {
      background-color: #00b5e2;
    }

    #blog-frame-container {
      display: none;
      max-width: 1000px;
      margin: 40px auto;
      padding: 20px;
    }

    #blog-frame {
      width: 100%;
      height: 600px;
      border: none;
      border-radius: 8px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
    }
  </style>
</head>
<body>

  <div class="background"></div>
  <div class="overlay"></div>

  <section class="hero">
    <h1>Tech with Treasure</h1>
    <p>Your ultimate source for tech trends, AI gadgets, and smart savings tips.</p>
  </section>

  <h2 class="section-title">Explore Our Highlights</h2>

  <section class="cards">
    <div class="card">
      <h3>ðŸ“° Tech News</h3>
      <p>Stay updated on breakthroughs in AI, apps, and devices that are shaping tomorrow.</p>
    </div>

    <div class="card">
      <h3>ðŸ’° Finance & Deals</h3>
      <p>Discover cost-saving strategies, tech discounts, and smart spending tips.</p>
    </div>

    <div class="card">
      <h3>ðŸ§  AI & Innovation</h3>
      <p>Dive into the evolving world of artificial intelligence and futuristic technologies.</p>
    </div>

    <div class="card">
      <h3>ðŸ” Gadget Reviews</h3>
      <p>Get our verdict on the latest smartphones, laptops, wearables, and more.</p>
    </div>
  </section>

  <button class="explore-button" onclick="showBlog()">Explore Blogs</button>

  <div id="blog-frame-container">
    <iframe id="blog-frame" src=""></iframe>
  </div>

  <script>
    function showBlog() {
      const frame = document.getElementById("blog-frame");
      frame.src = "https://srilankatechnova.blogspot.com/";
      document.getElementById("blog-frame-container").style.display = "block";
      window.scrollTo({
        top: document.getElementById("blog-frame-container").offsetTop,
        behavior: "smooth"
      });
    }
  </script>

</body>
</html>
