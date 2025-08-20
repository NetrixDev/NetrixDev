# 👾 NetrixDev - The Cyber Frontier

<style>
  /* Global resets and theme - Cyberpunk hacker aesthetic */
  .profile-container {
    font-family: 'Courier New', monospace;
    color: #00FF00; /* Neon green text */
    background: linear-gradient(135deg, #0D0D0D, #1A1A1A); /* Dark void gradient */
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 20px rgba(0, 255, 0, 0.2); /* Glowing edge */
    max-width: 1200px;
    margin: 0 auto;
    overflow: hidden;
    position: relative;
  }

  .profile-container::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle, rgba(0,255,0,0.1), transparent);
    opacity: 0.5;
    pointer-events: none;
    animation: pulse 5s infinite;
  }

  @keyframes pulse {
    0% { opacity: 0.3; }
    50% { opacity: 0.6; }
    100% { opacity: 0.3; }
  }

  /* Grid layout - Advanced CSS Grid for UI/UX */
  .profile-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: auto auto auto;
    gap: 20px;
    grid-template-areas:
      "header header header"
      "about skills news"
      "projects contact contact";
  }

  .header { grid-area: header; text-align: center; animation: glitch 2s infinite; }
  .about { grid-area: about; }
  .skills { grid-area: skills; }
  .news { grid-area: news; }
  .projects { grid-area: projects; }
  .contact { grid-area: contact; }

  @keyframes glitch {
    0% { transform: translate(0); }
    20% { transform: translate(-2px, 2px); }
    40% { transform: translate(2px, -2px); }
    60% { transform: translate(-2px, 2px); }
    80% { transform: translate(2px, -2px); }
    100% { transform: translate(0); }
  }

  /* Interactive skill cards - Hover effects, animations */
  .skill-card {
    background: rgba(0, 0, 0, 0.8);
    padding: 15px;
    border: 1px solid #00FF00;
    border-radius: 5px;
    transition: transform 0.3s, box-shadow 0.3s;
    cursor: pointer;
    position: relative;
    overflow: hidden;
  }

  .skill-card:hover {
    transform: scale(1.05);
    box-shadow: 0 0 15px #00FF00;
  }

  .skill-card::after {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(0,255,0,0.2), transparent);
    opacity: 0;
    transition: opacity 0.5s;
  }

  .skill-card:hover::after {
    opacity: 1;
  }

  /* Progress bars for skills - Animated on load */
  .skill-bar {
    background: #333;
    height: 10px;
    border-radius: 5px;
    margin-top: 5px;
    overflow: hidden;
  }

  .skill-progress {
    height: 100%;
    background: linear-gradient(90deg, #00FF00, #00CC00);
    animation: load-bar 2s ease-out;
  }

  @keyframes load-bar {
    0% { width: 0; }
    100% { width: var(--progress); }
  }

  /* News section - Placeholder for dynamic update */
  .news-item {
    background: rgba(255, 255, 255, 0.05);
    padding: 10px;
    margin-bottom: 10px;
    border-left: 3px solid #00FF00;
    transition: background 0.3s;
  }

  .news-item:hover {
    background: rgba(255, 255, 255, 0.1);
  }

  /* Responsive design - Mobile friendly */
  @media (max-width: 768px) {
    .profile-grid {
      grid-template-columns: 1fr;
      grid-template-areas:
        "header"
        "about"
        "skills"
        "news"
        "projects"
        "contact";
    }
  }
</style>

<div class="profile-container">
  <div class="profile-grid">
    <div class="header">
      <h1>👾 NetrixDev</h1>
      <p>Cybersecurity Maverick | Code Weaver | Ethical Hacker Extraordinaire</p>
      <img src="https://img.shields.io/badge/Hack-The-Planet-00FF00?style=for-the-badge&logo=hackthebox" alt="Hack Badge">
    </div>

    <div class="about">
      <h2>🔒 About Me</h2>
      <p>I'm NetrixDev, a passionate developer and cybersecurity enthusiast. Proficient in building secure, high-performance applications while wielding Kali Linux tools to uncover vulnerabilities. From gray hat hacking techniques to animating complex ideas with Manim, I thrive in the digital shadows.</p>
      <details>
        <summary>More Details (Interactive Toggle)</summary>
        <p>Exploring the intersection of code and security. Always hunting for the next exploit or optimization.</p>
      </details>
    </div>

    <div class="skills">
      <h2>🛠️ Skills Arsenal</h2>
      <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px;">
        <div class="skill-card">
          <p>💻 C++</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 95%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🐍 Python</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 90%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🎥 Manim</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 85%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🌐 JavaScript</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 90%;"></div></div>
        </div>
        <div class="skill-card">
          <p>📜 TypeScript</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 85%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🦀 Rust</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 80%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🔧 Assembly</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 75%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🖼️ Qt</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 80%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🐧 Kali Linux</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 95%;"></div></div>
        </div>
        <div class="skill-card">
          <p>🕵️ Gray Hat Hacking</p>
          <div class="skill-bar"><div class="skill-progress" style="--progress: 90%;"></div></div>
        </div>
      </div>
    </div>

    <div class="news">
      <h2>🌐 Live Cybersecurity News</h2>
      <p>Stay ahead of threats with real-time updates from top sources.</p>
      <!-- NEWS_START -->
      - [Latest Exploit Discovered](https://example.com)  
      - [New Ransomware Wave](https://example.com)  
      - [Patch Tuesday Alerts](https://example.com)  
      <!-- NEWS_END -->
      <p><small>Updated automatically via GitHub Actions. Powered by RSS feeds from The Hacker News or Cyber Security Hub.</small></p>
    </div>

    <div class="projects">
      <h2>🚀 Featured Projects</h2>
      <ul>
        <li><a href="https://github.com/NetrixDev/project1">SecureVault - Rust-based Encryption Tool</a></li>
        <li><a href="https://github.com/NetrixDev/project2">HackSim - Manim-animated Cybersecurity Simulations</a></li>
        <li>And more... Explore my repos!</li>
      </ul>
    </div>

    <div class="contact">
      <h2>📡 Connect</h2>
      <p>Let's hack the future together!</p>
      <a href="https://twitter.com/NetrixDev"><img src="https://img.shields.io/twitter/follow/NetrixDev?style=social" alt="Twitter"></a>
      <a href="https://linkedin.com/in/NetrixDev"><img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin"></a>
    </div>
  </div>
</div>

## Setup Instructions for Live Features
This README uses advanced CSS for a grid-based, interactive UI with animations and hover effects. For the **live Cybersecurity news**, it can't be truly real-time in a static README, but we can make it dynamic by auto-updating via GitHub Actions:

1. Create a repository named `NetrixDev` (your username) if not already done – this makes it your profile README.
2. Add the above content to `README.md`.
3. For news: Use the [rss-to-readme GitHub Action](https://github.com/JasonEtco/rss-to-readme). Create a `.github/workflows/update-news.yml` file with:
   ```
   name: Update News
   on:
     schedule:
       - cron: '0 */6 * * *'  # Every 6 hours
     workflow_dispatch:
   jobs:
     update:
       runs-on: ubuntu-latest
       steps:
         - uses: actions/checkout@v2
         - uses: JasonEtco/rss-to-readme@v1
           with:
             feed-url: https://thehackernews.com/rss.xml  # Or https://www.cshub.com/rss
             readme-section: NEWS
             max: 3  # Show top 3 news items
         - uses: test-room-7/action-update-file@v1
           with:
             file-path: README.md
             commit-msg: Update cybersecurity news
             github-token: ${{ secrets.GITHUB_TOKEN }}
   ```
4. Commit and push. The action will fetch RSS feeds (e.g., from The Hacker News) and update the news section automatically.

This setup ensures your profile is memorable, with a cyber-themed design that loads fast and works on mobile. Customize progress percentages, links, or add more grids as needed! 🚀
