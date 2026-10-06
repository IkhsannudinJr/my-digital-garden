---
{"dg-publish":true,"permalink":"/02-areas/riset/kkn/dashboard-kkn/","title":"Dashboard KKN","dg-note-properties":{"title":"Dashboard KKN","date":"2026-09-22","tags":[],"status":"draft"}}
---

<div class="glass-grid-container"><span></span><div class="kkn-map-dashboard-card"><div class="kkn-map-header">
        <div class="kkn-map-title-group">
            <span class="kkn-map-icon">🗺️</span>
            <div>
                <h3 class="kkn-map-title">Peta Sebaran Lokasi KKN Kabupaten Wonogiri</h3>
                <p class="kkn-map-subtitle">Arahkan kursor pada PIN lokasi untuk melihat detail identitas KKN</p>
            </div>
        </div>
        <div class="kkn-map-actions">
            <span class="kkn-stat-badge">📍 15 Kecamatan Terisi (19 Titik)</span>
            <span class="kkn-stat-badge proses">🟠 1 Proses</span>
            <span class="kkn-stat-badge selesai">🟢 7 Selesai</span>
            <button class="kkn-map-mode-btn" type="button" title="Ganti tampilan peta">🛰️ Satelit Asli</button>
            <button class="kkn-map-toggle-btn" type="button">▲ Sembunyikan Peta</button>
        </div>
    </div><div class="kkn-map-stage"><img class="kkn-map-satellite-img" src="https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/export?bbox=110.68,-8.24,111.35,-7.63&amp;bboxSR=4326&amp;imageSR=4326&amp;size=1400,700&amp;format=jpg&amp;f=image" alt="Citra Satelit Kabupaten Wonogiri" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; object-fit: cover; border-radius: 10px; opacity: 0.92; filter: brightness(0.82) contrast(1.18) saturate(1.15); pointer-events: none; transition: opacity 0.35s; z-index: 1;"><img class="kkn-map-gmaps-img" src="https://server.arcgisonline.com/ArcGIS/rest/services/World_Street_Map/MapServer/export?bbox=110.68,-8.24,111.35,-7.63&amp;bboxSR=4326&amp;imageSR=4326&amp;size=1400,700&amp;format=jpg&amp;f=image" alt="Peta Jalan GMaps Kabupaten Wonogiri" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; object-fit: cover; border-radius: 10px; opacity: 0; filter: contrast(1.06) saturate(1.15) brightness(0.96); pointer-events: none; transition: opacity 0.35s; z-index: 1;"><div class="kkn-map-satellite-overlay" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border-radius: 10px; background: radial-gradient(circle at 45% 45%, rgba(10, 14, 22, 0.18) 0%, rgba(8, 10, 16, 0.65) 100%); pointer-events: none; transition: opacity 0.35s; z-index: 2;"></div><div class="kkn-map-svg-wrapper" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; pointer-events: none; z-index: 3; transition: opacity 0.35s; opacity: 0.45;">
    <svg class="kkn-map-svg-bg" viewBox="0 0 1000 500" preserveAspectRatio="none">
        <defs>
            <radialGradient id="lakeGlow" cx="50%" cy="50%" r="50%">
                <stop offset="0%" stop-color="rgba(6, 182, 212, 0.45)"></stop>
                <stop offset="100%" stop-color="rgba(6, 182, 212, 0.12)"></stop>
            </radialGradient>
            <filter id="neonGlow">
                <feGaussianBlur stdDeviation="3" result="coloredBlur"></feGaussianBlur>
                <feMerge>
                    <feMergeNode in="coloredBlur"></feMergeNode>
                    <feMergeNode in="SourceGraphic"></feMergeNode>
                </feMerge>
            </filter>
        </defs>
        
        <!-- Grid Koordinat Halus -->
        <g opacity="0.06" stroke="#ffffff" stroke-width="1">
            <line x1="200" y1="0" x2="200" y2="500"></line>
            <line x1="400" y1="0" x2="400" y2="500"></line>
            <line x1="600" y1="0" x2="600" y2="500"></line>
            <line x1="800" y1="0" x2="800" y2="500"></line>
            <line x1="0" y1="125" x2="1000" y2="125"></line>
            <line x1="0" y1="250" x2="1000" y2="250"></line>
            <line x1="0" y1="375" x2="1000" y2="375"></line>
        </g>

        <!-- Kontur Siluet Wilayah Wonogiri -->
        <path d="M 280 60 
                 C 450 40, 680 50, 890 70 
                 C 960 110, 960 180, 940 220 
                 C 950 260, 920 320, 800 340 
                 C 750 370, 680 390, 650 440 
                 C 550 420, 420 400, 370 450 
                 C 340 470, 240 480, 170 470 
                 C 120 440, 130 380, 180 320 
                 C 120 280, 70 230, 90 150 
                 C 140 120, 200 90, 280 60 Z" fill="rgba(255, 255, 255, 0.015)" stroke="rgba(255, 255, 255, 0.12)" stroke-width="1.5" stroke-dasharray="6 4"></path>

        <!-- Waduk Gajah Mungkur -->
        <path d="M 335 150 
                 C 365 190, 375 230, 360 270 
                 C 340 310, 310 295, 290 270 
                 C 280 235, 295 190, 315 160 Z" fill="url(#lakeGlow)" stroke="#06b6d4" stroke-width="1.5" filter="url(#neonGlow)"></path>
        
        <text x="330" y="225" fill="#22d3ee" font-size="10.5" font-weight="600" opacity="0.9" text-anchor="middle" letter-spacing="0.5">
            Waduk Gajah Mungkur
        </text>

        <!-- Garis Riak Air -->
        <ellipse cx="330" cy="245" rx="16" ry="6" fill="none" stroke="rgba(34, 211, 238, 0.4)" stroke-width="1"></ellipse>
    </svg>
    </div><div class="kkn-district-bg-dot" style="position: absolute; left: 23%; top: 50.5%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Eromoko</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 26.3%; top: 76.7%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Giritontro</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 51.1%; top: 54%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Batuwarno</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 42%; top: 43.3%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Nguntoronadi</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 61.8%; top: 16.3%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Girimarto</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 88.1%; top: 22.4%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Puhpelem</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 92.7%; top: 34.2%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Kismantoro</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 60.3%; top: 47.5%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Tirtomoyo</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 64.3%; top: 60.9%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Karangtengah</span></div><div class="kkn-district-bg-dot" style="position: absolute; left: 18.2%; top: 92%; transform: translate(-50%, -50%); pointer-events: none; opacity: 0.75; font-size: 9.5px; font-weight: 500; color: rgb(226, 232, 240); text-shadow: rgba(0, 0, 0, 0.9) 0px 1px 3px, rgba(0, 0, 0, 0.8) 0px 0px 6px; z-index: 4; display: flex; flex-direction: column; align-items: center; gap: 2px;"><span style="width:5px;height:5px;border-radius:50%;background:rgba(255,255,255,0.7);box-shadow:0 0 4px rgba(0,0,0,0.8);"></span><span>Paranggupito</span></div><div class="kkn-map-pin-anchor" style="left: 15.2%; top: 65.2%;"><div class="kkn-pin-beacon proses"></div><div class="kkn-pin-marker proses">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNY</span>
            
        </div><div class="kkn-pin-popover popover-align-left popover-align-top"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. PRACIMANTORO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNY</span>
                    <span class="kkn-popover-badge proses">Proses</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">22611</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Banaran; Desa Bulurejo; Desa Gerikikis; Desa Gebangharjo</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Dr. Banu Setyo Adi, M.Pd.</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">081249154670</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-10-12 s/d 2026-12-18</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 36%; top: 67.1%;"><div class="kkn-pin-beacon proses"></div><div class="kkn-pin-marker proses">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNY</span>
            
        </div><div class="kkn-pin-popover popover-align-top"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. GIRIWOYO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNY</span>
                    <span class="kkn-popover-badge proses">Proses</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">22611</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Banaran; Desa Bulurejo; Desa Gerikikis; Desa Gebangharjo</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Dr. Banu Setyo Adi, M.Pd.</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">081249154670</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-10-12 s/d 2026-12-18</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 88.2%; top: 15.8%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">STABN Wonogiri</span>
            
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. BULUKERTO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ STABN Wonogiri</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21871</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Krandegan</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Tri Yatno</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6285870418109</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-14 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 58.3%; top: 30.4%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">IPB</span>
            
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. SIDOHARJO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ IPB</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21308</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pingkuk; Desa Mojopuro; Desa Pesido; Desa Cangkring; Desa Sanggorng; Desa Jatirejo; Desa Tremes; Desa Kebon Agung; Desa Ngabeyan; Desa Sembukan; Desa Tempursari; Desa Jatinom; Desa Mojoreno; Desa Widoro; Desa Kedunggupit; Desa Sumpekerep; Kelurahan Sidoharjo; Kelurahan Kayuloko; Desa Manjung</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Handian Purwawangsa</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6281262106768</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-06 s/d 2026-08-14</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 71.3%; top: 31.6%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">IPB</span>
            
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. JATIROTO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ IPB</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21308</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pingkuk; Desa Mojopuro; Desa Pesido; Desa Cangkring; Desa Sanggorng; Desa Jatirejo; Desa Tremes; Desa Kebon Agung; Desa Ngabeyan; Desa Sembukan; Desa Tempursari; Desa Jatinom; Desa Mojoreno; Desa Widoro; Desa Kedunggupit; Desa Sumpekerep; Kelurahan Sidoharjo; Kelurahan Kayuloko; Desa Manjung</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Handian Purwawangsa</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6281262106768</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-06 s/d 2026-08-14</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 69.1%; top: 25.8%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">IPB, UGM 2</span>
            <span class="kkn-pin-count-badge">2</span>
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. JATISRONO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">2 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ IPB</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21308</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pingkuk; Desa Mojopuro; Desa Pesido; Desa Cangkring; Desa Sanggorng; Desa Jatirejo; Desa Tremes; Desa Kebon Agung; Desa Ngabeyan; Desa Sembukan; Desa Tempursari; Desa Jatinom; Desa Mojoreno; Desa Widoro; Desa Kedunggupit; Desa Sumpekerep; Kelurahan Sidoharjo; Kelurahan Kayuloko; Desa Manjung</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Handian Purwawangsa</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6281262106768</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-06 s/d 2026-08-14</span>
                    </div>
                </div>
            </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UGM 2</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21579</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pule;
Kelurahan Pelem;</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Muhammad Naufal Aljazari</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6285321569293</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-06-20 s/d 2026-08-09</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 33.5%; top: 22.4%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">IPB +1</span>
            <span class="kkn-pin-count-badge">2</span>
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. WONOGIRI</span>
            <span style="font-size:9.5px;color:var(--text-faint);">2 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ IPB</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21308</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pingkuk; Desa Mojopuro; Desa Pesido; Desa Cangkring; Desa Sanggorng; Desa Jatirejo; Desa Tremes; Desa Kebon Agung; Desa Ngabeyan; Desa Sembukan; Desa Tempursari; Desa Jatinom; Desa Mojoreno; Desa Widoro; Desa Kedunggupit; Desa Sumpekerep; Kelurahan Sidoharjo; Kelurahan Kayuloko; Desa Manjung</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Handian Purwawangsa</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6281262106768</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-06 s/d 2026-08-14</span>
                    </div>
                </div>
            </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ STAI Mulia Astuti</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">5837</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Jatipurno (Slogoretno), Wonogiri (Pokoh Kidul), Selogiri (Sendang Ijo)</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Amir Mukminin, S.Pd.I., M.Pd.</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">082223204552</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-20</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 30.1%; top: 15.5%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UGM 2 +2</span>
            <span class="kkn-pin-count-badge">3</span>
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. SELOGIRI</span>
            <span style="font-size:9.5px;color:var(--text-faint);">3 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UGM 2</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21579</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pule;
Kelurahan Pelem;</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Muhammad Naufal Aljazari</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">+6285321569293</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-06-20 s/d 2026-08-09</span>
                    </div>
                </div>
            </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNS</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21254</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Hery Widjianto</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">08122609524</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ STAI Mulia Astuti</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">5837</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Jatipurno (Slogoretno), Wonogiri (Pokoh Kidul), Selogiri (Sendang Ijo)</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Amir Mukminin, S.Pd.I., M.Pd.</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">082223204552</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-20</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 32.8%; top: 56.6%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNS</span>
            
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. BATURETNO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNS</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21254</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Hery Widjianto</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">08122609524</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 46.9%; top: 27.3%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNS</span>
            
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. NGADIROJO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNS</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21254</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Hery Widjianto</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">08122609524</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 25.1%; top: 39.5%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNS</span>
            
        </div><div class="kkn-pin-popover"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. WURYANTORO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNS</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21254</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Hery Widjianto</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">08122609524</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 92.6%; top: 27.8%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNS</span>
            
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. PURWANTORO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNS</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">21254</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Hery Widjianto</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">08122609524</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-21</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 9.5%; top: 31.4%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UNIVET</span>
            
        </div><div class="kkn-pin-popover popover-align-left"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. MANYARAN</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UNIVET</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">20873</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Desa Pijiharjo</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Ainur Komariah</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">081393456122</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-08-01 s/d 2026-09-15</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 75.2%; top: 13.7%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">STAI Mulia Astuti</span>
            
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. JATIPURNO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ STAI Mulia Astuti</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">5837</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Jatipurno (Slogoretno), Wonogiri (Pokoh Kidul), Selogiri (Sendang Ijo)</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Amir Mukminin, S.Pd.I., M.Pd.</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">082223204552</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-07-07 s/d 2026-08-20</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div><div class="kkn-map-pin-anchor" style="left: 78.2%; top: 25.1%;"><div class="kkn-pin-beacon selesai"></div><div class="kkn-pin-marker selesai">
            <span class="kkn-pin-icon">📍</span>
            <span class="kkn-pin-label">UGM 1</span>
            
        </div><div class="kkn-pin-popover popover-align-right"><div style="border-bottom: 1px solid rgba(255, 255, 255, 0.08); padding-bottom: 5px; display: flex; justify-content: space-between; align-items: center;">
            <span style="font-size:11px;font-weight:700;color:#60a5fa;">📍 KEC. SLOGOHIMO</span>
            <span style="font-size:9.5px;color:var(--text-faint);">1 Kegiatan KKN</span>
        </div><div class="kkn-popover-item">
                <div class="kkn-popover-item-head">
                    <span class="kkn-popover-ptn">🏛️ UGM 1</span>
                    <span class="kkn-popover-badge selesai">Selesai</span>
                </div>
                <div class="kkn-popover-meta">
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kode KKN:</span>
                        <span class="kkn-meta-val highlight">3814</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Lokasi Desa:</span>
                        <span class="kkn-meta-val">Setren &amp; Sokoboyo</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">PIC:</span>
                        <span class="kkn-meta-val">Elisa Dwi Rohani,
S.E., M.Sc</span>
                    </div>
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Kontak HP:</span>
                        <span class="kkn-meta-val">085932932705</span>
                    </div>
                    
                    <div class="kkn-meta-row">
                        <span class="kkn-meta-label">Periode:</span>
                        <span class="kkn-meta-val" style="font-size:9.5px;color:var(--text-muted);">2026-06-01 s/d 2026-08-01</span>
                    </div>
                </div>
            </div><div class="kkn-popover-hint">💡 Klik PIN untuk menyorot baris di tabel</div></div></div></div></div><div class="flex-grid-table"><div class="grid-row header-row"><div class="grid-cell th-cell th-kode">Kode</div><div class="grid-cell th-cell th-ptn">PTN</div><div class="grid-cell th-cell th-status">Status</div><div class="grid-cell th-cell th-pic">PIC</div><div class="grid-cell th-cell th-nohp">No. HP</div><div class="grid-cell th-cell th-kecamatan">Kecamatan</div><div class="grid-cell th-cell th-usulan">Usulan</div><div class="grid-cell th-cell th-buka">Buka</div><div class="grid-cell th-cell th-tutup">Tutup</div><div class="grid-cell th-cell th-tinjauan">Tinjauan</div><div class="grid-cell th-cell th-lokasi">Lokasi</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">22611</div><div class="grid-cell td-cell cell-ptn">UNY</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-proses"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Dr. Banu Setyo Adi, M.Pd.</div><div class="grid-cell td-cell cell-hp">081249154670</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-pracimantoro">Pracimantoro <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-giriwoyo">Giriwoyo <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Desa Banaran; Desa Bulurejo; Desa Gerikikis; Desa Gebangharjo</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">21871</div><div class="grid-cell td-cell cell-ptn">STABN Wonogiri</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Tri Yatno</div><div class="grid-cell td-cell cell-hp">+6285870418109</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-bulukerto">Bulukerto <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Desa Krandegan</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">21308</div><div class="grid-cell td-cell cell-ptn">IPB</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Handian Purwawangsa</div><div class="grid-cell td-cell cell-hp">+6281262106768</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-sidoharjo">Sidoharjo&nbsp; <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-jatiroto">jatiroto <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-jatisrono">jatisrono <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-wonogiri">Wonogiri <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Desa Pingkuk; Desa Mojopuro; Desa Pesido; Desa Cangkring; Desa Sanggorng; Desa Jatirejo; Desa Tremes; Desa Kebon Agung; Desa Ngabeyan; Desa Sembukan; Desa Tempursari; Desa Jatinom; Desa Mojoreno; Desa Widoro; Desa Kedunggupit; Desa Sumpekerep; Kelurahan Sidoharjo; Kelurahan Kayuloko; Desa Manjung</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">21579</div><div class="grid-cell td-cell cell-ptn">UGM 2</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Muhammad Naufal Aljazari</div><div class="grid-cell td-cell cell-hp">+6285321569293</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-jatisrono">jatisrono <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-selogiri">Selogiri <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Desa Pule;<br>Kelurahan Pelem;</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">21254</div><div class="grid-cell td-cell cell-ptn">UNS</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Hery Widjianto</div><div class="grid-cell td-cell cell-hp">08122609524</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-baturetno">Baturetno <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-ngadirojo">Ngadirojo <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-selogiri">Selogiri <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-wuryantoro">Wuryantoro <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-purwantoro">Purwantoro <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">1. Kec Baturetno, 2. Kec Ngadirojo, 3. Kec Selogiri, 4. Kec Wuryantoro, 5. Kec Purwantoro</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">20873</div><div class="grid-cell td-cell cell-ptn">UNIVET</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Ainur Komariah</div><div class="grid-cell td-cell cell-hp">081393456122</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-manyaran">Manyaran <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Desa Pijiharjo</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">5837</div><div class="grid-cell td-cell cell-ptn">STAI Mulia Astuti</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Amir Mukminin, S.Pd.I., M.Pd.</div><div class="grid-cell td-cell cell-hp">082223204552</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-jatipurno">jatipurno <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-wonogiri">Wonogiri <span class="capsule-remove">×</span></span><span class="seamless-kec-capsule kec-selogiri">Selogiri <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Jatipurno (Slogoretno), Wonogiri (Pokoh Kidul), Selogiri (Sendang Ijo)</div></div><div class="grid-row body-row"><div class="grid-cell td-cell cell-id">3814</div><div class="grid-cell td-cell cell-ptn">UGM 1</div><div class="grid-cell td-cell cell-status"><select class="glass-select-inline inline-status-selesai"><option value="Proses">Proses</option><option value="Selesai">Selesai</option><option value="Usulan">Usulan</option></select></div><div class="grid-cell td-cell cell-pic">Elisa Dwi Rohani,<br>S.E., M.Sc</div><div class="grid-cell td-cell cell-hp">085932932705</div><div class="grid-cell td-cell cell-kecamatan"><div class="inline-capsule-container"><div class="badge-row-flow"><span class="seamless-kec-capsule kec-slogohimo">Slogohimo <span class="capsule-remove">×</span></span></div><button class="add-capsule-btn">+</button></div></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-date"><input type="date" class="glass-date-input"></div><div class="grid-cell td-cell cell-tinjauan"><input type="text" class="glass-text-input-inline" placeholder="..."></div><div class="grid-cell td-cell cell-lokasi">Setren &amp; Sokoboyo</div></div></div></div>