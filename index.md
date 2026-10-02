---
layout: default
title: "hv33y | Web Interfaces & Systems"
description: "Personal site and project directory for hv33y."
keywords: "hv33y, hvOS, automation, UI, developer"
author: "hv33y"
robots: "index, follow"

og:
  title: "hv33y | Web Interfaces & Systems"
  type: website
  url: "https://hv33y.github.io/"
  description: "Personal site and project directory for hv33y."
  image: "https://hv33y.github.io/og-preview.jpg"

twitter:
  card: summary_large_image
  title: "hv33y | Web Interfaces & Systems"
  description: "Personal site and project directory for hv33y."
  image: "https://hv33y.github.io/og-preview.jpg"
---

<style>
  /* 1. Nuke GitHub's default layout constraints & injected headers */
  header, .page-header, .project-name, .project-tagline { display: none !important; }
  .markdown-body > h1:first-child { display: none !important; }
  
  html, body {
    width: 100%;
    margin: 0;
    padding: 0;
    overflow-x: hidden;
  }
  
  body, .markdown-body { 
    /* Centered the radial glow */
    background: radial-gradient(circle at 50% 0%, #1a0b12, #050505 80%) !important; 
    background-color: #050505 !important;
    color: #f5f5f7 !important; 
    font-family: 'Google Sans', -apple-system, BlinkMacSystemFont, sans-serif !important; 
    min-height: 100vh;
  }

  /* 2. Break out of the left-aligned container and center the grid */
  .wrapper, .container, .container-lg, .markdown-body, main, section {
    max-width: 1100px !important;
    width: 100% !important;
    margin: 0 auto !important;
    padding: 0 20px !important;
    float: none !important;
    box-sizing: border-box !important;
  }

  /* 4DX Hero Section */
  .hero {
    text-align: center;
    padding: 80px 20px 40px;
    width: 100%;
  }
  .hero h1 {
    font-size: 4.5rem !important;
    font-weight: 900 !important;
    letter-spacing: -0.05em;
    margin-bottom: 10px !important;
    background: linear-gradient(135deg, #ffffff, #800020);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    border: none !important;
  }
  .hero p {
    font-size: 1.2rem;
    color: #a1a1a6;
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.5;
  }

  /* Social Links */
  .social-pills {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-top: 30px;
    flex-wrap: wrap;
  }
  .social-pills a {
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    color: #fff !important;
    padding: 10px 24px;
    border-radius: 50px;
    text-decoration: none !important;
    font-weight: 600;
    transition: all 0.3s ease;
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
  }
  .social-pills a:hover {
    background: rgba(128, 0, 32, 0.2);
    border-color: rgba(128, 0, 32, 0.5);
    transform: translateY(-3px);
  }

  /* Gen Z Bento Grid */
  .bento-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 24px;
    max-width: 1000px;
    margin: 60px auto;
    width: 100%;
  }

  /* Glassmorphism Cards */
  .bento-card {
    background: rgba(255, 255, 255, 0.02);
    border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 24px;
    padding: 32px;
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
    display: flex;
    flex-direction: column;
    text-decoration: none !important;
    color: inherit !important;
  }
  .bento-card:hover {
    transform: translateY(-8px) scale(1.02);
    border-color: rgba(128, 0, 32, 0.4);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5), inset 0 0 0 1px rgba(128, 0, 32, 0.2);
  }
  .bento-card h3 {
    margin-top: 0 !important;
    font-size: 1.5rem;
    color: #ffffff;
    border: none !important;
  }
  .bento-card p {
    color: #a1a1a6;
    flex-grow: 1;
    line-height: 1.6;
  }

  /* Tech Stack Tags */
  .tags {
    margin-top: 20px;
  }
  .tag {
    background: rgba(255, 255, 255, 0.08);
    color: #eaeaea;
    padding: 6px 12px;
    border-radius: 8px;
    font-size: 0.85rem;
    font-weight: 600;
    display: inline-block;
    margin: 0 6px 6px 0;
  }

  /* GitHub Stats Span */
  .stats-container {
    max-width: 1000px;
    margin: 0 auto 60px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 24px;
    width: 100%;
  }
  .stats-container img {
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.05);
    background: rgba(255, 255, 255, 0.02);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
  }
</style>

<link rel="icon" type="image/png" href="hv33y.png">
<link rel="apple-touch-icon" href="hv33y.png">

<div class="hero">
  <h1>hv33y</h1>
  <p>Building high-performance interfaces, automated media systems, and sleek deployment workflows.</p>
  
  <div class="social-pills">
    <a href="https://github.com/hv33y">GitHub</a>
    <a href="/repo">Repositories</a>
    <a href="/tools">Tools</a>
    <a href="/contact">Contact</a>
  </div>
</div>

<div class="stats-container">
  <img src="https://github-readme-stats.vercel.app/api?username=hv33y&show_icons=true&theme=transparent&hide_border=true&icon_color=ffffff&title_color=ffffff&text_color=a1a1a6" alt="hv33y Stats" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hv33y&layout=compact&theme=transparent&hide_border=true&title_color=ffffff&text_color=a1a1a6" alt="Top Languages" height="150" />
</div>

<div class="bento-grid">
  <!-- hvOS -->
  <a href="https://github.com/hv33y/hvOS" class="bento-card">
    <h3>hvOS</h3>
    <p>Transforms desktop YouTube into a fluid Apple TV experience with ambient lighting and instant load times.</p>
    <div class="tags">
      <span class="tag">JavaScript</span>
      <span class="tag">UI/UX</span>
    </div>
  </a>

  <!-- inline-b64-reveal -->
  <a href="https://github.com/hv33y/inline-b64-reveal" class="bento-card">
    <h3>inline-b64-reveal</h3>
    <p>Automatically detects, decodes, and displays Base64 strings inline with a quick-copy UI.</p>
    <div class="tags">
      <span class="tag">JavaScript</span>
      <span class="tag">DOM</span>
    </div>
  </a>

  <!-- gemini-sweep -->
  <a href="https://github.com/hv33y/gemini-sweep" class="bento-card">
    <h3>gemini-sweep</h3>
    <p>Automated cleanup utility that sequentially purges unpinned AI conversations.</p>
    <div class="tags">
      <span class="tag">Automation</span>
      <span class="tag">Workflow</span>
    </div>
  </a>

  <!-- open-directory -->
  <a href="https://github.com/hv33y/open-directory" class="bento-card">
    <h3>open-directory</h3>
    <p>Fast web directory crawler and index explorer designed for instant resource discovery.</p>
    <div class="tags">
      <span class="tag">HTML</span>
      <span class="tag">Search</span>
    </div>
  </a>
</div>

<div align="center" style="margin: 60px 0 40px; color: #6e6e73; font-size: 0.9rem;">
  hv33y • 2026
</div>
