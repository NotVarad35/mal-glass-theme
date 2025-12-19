# Customization Guide

This document explains how to customize **MAL Glass Theme** to match your personal preferences.
All customization is done by editing `theme.css`.

⚠️ Note  
MyAnimeList only allows **CSS-based customization**. JavaScript, HTML changes, and external fonts for visitors are restricted.

---

## 🎨 Theme Colors (Optional)

You can define custom colors at the top of `theme.css` for easier editing:

```css
:root {
  --accent: #1db954;
  --header-text: #8fd3ff;
  --glass-bg: rgba(20,20,24,0.85);
}

##🖼️ Changing Background Image
body::before {
    background: url("assets/bg-img.jpg") center / cover no-repeat;
}

##🖼️ Changing Cover Artwork
.cover-block .image-container img {
    content: url("assets/cover-art.png");
}

##🔤 Changing Font
font-family: "JetBrains Mono", Consolas, monospace;

##🎯 Status Bar Colors
.data.status.watching {
    background: linear-gradient(180deg, #1db954, #0f7a3c);
}

##🧊 Blur Strength
#column,
.list-container {
    backdrop-filter: blur(12px);
}



