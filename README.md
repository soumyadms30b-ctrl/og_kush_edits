# Create updated website with Instagram + YouTube buttons

html_content = """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>og_kush_edits</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
    body { background: #0f0f0f; color: #fff; }
    header {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(135deg, #1e1e1e, #000);
    }
    header h1 { font-size: 3rem; letter-spacing: 2px; }
    header p { margin-top: 15px; font-size: 1.2rem; color: #aaa; }

    .btn {
      margin-top: 15px;
      padding: 12px 30px;
      color: #fff;
      border: none;
      border-radius: 25px;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
    }
    .btn-explore { background: #ff004f; }
    .btn-youtube { background: #ff0000; }
    .btn-instagram { background: linear-gradient(45deg, #f58529, #dd2a7b, #8134af); }

    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    section h2 { text-align: center; margin-bottom: 30px; font-size: 2rem; }
    .about p { text-align: center; color: #ccc; line-height: 1.6; }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: #1c1c1c;
      padding: 20px;
      border-radius: 12px;
      text-align: center;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: #000;
      color: #777;
    }
  </style>
</head>
<body>
  <header>
    <h1>og_kush_edits</h1>
    <p>Anime • CapCut • Creative Video Edits</p>

    <a href="#about" class="btn btn-explore">Explore</a><br/>
    <a href="https://www.youtube.com/@ogkushedits" target="_blank" class="btn btn-youtube">
      🔴 YouTube Channel
    </a><br/>
    <a href="https://www.instagram.com/edits.exe.22?igsh=Mm4yZHliNXBwenl5" target="_blank" class="btn btn-instagram">
      📸 Instagram Profile
    </a>
  </header>

  <section id="about" class="about">
    <h2>About Me</h2>
    <p>
      Welcome to <b>og_kush_edits</b> 🎬<br />
      I create high-quality anime & CapCut edits.<br/>
      Follow me on YouTube & Instagram for daily edits 🔥
    </p>
  </section>

  <section>
    <h2>What I Do</h2>
    <div class="services">
      <div class="card">Anime Edits</div>
      <div class="card">Instagram Reels</div>
      <div class="card">CapCut Templates</div>
      <div class="card">YouTube Shorts</div>
    </div>
  </section>

  <footer>
    <p>© 2025 og_kush_edits | All Rights Reserved</p>
  </footer>
</body>
</html>
"""

file_path = "/mnt/data/og_kush_edits_with_youtube_instagram.html"
with open(file_path, "w") as f:
    f.write(html_content)

file_path
