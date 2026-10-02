---
layout: default
title: "Repositories | hv33y"
permalink: /repo/
description: "Source code index for automation scripts, UI bypasses, and custom web infrastructure."
keywords: "hv33y, repositories, automation, scripts, github"
author: "hv33y"
robots: "index, follow"

og:
  title: "Repositories | hv33y"
  type: website
  url: "https://hv33y.github.io/repo/"
  description: "Source code index for automation scripts, UI bypasses, and custom web infrastructure."
  image: "https://hv33y.github.io/og-preview.jpg"

twitter:
  card: summary_large_image
  title: "Repositories | hv33y"
  description: "Source code index for automation scripts, UI bypasses, and custom web infrastructure."
  image: "https://hv33y.github.io/og-preview.jpg"
---

<style>
  header, .page-header, .project-name, .project-tagline { display: none !important; }
  .markdown-body > h1:first-child { display: none !important; }
  
  html, body { width: 100%; margin: 0; padding: 0; overflow-x: hidden; }
  
  body, .markdown-body { 
    background: radial-gradient(circle at 50% 0%, #1a0b12, #050505 80%) !important; 
    background-color: #050505 !important;
    color: #f5f5f7 !important; 
    font-family: 'Google Sans', -apple-system, BlinkMacSystemFont, sans-serif !important; 
    min-height: 100vh;
  }

  .wrapper, .container, .container-lg, .markdown-body, main, section {
    max-width: 1100px !important; width: 100% !important; margin: 0 auto !important;
    padding: 0 20px !important; float: none !important; box-sizing: border-box !important;
  }

  .hero { text-align: center; padding: 80px 20px 40px; width: 100%; }
  .hero h1 {
    font-size: 4.5rem !important; font-weight: 900 !important; letter-spacing: -0.05em;
    margin-bottom: 10px !important;
    background: linear-gradient(135deg, #ffffff, #800020);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent; border: none !important;
  }
  .hero p { font-size: 1.2rem; color: #a1a1a6; max-width: 600px; margin: 0 auto; line-height: 1.5; }

  .social-pills { display: flex; justify-content: center; gap: 15px; margin-top: 30px; flex-wrap: wrap; }
  .social-pills a {
    background: rgba(255, 255, 255, 0.05); border: 1px solid rgba(255, 255, 255, 0.1);
    color: #fff !important; padding: 10px 24px; border-radius: 50px;
    text-decoration: none !important; font-weight: 600; transition: all 0.3s ease;
    backdrop-filter: blur(10px); -webkit-backdrop-filter: blur(10px);
  }
  .social-pills a:hover {
    background: rgba(128, 0, 32, 0.2); border-color: rgba(128, 0, 32, 0.5); transform: translateY(-3px);
  }

  .bento-grid {
    display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 24px; max-width: 1000px; margin: 40px auto 60px; width: 100%;
  }

  .bento-card {
    background: rgba(255, 255, 255, 0.02); border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 24px; padding: 32px;
    backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
    transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
    display: flex; flex-direction: column; text-decoration: none !important; color: inherit !important;
  }
  .bento-card:hover {
    transform: translateY(-8px) scale(1.02); border-color: rgba(128, 0, 32, 0.4);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.5), inset 0 0 0 1px rgba(128, 0, 32, 0.2);
  }
  .bento-card h3 { margin-top: 0 !important; font-size: 1.5rem; color: #ffffff; border: none !important; }
  .bento-card p { color: #a1a1a6; flex-grow: 1; line-height: 1.6; }

  .tags { margin-top: 20px; }
  .tag {
    background: rgba(255, 255, 255, 0.08); color: #eaeaea; padding: 6px 12px;
    border-radius: 8px; font-size: 0.85rem; font-weight: 600; display: inline-block; margin: 0 6px 6px 0;
  }
</style>

<div class="hero">
  <h1>Repositories</h1>
  <p>Source code index for automation scripts, UI bypasses, and custom web infrastructure.</p>
  
  <div class="social-pills">
    <a href="/">Index</a>
    <a href="https://github.com/hv33y">GitHub</a>
    <a href="/contact">Contact</a>
  </div>
</div>

<div class="bento-grid">
  <a href="https://github.com/hv33y/systemwide-adb-installer" class="bento-card">
    <h3>systemwide-adb-installer</h3>
    <p>Lightweight one-line Windows script to download, configure, and install Android ADB & Fastboot system-wide.</p>
    <div class="tags"><span class="tag">Batchfile</span><span class="tag">System Tool</span></div>
  </a>

  <a href="https://github.com/hv33y/delete-linkedin-skills" class="bento-card">
    <h3>delete-linkedin-skills</h3>
    <p>Rapid DOM automation script for mass skills removal directly from a LinkedIn profile.</p>
    <div class="tags"><span class="tag">JavaScript</span><span class="tag">DOM</span></div>
  </a>

  <a href="https://github.com/hv33y/reddit-raw-image-viewer" class="bento-card">
    <h3>reddit-raw-image-viewer</h3>
    <p>A lightweight userscript to bypass Reddit media redirects and instantly load direct raw images.</p>
    <div class="tags"><span class="tag">JavaScript</span><span class="tag">Userscript</span></div>
  </a>

  <a href="https://github.com/hv33y/abyss-jellyfin" class="bento-card">
    <h3>abyss-jellyfin</h3>
    <p>Customizable, high-contrast minimal dark theme CSS engineered for Jellyfin media clients.</p>
    <div class="tags"><span class="tag">CSS</span><span class="tag">Theming</span></div>
  </a>

  <a href="https://github.com/hv33y/gd-index" class="bento-card">
    <h3>gd-index</h3>
    <p>Multi-branch cloud drive index explorer for Google Drive.</p>
    <div class="tags"><span class="tag">Web</span><span class="tag">Indexer</span></div>
  </a>

  <a href="https://github.com/hv33y/lyc8503-onedrive-cf-index-ng" class="bento-card">
    <h3>onedrive-cf-index-ng</h3>
    <p>OneDrive public directory listing running on Docker and Cloudflare Workers.</p>
    <div class="tags"><span class="tag">TypeScript</span><span class="tag">Cloudflare</span></div>
  </a>
</div>

<div align="center" style="margin: 40px 0; padding-bottom: 40px;">
  <a href="https://github.com/hv33y?tab=repositories" style="color: #58a6ff; text-decoration: none; font-weight: 600;">View all 24 repositories on GitHub ↗</a>
</div>
