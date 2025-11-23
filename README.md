# srikandi-automotive
<!doctype html>

<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Hubungan Cepat — WhatsApp · Instagram · Maps</title>
  <meta name="description" content="Halaman sederhana untuk mengarahkan pengunjung ke WhatsApp, Instagram, dan Maps." />
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--accent:#06b6d4;--muted:#94a3b8;--white:#ffffff}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;display:flex;align-items:center;justify-content:center;min-height:100vh;background:linear-gradient(180deg,#071027 0%,#081226 100%);color:var(--white)}
    .container{width:min(720px,94%);background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:14px;padding:28px;box-shadow:0 8px 30px rgba(2,6,23,0.7);}
    header{display:flex;gap:16px;align-items:center}
    .logo{width:60px;height:60px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700}
    h1{margin:0;font-size:20px}
    p{margin:6px 0 18px;color:var(--muted)}
    .links{display:grid;grid-template-columns:1fr;gap:12px}
    .btn{display:flex;gap:12px;align-items:center;padding:14px 16px;border-radius:10px;text-decoration:none;font-weight:600;background:linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.04)}
    .btn svg{width:28px;height:28px;flex-shrink:0}
    .btn .meta{display:flex;flex-direction:column;font-size:14px}
    .btn .meta .label{color:var(--white)}
    .btn .meta .sub{color:var(--muted);font-size:13px;margin-top:2px}
    .whatsapp{border-left:4px solid #25D366}
    .instagram{border-left:4px solid #C13584}
    .maps{border-left:4px solid #4285F4}
    footer{margin-top:18px;font-size:13px;color:var(--muted);text-align:center}
    @media(min-width:520px){.links{grid-template-columns:repeat(3,1fr)}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <img src="logo.png" alt="Logo Srikandi Automotif" style="width:120px; height:auto; border-radius:12px; margin-right:16px;">
      <div class="logo">LH</div>
      <div>
        <h1>Hub Link Cepat</h1>
        <p>Buka WhatsApp, Instagram, atau Lokasi Maps dengan satu ketukan.</p>
      </div>
    </header><div class="links" style="margin-top:12px">
  <!-- WhatsApp: ganti PHONENUM dengan nomor internasional tanpa tanda + atau spasi (contoh: 6281234567890). -->
  <a class="btn whatsapp" id="whatsappBtn" href="https://wa.me/6282141170080?text=Halo%20saya%20tertarik%20dengan%20produk%20Anda" target="_blank" rel="noopener">
    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M20.52 3.48A11.92 11.92 0 0012 .12C5.56.12.84 4.84.84 11.28c0 1.98.52 3.9 1.5 5.6L.12 23.88l7.32-1.92a11.1 11.1 0 005.46 1.32h.06c6.44 0 11.16-4.72 11.16-11.16 0-3-1.16-5.82-3.54-7.68z" fill="#25D366"/></svg>
    <div class="meta"><span class="label">WhatsApp</span><span class="sub">Chat & Pesan langsung</span></div>
  </a>

  <!-- Instagram: ganti USERNAME dengan username Instagram tanpa @ -->
  <a class="btn instagram" id="instagramBtn" href="https://instagram.com/srikandiautomotive" target="_blank" rel="noopener">
    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><rect x="2" y="2" width="20" height="20" rx="5" stroke="#C13584" stroke-width="1.5" fill="none"/><path d="M15.5 8.5a3 3 0 11-6 0 3 3 0 016 0zM17.8 6.2l.01.01" stroke="#C13584" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.4"/></svg>
    <div class="meta"><span class="label">Instagram</span><span class="sub">Lihat katalog & feed</span></div>
  </a>

  <!-- Maps: link yang kamu berikan dimasukkan di bawah -->
  <a class="btn maps" id="mapsBtn" href="https://maps.app.goo.gl/osYeddFMxHLtbBds9" target="_blank" rel="noopener">
    <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2C8.1 2 5 5.1 5 9c0 5.3 7 13 7 13s7-7.7 7-13c0-3.9-3.1-7-7-7z" stroke="#4285F4" stroke-width="1.4" fill="none"/><circle cx="12" cy="9" r="2.2" stroke="#4285F4" stroke-width="1.2" fill="none"/></svg>
    <div class="meta"><span class="label">Maps</span><span class="sub">Arah ke lokasi toko</span></div>
  </a>
</div>

<footer>
  <footer>
  Terhubung langsung ke WhatsApp, Instagram, dan Maps.
</footer>

  </div>  <!-- Simple script to help preview / replace placeholders quickly -->  <script>
    // If you want to pre-fill links dynamically, change these variables below:
    const phone = '';
    const insta = '';
    // If left empty, placeholders remain.
    if(phone){
      const wa = document.getElementById('whatsappBtn');
      wa.href = `https://wa.me/${phone}?text=${encodeURIComponent('Halo saya tertarik dengan produk Anda')}`;
    }
    if(insta){
      document.getElementById('instagramBtn').href = `https://instagram.com/${insta}`;
    }
  </script></body>
</html>
