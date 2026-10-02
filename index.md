---
layout: default
title: "hv33y | Developer, Automation & Systems"
description: "Personal site and project directory for hv33y. Custom user interfaces, Cloudflare automations, Tampermonkey userscripts, and lightweight developer utilities."
keywords: "hv33y, hvOS, automation, userscripts, cloudflare workers, github pages"
author: "hv33y"
robots: "index, follow"
---

<style>
  body {
    background-color: #0d1117 !important;
    color: #c9d1d9 !important;
    font-family: 'Google Sans', -apple-system, BlinkMacSystemFont, sans-serif !important;
  }
  a { color: #58a6ff !important; text-decoration: none; }
  a:hover { text-decoration: underline; }
  table td { border: 1px solid #30363d !important; }
  hr { border-top: 1px solid #21262d !important; }
  code { background: rgba(110,118,129,0.4) !important; color: #c9d1d9 !important; border-radius: 4px; padding: 2px 6px; }
</style>
<button id="theme-toggle" style="position: fixed; top: 20px; right: 20px; background: transparent; border: 1px solid #30363d; color: #c9d1d9; padding: 5px 10px; border-radius: 5px; cursor: pointer; font-family: 'Google Sans';">Toggle Light Mode</button>

<script>
  document.getElementById('theme-toggle').addEventListener('click', () => {
    const body = document.body;
    if (body.style.backgroundColor === 'rgb(255, 255, 255)') {
      body.style.backgroundColor = '#0d1117';
      body.style.color = '#c9d1d9';
      document.getElementById('theme-toggle').style.color = '#c9d1d9';
    } else {
      body.style.backgroundColor = '#ffffff';
      body.style.color = '#24292f';
      document.getElementById('theme-toggle').style.color = '#24292f';
    }
  });
</script>

<link rel="icon" type="image/png" href="hv33y.png">
<link rel="apple-touch-icon" href="hv33y.png">

<div align="center">

<h2>Developer • Automation • Web Interfaces</h2>

<p>
  <strong>Index</strong> &nbsp;•&nbsp; <a href="/repo">Repositories</a>
</p>

<!-- Live GitHub API Stats -->
<p>
  <a href="https://github.com/hv33y">
    <img src="https://github-readme-stats.vercel.app/api?username=hv33y&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&icon_color=58a6ff&title_color=ffffff&text_color=c9d1d9" alt="hv33y Stats" height="150" />
  </a>
  <a href="https://github.com/hv33y">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hv33y&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=ffffff&text_color=c9d1d9" alt="Top Languages" height="150" />
  </a>
</p>

<p>Building custom interfaces, system automation, and browser extensions designed for speed, minimal overhead, and modern typography.</p>

<hr>

</div>

## Featured Deployments & Tools

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/hv33y/hvOS">hvOS</a></h3>
      <p>Transforms desktop YouTube into a high-performance Apple TV experience featuring fluid ambient lighting, pop-out focus search, and instantaneous load times.</p>
      <p><code>JavaScript</code> <code>Userscript</code> <code>UI/UX</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/hv33y/inline-b64-reveal">inline-b64-reveal</a></h3>
      <p>A lightweight userscript that automatically detects, decodes, and displays Base64 strings inline alongside a minimal UI and quick-copy functionality.</p>
      <p><code>JavaScript</code> <code>Automation</code> <code>DOM</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/hv33y/gemini-sweep">gemini-sweep</a></h3>
      <p>Automated cleanup utility for Google Gemini that purges unpinned conversations in sequence while keeping pinned threads intact.</p>
      <p><code>JavaScript</code> <code>Automation</code> <code>Workflow</code></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/hv33y/open-directory">open-directory</a></h3>
      <p>Fast web directory crawler and index explorer designed for quick resource discovery.</p>
      <p><code>HTML</code> <code>Search</code> <code>Index</code></p>
    </td>
  </tr>
</table>

<hr>

<div align="center">
  <sub>Maintained by <a href="https://github.com/hv33y">hv33y</a> • October 2026</sub>
</div>
