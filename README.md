<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Anime World</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background-color: #0f0f1a;
      color: #ffffff;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #1a1a2e;
      text-align: center;
      padding: 30px 20px;
    }

    h1 {
      color: #ff66cc;
      font-size: 2.2em;
    }

    nav {
      background-color: #16213e;
      display: flex;
      justify-content: center;
      gap: 25px;
      padding: 15px;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ff66cc;
    }

    section {
      padding: 30px 20px;
      text-align: center;
    }

    .anime-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      padding: 20px;
    }

    .anime-card {
      background-color: #1a1a2e;
      border-radius: 10px;
      padding: 15px;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .anime-card:hover {
      transform: scale(1.05);
      box-shadow: 0 0 15px #ff66cc;
    }

    .anime-card img {
      width: 100%;
      border-radius: 10px;
    }

    .anime-card h3 {
      color: #ff66cc;
      margin-top: 10px;
    }

    .anime-card p {
      font-size: 0.9em;
      color: #ddd;
    }

    iframe {
      width: 80%;
      height: 400px;
      border: none;
      border-radius: 10px;
      box-shadow: 0 0 15px #ff66cc;
      margin-top: 20px;
    }

    .link-box {
      background-color: #1a1a2e;
      padding: 15px;
      border-radius: 10px;
      display: inline-block;
      margin-top: 30px;
    }

    input {
      padding: 8px;
      width: 250px;
      border-radius: 5px;
      border: none;
    }

    button {
      background-color: #ff66cc;
      color: #fff;
      border: none;
      padding: 8px 12px;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background-color: #ff3385;
    }

    footer {
      background-color: #1a1a2e;
      text-align: center;
      padding: 15px;
      color: #aaa;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <h1>🌸 Welcome to Anime World 🌸</h1>
    <p>Your gateway to the best anime across genres!</p>
  </header>

  <nav>
    <a href="#action">Action</a>
    <a href="#romance">Romance</a>
    <a href="#fantasy">Fantasy</a>
    <a href="#trailer">Trailer</a>
  </nav>

  <section id="action">
    <h2>🔥 Top Action Anime</h2>
    <div class="anime-grid">
      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/2/20/Attack_on_Titan_cover.jpg" alt="Attack on Titan">
        <h3>Attack on Titan</h3>
        <p>Humanity fights for survival against giant humanoid Titans in this intense series.</p>
      </div>

      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/7/72/Demon_Slayer_Kimetsu_no_Yaiba_volume_1_cover.jpg" alt="Demon Slayer">
        <h3>Demon Slayer</h3>
        <p>Tanjiro sets out on a quest to save his sister and destroy the demons plaguing Japan.</p>
      </div>
    </div>
  </section>

  <section id="romance">
    <h2>💖 Heartwarming Romance Anime</h2>
    <div class="anime-grid">
      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/7/7b/Your_Lie_in_April_manga_volume_1_cover.jpg" alt="Your Lie in April">
        <h3>Your Lie in April</h3>
        <p>A pianist finds love and inspiration from a free-spirited violinist.</p>
      </div>

      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/5/5e/Toradora%21_light_novel_volume_1_cover.jpg" alt="Toradora!">
        <h3>Toradora!</h3>
        <p>A charming romantic comedy between two unlikely high school students.</p>
      </div>
    </div>
  </section>

  <section id="fantasy">
    <h2>🌌 Magical Fantasy Worlds</h2>
    <div class="anime-grid">
      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/0/0d/Sword_Art_Online_light_novel_volume_1_cover.jpg" alt="Sword Art Online">
        <h3>Sword Art Online</h3>
        <p>Players trapped in a virtual game world must fight their way to freedom.</p>
      </div>

      <div class="anime-card">
        <img src="https://upload.wikimedia.org/wikipedia/en/0/0c/Re_Zero_light_novel_cover_volume_1.jpg" alt="Re:Zero">
        <h3>Re:Zero</h3>
        <p>Subaru finds himself reliving death in a mysterious fantasy world.</p>
      </div>
    </div>
  </section>

  <section id="trailer">
    <h2>🎬 Watch a Popular Anime Trailer</h2>
    <iframe 
      src="https://www.youtube.com/embed/VQGCKyvzIM4" 
      title="Demon Slayer Trailer" 
      allowfullscreen>
    </iframe>

    <div class="link-box">
      <p>Copy this link to explore more anime:</p>
      <input type="text" value="https://myanimelist.net" id="animeLink" readonly>
      <button onclick="copyLink()">Copy Link</button>
    </div>
  </section>

  <footer>
    <p>© 2025 Anime World | Made with ❤️ by an anime fan</p>
  </footer>

  <script>
    function copyLink() {
      const copyText = document.getElementById("animeLink");
      copyText.select();
      copyText.setSelectionRange(0, 99999);
      navigator.clipboard.writeText(copyText.value);
      alert("Link copied to clipboard!");
    }
  </script>
</body>
</html>

