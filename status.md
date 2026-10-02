---
layout: default
title: "System Status | hv33y"
permalink: /status/
---

<style>
  body { background-color: #0d1117 !important; color: #c9d1d9 !important; font-family: 'Google Sans', -apple-system, sans-serif !important; }
  a { color: #58a6ff !important; text-decoration: none; }
  a:hover { text-decoration: underline; }
  .status-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin-top: 20px; }
  .status-card { border: 1px solid #30363d; padding: 15px; border-radius: 6px; background: #161b22; }
  .dot { height: 10px; width: 10px; background-color: #238636; border-radius: 50%; display: inline-block; margin-right: 8px; }
  hr { border-top: 1px solid #21262d !important; margin: 40px 0; }
</style>

<div align="center">

<h2>System Status</h2>

<p>
  <a href="/">Index</a> &nbsp;•&nbsp; <a href="/repo">Repositories</a> &nbsp;•&nbsp; <strong>Status</strong>
</p>

<hr>

</div>

<div class="status-grid">
  <div class="status-card">
    <span class="dot"></span> <strong>kxdhvbot API</strong><br>
    <small style="color: #8b949e;">Telegram automation relay</small>
  </div>
  <div class="status-card">
    <span class="dot"></span> <strong>Media Stack</strong><br>
    <small style="color: #8b949e;">Jellyfin / Radarr / Sonarr / Aria2</small>
  </div>
  <div class="status-card">
    <span class="dot"></span> <strong>d.harry.run</strong><br>
    <small style="color: #8b949e;">GitHub Actions Deployment</small>
  </div>
  <div class="status-card">
    <span class="dot"></span> <strong>Cloudflare Workers</strong><br>
    <small style="color: #8b949e;">Directory indexers & routing</small>
  </div>
</div>
