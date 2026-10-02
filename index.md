---
layout: default
title: "hv33y | Developer, Automation & Systems"
description: "Personal site and project directory for hv33y. Custom user interfaces, Cloudflare automations, Tampermonkey userscripts, and lightweight developer utilities."
keywords: "hv33y, hvOS, automation, userscripts, cloudflare workers, github pages"
author: "hv33y"
robots: "index, follow"
---

<style>
  /* 1. Hide the default GitHub Pages generated header */
  header, .page-header { display: none !important; }
  
  /* 2. Force Dark Mode & Typography (Overrides GitHub's Default Theme) */
  body, .markdown-body {
    background-color: #0d1117 !important;
    color: #c9d1d9 !important;
    font-family: 'Google Sans', -apple-system, BlinkMacSystemFont, sans-serif !important;
  }
  
  /* 3. Fix the broken white tables from the screenshot */
  .markdown-body table, .markdown-body table tr, .markdown-body table td {
    background-color: #0d1117 !important;
    border: 1px solid #30363d !important;
    color: #c9d1d9 !important;
  }
  
  .markdown-body a { color: #58a6ff !important; text-decoration: none; }
  .markdown-body a:hover { text-decoration: underline; }
  .markdown-body hr { border-top: 1px solid #30363d !important; background: transparent; }
  .markdown-body code { background: rgba(110,118,129,0.4) !important; color: #c9d1d9 !important; border-radius: 4px; padding: 2px 6px; }

  /* 4. Light Mode Class (Triggered by the JS Button) */
  body.light-mode, body.light-mode .markdown-body, body.light-mode .markdown-body table tr, body.light-mode .markdown-body table td {
    background-color: #ffffff !important;
    color: #24292f !important;
    border-color: #d0d7de !important;
  }
  body.light-mode .markdown-body a { color: #0969da !important; }
  body.light-mode .markdown-body code { background: rgba(175,184,193,0.2) !important; color: #24292f !important; }
  body.light-mode .markdown-body hr { border-top: 1px solid #d0d7de !important; }
  
  /* 5. Button Styling */
  #theme-toggle {
    position: fixed; top: 20px; right: 20px;
    background: transparent; border: 1px solid #30363d;
    color: #c9d1d9; padding: 5px 10px; border-radius: 5px;
    cursor: pointer; font-family: 'Google Sans'; z-index: 100;
  }
  body.light-mode #theme-toggle {
    border-color: #d0d7de; color: #24292f;
  }
</style>

<!-- Theme Toggle Button & Script -->
<button id="theme-toggle">Toggle Light Mode</button>
<script>
  const toggleBtn = document.getElementById('theme-toggle');
  toggleBtn.addEventListener('click', () => {
    // Toggles the class instead of checking inline styles
    document.body.classList.toggle('light-mode');
    
    // Update button text
    if (document.body.classList.contains('light-mode')) {
      toggleBtn.innerText = 'Toggle Dark Mode';
    } else {
      toggleBtn.innerText = 'Toggle Light Mode';
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
  <p>
    <a href="mailto:your.email@example.com">Email</a> &nbsp;•&nbsp;
    <a href="https://t.me/your_telegram">Telegram</a> &nbsp;•&nbsp;
    <a href="https://github.com/hv33y">GitHub</a>
  </p>
  <sub>Maintained by <a href="https://github.com/hv33y">hv33y</a> • October 2026</sub>
</div>
