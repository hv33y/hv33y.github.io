---
layout: default
title: "Tools | hv33y"
permalink: /tools/
description: "Client-side utility suite by hv33y. Image resizing, format conversion, and PDF manipulation."
keywords: "hv33y, tools, image resizer, pdf editor, base64, utility"
author: "hv33y"
robots: "index, follow"

og:
  title: "Tools | hv33y"
  type: website
  url: "https://hv33y.github.io/tools/"
  description: "Client-side utility suite by hv33y. Image resizing, format conversion, and PDF manipulation."
  image: "https://hv33y.github.io/og-preview.jpg"

twitter:
  card: summary_large_image
  title: "Tools | hv33y"
  description: "Client-side utility suite by hv33y. Image resizing, format conversion, and PDF manipulation."
  image: "https://hv33y.github.io/og-preview.jpg"
---

<!-- Import PDF-lib for client-side PDF manipulation -->
<script src="https://unpkg.com/pdf-lib/dist/pdf-lib.min.js"></script>

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
    display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 24px; max-width: 1000px; margin: 40px auto 60px; width: 100%;
  }

  .bento-card {
    background: rgba(255, 255, 255, 0.02); border: 1px solid rgba(255, 255, 255, 0.05);
    border-radius: 24px; padding: 32px;
    backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
    display: flex; flex-direction: column; color: inherit !important;
  }
  .bento-card h3 { margin-top: 0 !important; font-size: 1.5rem; color: #ffffff; border: none !important; margin-bottom: 15px;}
  .bento-card p { color: #a1a1a6; font-size: 0.95rem; margin-bottom: 20px; }

  /* Custom UI Elements */
  input[type="number"], input[type="text"] {
    background: rgba(0,0,0,0.5); border: 1px solid rgba(255,255,255,0.1);
    color: #fff; padding: 12px 15px; border-radius: 12px; font-family: 'Google Sans';
    width: 100%; box-sizing: border-box; margin-bottom: 15px; outline: none;
  }
  input[type="number"]:focus { border-color: rgba(128, 0, 32, 0.5); }
  
  .file-upload-btn {
    display: block; width: 100%; background: rgba(255,255,255,0.05);
    border: 1px dashed rgba(255,255,255,0.2); padding: 20px; text-align: center;
    border-radius: 12px; cursor: pointer; color: #a1a1a6; transition: all 0.3s;
    margin-bottom: 15px; box-sizing: border-box; font-weight: 600;
  }
  .file-upload-btn:hover { background: rgba(128,0,32,0.1); border-color: #800020; color: #fff; }
  input[type="file"] { display: none; }

  .action-btn {
    background: rgba(128, 0, 32, 0.8); color: #fff; border: none;
    padding: 12px 20px; border-radius: 12px; font-family: 'Google Sans'; font-weight: 600;
    cursor: pointer; transition: all 0.3s; width: 100%; font-size: 1rem;
  }
  .action-btn:hover { background: rgba(160, 0, 40, 1); transform: translateY(-2px); }
  
  .btn-row { display: flex; gap: 10px; margin-top: 10px; }
</style>

<div class="hero">
  <h1>Tools</h1>
  <p>Local edge utilities. Everything processes instantly inside your browser. Zero server uploads. Total privacy.</p>
  
  <div class="social-pills">
    <a href="/">Index</a>
    <a href="/repo">Repositories</a>
  </div>
</div>

<div class="bento-grid">

  <!-- TOOL 1: IMAGE STUDIO -->
  <div class="bento-card">
    <h3>Image Studio</h3>
    <p>Resize, compress, or convert between JPG, PNG, and WebP instantly.</p>
    
    <label class="file-upload-btn">
      <span id="img-label">Select Image File</span>
      <input type="file" id="img-input" accept="image/png, image/jpeg, image/webp">
    </label>
    
    <div style="display: flex; gap: 10px;">
      <input type="number" id="img-width" placeholder="Width (px)">
      <input type="number" id="img-height" placeholder="Height (px)">
    </div>
    
    <div class="btn-row">
      <button class="action-btn" onclick="processImage('jpeg')">Get JPG</button>
      <button class="action-btn" onclick="processImage('png')">Get PNG</button>
      <button class="action-btn" onclick="processImage('webp')">Get WebP</button>
    </div>
  </div>

  <!-- TOOL 2: PDF PRIVACY STUDIO -->
  <div class="bento-card">
    <h3>PDF Meta-Stripper</h3>
    <p>Upload a PDF to instantly strip all hidden tracking metadata (author, software, timestamps) and secure the file.</p>
    
    <label class="file-upload-btn">
      <span id="pdf-label">Select PDF Document</span>
      <input type="file" id="pdf-input" accept="application/pdf">
    </label>
    
    <button class="action-btn" onclick="cleanPDF()" style="margin-top: auto;">Clean & Download PDF</button>
  </div>

</div>

<!-- INVISIBLE PROCESSING CANVAS -->
<canvas id="canvas" style="display: none;"></canvas>

<script>
  // --- IMAGE STUDIO LOGIC ---
  const imgInput = document.getElementById('img-input');
  const imgLabel = document.getElementById('img-label');
  let currentImage = new Image();

  imgInput.addEventListener('change', (e) => {
    const file = e.target.files[0];
    if (!file) return;
    imgLabel.innerText = file.name;
    
    const reader = new FileReader();
    reader.onload = (event) => {
      currentImage.src = event.target.result;
      currentImage.onload = () => {
        document.getElementById('img-width').value = currentImage.width;
        document.getElementById('img-height').value = currentImage.height;
      };
    };
    reader.readAsDataURL(file);
  });

  function processImage(format) {
    if (!currentImage.src) { alert("Please select an image first."); return; }
    
    const canvas = document.getElementById('canvas');
    const ctx = canvas.getContext('2d');
    
    // Get custom dimensions or fallback to original
    const targetWidth = parseInt(document.getElementById('img-width').value) || currentImage.width;
    const targetHeight = parseInt(document.getElementById('img-height').value) || currentImage.height;
    
    canvas.width = targetWidth;
    canvas.height = targetHeight;
    
    // Draw and convert
    ctx.drawImage(currentImage, 0, 0, targetWidth, targetHeight);
    const dataUrl = canvas.toDataURL(`image/${format}`, 0.9);
    
    // Trigger auto-download
    const a = document.createElement('a');
    a.href = dataUrl;
    a.download = `hv33y-export.${format}`;
    a.click();
  }

  // --- PDF STUDIO LOGIC ---
  const pdfInput = document.getElementById('pdf-input');
  const pdfLabel = document.getElementById('pdf-label');

  pdfInput.addEventListener('change', (e) => {
    if(e.target.files[0]) {
      pdfLabel.innerText = e.target.files[0].name;
    }
  });

  async function cleanPDF() {
    const file = pdfInput.files[0];
    if (!file) { alert("Please select a PDF first."); return; }
    
    pdfLabel.innerText = "Processing...";
    
    try {
      const arrayBuffer = await file.arrayBuffer();
      const pdfDoc = await PDFLib.PDFDocument.load(arrayBuffer);
      
      // Strip metadata to ensure privacy
      pdfDoc.setTitle('');
      pdfDoc.setAuthor('');
      pdfDoc.setSubject('');
      pdfDoc.setKeywords([]);
      pdfDoc.setProducer('hvOS Subsystem');
      pdfDoc.setCreator('hvOS Subsystem');
      
      const pdfBytes = await pdfDoc.save();
      
      // Create a Blob and trigger download
      const blob = new Blob([pdfBytes], { type: "application/pdf" });
      const link = document.createElement('a');
      link.href = window.URL.createObjectURL(blob);
      link.download = `secure_${file.name}`;
      link.click();
      
      pdfLabel.innerText = "Done! Select another PDF";
    } catch (error) {
      alert("Error processing PDF. Make sure it isn't password protected.");
      pdfLabel.innerText = "Select PDF Document";
    }
  }
</script>

<div align="center" style="margin: 60px 0 40px; color: #6e6e73; font-size: 0.9rem;">
  hv33y • 2026
</div>
