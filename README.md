<div align="center">

<!-- Animated live contribution heatmap: real GitHub data, boxes slide in diagonally (refreshed daily via GitHub Actions) -->
<h3><code>sivsubramanian@github ~ $ ./contributions.sh</code></h3>

<img src="./contrib-heatmap.svg" width="860" alt="Sivasubramanian's Live GitHub Contribution Graph" />

<br>
<br>

<!-- Live Streak & Analytics Terminal Card -->
<h3><code>sivsubramanian@github ~ $ ./stats.sh</code></h3>

<img src="./stats.svg" width="840" alt="Sivasubramanian's Activity Stats & Streak Card" />

<br>
<br>

<h3><code>sivsubramanian@github ~ $ cat info.txt</code></h3>

<p align="center">
  <b>Sivasubramanian M</b> · AI Enthusiast & B.Tech in AI & Data Science<br>
  Specialized in Data Analytics, Python, Generative AI Tools & Project Coordination
</p>

<p align="center">
  <a href="https://github.com/sivsubramanian">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  &nbsp;
  <a href="mailto:sivasufriend@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

</div>

---

### ⚙️ How It Works

- **No Third-Party Rate Limits**: Scrapes GitHub's public contribution calendar via lightweight Python scripts directly into `data/contributions.json`.
- **Pure SVG Animation**: Uses pure CSS keyframes and SMIL embedded inside SVGs—no client-side JavaScript needed (works natively on GitHub profile pages).
- **Auto-Refreshed Daily**: A GitHub Actions workflow (`.github/workflows/update-profile-art.yml`) automatically regenerates `contrib-heatmap.svg` and `stats.svg` every day at ~06:17 UTC.

### 🖼️ Adding an ASCII Portrait (Optional)

If you'd like to place an animated ASCII portrait alongside the stats card:
1. Place a photo as `source-photo.jpg` in this directory.
2. Run:
   ```bash
   pip install pillow numpy opencv-python rembg
   python scripts/prep_photo.py source-photo.jpg
   python scripts/make_ascii_svg.py
   ```
3. Update `README.md` to place `portrait-ascii.svg` and `stats.svg` side-by-side using the provided `<table>` layout.
