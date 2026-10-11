<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CODM AZK GHOST | Marketplace & Intermediario Seguro</title>
    <style>
        :root {
            --bg-dark: #07070c;
            --bg-card: #12121a;
            --border-color: #1f1f2e;
            --gaming-red: #ff2a4b;
            --gaming-gold: #ffd700;
            --gaming-violet: #a855f7;
            --text-main: #f3f4f6;
            --text-muted: #9ca3af;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; background-color: var(--bg-dark); color: var(--text-main); min-height: 100vh; display: flex; flex-direction: column; }
        
        /* Glow effects */
        .glow-red { text-shadow: 0 0 15px rgba(255, 42, 75, 0.6); }
        .glow-gold { text-shadow: 0 0 15px rgba(255, 215, 0, 0.6); }
        .glow-violet { text-shadow: 0 0 15px rgba(168, 85, 247, 0.6); }

        /* Header */
        header { position: sticky; top: 0; z-index: 50; background: rgba(7, 7, 12, 0.95); backdrop-filter: blur(10px); border-bottom: 1px solid var(--border-color); }
        .nav-container { max-width: 1200px; margin: 0 auto; padding: 0 20px; height: 80px; display: flex; align-items: center; justify-content: space-between; }
        .logo-box { display: flex; align-items: center; gap: 12px; }
        .logo-icon { width: 40px; height: 40px; border-radius: 12px; background: linear-gradient(135deg, var(--gaming-red), var(--gaming-violet)); display: flex; align-items: center; justify-content: center; color: white; font-size: 18px; box-shadow: 0 0 15px rgba(255,42,75,0.4); }
        .logo-text h1 { font-size: 20px; font-weight: 900; background: linear-gradient(90deg, var(--gaming-red), var(--gaming-violet), var(--gaming-gold)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
        .logo-text span { font-size: 10px; color: var(--gaming-gold); text-transform: uppercase; letter-spacing: 1px; display: block; font-weight: 700; }

        nav.desktop-nav { display: flex; gap: 20px; font-size: 13px; font-weight: 600; }
        nav.desktop-nav a { color: var(--text-main); text-decoration: none; transition: color 0.2s; }
        nav.desktop-nav a:hover { color: var(--gaming-red); }

        .header-actions { display: flex; gap: 12px; align-items: center; }
        .btn-admin { background: var(--bg-card); border: 1px solid rgba(168,85,247,0.5); color: var(--gaming-violet); padding: 8px 14px; border-radius: 10px; font-size: 12px; font-weight: 600; cursor: pointer; display: flex; align-items: center; gap: 6px; }
        .btn-whatsapp { background: linear-gradient(135deg, var(--gaming-red), var(--gaming-violet)); color: white; padding: 10px 16px; border-radius: 10px; font-size: 12px; font-weight: 700; text-decoration: none; display: flex; align-items: center; gap: 8px; box-shadow: 0 0 15px rgba(255,42,75,0.3); text-transform: uppercase; }

        /* Notice bar */
        .notice-bar { background: linear-gradient(90deg, var(--gaming-red), var(--gaming-violet), var(--gaming-gold)); color: #07070c; font-weight: 900; font-size: 12px; text-align: center; padding: 8px; letter-spacing: 1px; }

        /* Hero */
        .hero { padding: 80px 20px; text-align: center; background: linear-gradient(to bottom, var(--bg-card), var(--bg-dark)); border-bottom: 1px solid var(--border-color); }
        .hero h2 { font-size: clamp(28px, 5vw, 48px); font-weight: 900; line-height: 1.2; margin-bottom: 20px; }
        .hero p { max-width: 700px; margin: 0 auto 30px auto; color: var(--text-muted); font-size: 16px; line-height: 1.5; }
        .hero-buttons { display: flex; justify-content: center; gap: 16px; flex-wrap: wrap; }
        .btn-primary { background: var(--gaming-red); color: white; padding: 14px 28px; border-radius: 12px; font-weight: 800; font-size: 13px; text-decoration: none; box-shadow: 0 0 20px rgba(255,42,75,0.4); display: inline-flex; align-items: center; gap: 8px; cursor: pointer; border: none; }
        .btn-secondary { background: var(--bg-card); border: 1px solid rgba(255,215,0,0.5); color: var(--gaming-gold); padding: 14px 28px; border-radius: 12px; font-weight: 800; font-size: 13px; text-decoration: none; box-shadow: 0 0 15px rgba(255,215,0,0.2); display: inline-flex; align-items: center; gap: 8px; cursor: pointer; }

        /* Stats */
        .stats-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 16px; max-width: 900px; margin: 60px auto 0 auto; }
        .stat-card { background: rgba(18,18,26,0.8); border: 1px solid var(--border-color); padding: 20px; border-radius: 12px; text-align: center; }
        .stat-card .num { font-size: 24px; font-weight: 900; color: var(--gaming-gold); }
        .stat-card .label { font-size: 12px; color: var(--text-muted); margin-top: 4px; }

        /* Container */
        .container { max-width: 1200px; margin: 0 auto; padding: 40px 20px; width: 100%; flex-grow: 1; }

        /* Marketplace */
        .section-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 24px; flex-wrap: wrap; gap: 16px; }
        .section-title { font-size: 22px; font-weight: 900; display: flex; align-items: center; gap: 10px; }
        .filters { display: flex; gap: 12px; flex-wrap: wrap; }
        .search-input, .filter-select { background: var(--bg-card); border: 1px solid var(--border-color); color: white; padding: 10px 16px; border-radius: 10px; font-size: 14px; outline: none; }
        .search-input:focus, .filter-select:focus { border-color: var(--gaming-red); }

        .listings-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(320px, 1fr)); gap: 24px; }
        .listing-card { background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 16px; overflow: hidden; display: flex; flex-direction: column; justify-content: space-between; transition: border-color 0.3s; }
        .listing-card:hover { border-color: rgba(255,42,75,0.5); }
        .card-body { padding: 20px; }
        .card-badge { display: inline-block; padding: 4px 10px; border-radius: 20px; font-size: 10px; font-weight: 800; text-transform: uppercase; margin-bottom: 12px; }
        .badge-codm { background: rgba(255,42,75,0.15); color: var(--gaming-red); border: 1px solid rgba(255,42,75,0.3); }
        .badge-blood { background: rgba(168,85,247,0.15); color: var(--gaming-violet); border: 1px solid rgba(168,85,247,0.3); }
        .badge-free { background: rgba(255,215,0,0.15); color: var(--gaming-gold); border: 1px solid rgba(255,215,0,0.3); }
        
        .listing-title { font-size: 15px; font-weight: 800; margin-bottom: 8px; color: white; display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical; overflow: hidden; }
        .listing-desc { font-size: 12px; color: var(--text-muted); margin-bottom: 16px; line-height: 1.4; display: -webkit-box; -webkit-line-clamp: 3; -webkit-box-orient: vertical; overflow: hidden; }
        .listing-seller { font-size: 11px; color: var(--text-muted); display: flex; align-items: center; gap: 6px; }
        .listing-seller strong { color: white; }

        .card-footer { padding: 16px 20px; background: rgba(7,7,12,0.6); border-top: 1px solid var(--border-color); display: flex; align-items: center; justify-content: space-between; gap: 12px; }
        .price-tag .label { font-size: 9px; text-transform: uppercase; color: var(--text-muted); display: block; font-weight: 700; }
        .price-tag .val { font-size: 18px; font-weight: 900; color: var(--gaming-gold); }
        .btn-buy { background: linear-gradient(135deg, var(--gaming-red), var(--gaming-violet)); color: white; padding: 10px 14px; border-radius: 10px; font-size: 11px; font-weight: 800; text-decoration: none; display: flex; align-items: center; gap: 6px; box-shadow: 0 0 10px rgba(255,42,75,0.3); text-transform: uppercase; white-space: nowrap; }

        /* Sections */
        .section-box { background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 20px; padding: 30px; margin-top: 60px; }
        .form-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 16px; margin-bottom: 16px; }
        .form-group label { display: block; font-size: 12px; font-weight: 700; color: var(--text-muted); margin-bottom: 6px; }
        .form-control { width: 100%; background: var(--bg-dark); border: 1px solid var(--border-color); border-radius: 10px; padding: 12px; color: white; font-size: 14px; outline: none; }
        .form-control:focus { border-color: var(--gaming-gold); }
        textarea.form-control { resize: vertical; min-height: 90px; }

        /* Calculator */
        .calc-container { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; }
        @media(max-width: 768px) { .calc-container { grid-template-columns: 1fr; } }
        .calc-result-box { background: linear-gradient(135deg, rgba(168,85,247,0.15), var(--bg-dark)); border: 1px solid rgba(168,85,247,0.3); padding: 30px; border-radius: 16px; display: flex; flex-direction: column; justify-content: space-between; text-align: center; }
        .calc-result-box .price-display { font-size: 32px; font-weight: 900; color: white; margin: 20px 0; text-shadow: 0 0 20px rgba(168,85,247,0.6); }

        /* Services */
        .service-card { background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 16px; padding: 24px; display: flex; flex-direction: column; justify-content: space-between; }

        /* Modal */
        .modal-overlay { position: fixed; inset: 0; background: rgba(0,0,0,0.8); backdrop-filter: blur(5px); z-index: 100; display: none; align-items: center; justify-content: center; padding: 20px; }
        .modal-box { background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 16px; width: 100%; max-width: 400px; padding: 24px; position: relative; }
        .modal-close { position: absolute; top: 16px; right: 16px; background: none; border: none; color: var(--text-muted); font-size: 18px; cursor: pointer; }

        /* Footer */
        footer { background: var(--bg-card); border-top: 1px solid var(--border-color); margin-top: 80px; padding: 40px 20px; text-align: center; }
        .footer-content { max-width: 1200px; margin: 0 auto; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 20px; text-align: left; }
    </style>
</head>
<body>

    <div class="notice-bar">
        ⚡ 100% SEGURO CON INTERMEDIARIO OFICIAL • AZK GHOST (+58 422 475 7006) • CERO ESTAFAS ⚡
    </div>

    <header>
        <div class="nav-container">
            <div class="logo-box">
                <div class="logo-icon">👻</div>
                <div class="logo-text">
                    <h1>CODM AZK GHOST</h1>
                    <span>Marketplace & Escrow Oficial</span>
                </div>
            </div>

            <nav class="desktop-nav">
                <a href="#marketplace">Marketplace</a>
                <a href="#publicar">+ Publicar Cuenta</a>
                <a href="#valoracion">Calculadora Realista</a>
                <a href="#recargas">Recargas CP</a>
                <a href="#servicios">Recuperación</a>
            </nav>

            <div class="header-actions">
                <button onclick="openAdminModal()" class="btn-admin">🛡️ Panel Admin</button>
                <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20vengo%20de%20tu%20marketplace%20y%20quiero%20información." target="_blank" class="btn-whatsapp">💬 Soporte</a>
            </div>
        </div>
    </header>

    <section class="hero">
        <span style="display: inline-block; padding: 6px 16px; border-radius: 20px; background: rgba(168,85,247,0.1); border: 1px solid rgba(168,85,247,0.3); color: var(--gaming-violet); font-size: 11px; font-weight: 700; text-transform: uppercase; margin-bottom: 20px;">
            🛡️ Marketplace con Intermediario Garantizado
        </span>
        <h2>COMPRA, VENDE Y GESTIONA <br/>
            <span style="background: linear-gradient(90deg, var(--gaming-red), var(--gaming-gold), var(--gaming-violet)); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
                CON INTERMEDIARIO 100% SEGURO
            </span>
        </h2>
        <p>Publica tus cuentas de Call of Duty Mobile, Blood Strike, Free Fire y más. Tratos protegidos por AZK GHOST.</p>
        <div class="hero-buttons">
            <a href="#marketplace" class="btn-primary">🛒 Ver Catálogo de Cuentas</a>
            <a href="#publicar" class="btn-secondary">📤 Publicar Mi Cuenta Gratis</a>
        </div>

        <div class="stats-grid">
            <div class="stat-card">
                <div class="num">+500</div>
                <div class="label">Tratos Exitosos</div>
            </div>
            <div class="stat-card">
                <div class="num" style="color: var(--gaming-red);">100%</div>
                <div class="label">Protección Escrow</div>
            </div>
            <div class="stat-card">
                <div class="num" style="color: var(--gaming-violet);">24/7</div>
                <div class="label">Atención Directa</div>
            </div>
            <div class="stat-card">
                <div class="num">0 Estafas</div>
                <div class="label">Garantía AZK GHOST</div>
            </div>
        </div>
    </section>

    <div class="container" id="marketplace">
        <div class="section-header">
            <div>
                <h3 class="section-title">🛍️ MARKETPLACE OFICIAL</h3>
                <p style="font-size: 13px; color: var(--text-muted); margin-top: 4px;">Cuentas auditadas por el intermediario AZK GHOST.</p>
            </div>
            <div class="filters">
                <input type="text" id="searchInput" oninput="filterListings()" placeholder="Buscar..." class="search-input">
                <select id="gameFilter" onchange="filterListings()" class="filter-select">
                    <option value="ALL">Todos los Juegos</option>
                    <option value="CODM">Call of Duty Mobile</option>
                    <option value="Blood Strike">Blood Strike</option>
                    <option value="Free Fire">Free Fire</option>
                    <option value="Mobile Legends">Mobile Legends</option>
                </select>
            </div>
        </div>

        <div id="listingsGrid" class="listings-grid"></div>

        <!-- Publicar Cuenta (Estilo ZonaArthur / Mercado Libre) -->
        <div id="publicar" class="section-box">
            <div style="max-width: 600px; margin: 0 auto 30px auto; text-align: center;">
                <span style="color: var(--gaming-gold); font-size: 11px; font-weight: 700; text-transform: uppercase; background: rgba(255,215,0,0.1); padding: 4px 12px; border-radius: 20px;">Vende Seguro</span>
                <h3 style="font-size: 22px; font-weight: 800; margin-top: 10px;">Publica tu Cuenta en el Marketplace</h3>
                <p style="font-size: 13px; color: var(--text-muted); margin-top: 6px;">Envía tus datos y será publicada bajo la supervisión de AZK GHOST.</p>
            </div>

            <form id="publishForm" onsubmit="handlePublish(event)" style="max-width: 600px; margin: 0 auto;">
                <div class="form-grid">
                    <div class="form-group">
                        <label>Juego</label>
                        <select id="pubGame" required class="form-control">
                            <option value="CODM">Call of Duty Mobile</option>
                            <option value="Blood Strike">Blood Strike</option>
                            <option value="Free Fire">Free Fire</option>
                            <option value="Mobile Legends">Mobile Legends</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label>Título del Anuncio</label>
                        <input type="text" id="pubTitle" required placeholder="Ej: Cuenta Nivel 150 con 2 Míticas" class="form-control">
                    </div>
                </div>
                <div class="form-grid">
                    <div class="form-group">
                        <label>Precio (USD / USDT)</label>
                        <input type="number" id="pubPrice" required placeholder="Ej: 45" class="form-control">
                    </div>
                    <div class="form-group">
                        <label>Tu Número de WhatsApp</label>
                        <input type="text" id="pubWhatsapp" required placeholder="+58 412..." class="form-control">
                    </div>
                </div>
                <div class="form-group" style="margin-bottom: 16px;">
                    <label>Detalles e Inventario (Armas Míticas, Skins, Rango)</label>
                    <textarea id="pubDesc" required placeholder="Describe los detalles..." class="form-control"></textarea>
                </div>
                <button type="submit" class="btn-primary" style="width: 100%; justify-content: center; background: linear-gradient(135deg, var(--gaming-gold), var(--gaming-red)); color: var(--bg-dark);">
                    🚀 Enviar Cuenta para Aprobación de AZK GHOST
                </button>
            </form>
        </div>

        <!-- Calculadora Realista -->
        <div id="valoracion" class="section-box">
            <div style="max-width: 600px; margin: 0 auto 30px auto; text-align: center;">
                <span style="color: var(--gaming-violet); font-size: 11px; font-weight: 700; text-transform: uppercase; background: rgba(168,85,247,0.1); padding: 4px 12px; border-radius: 20px;">Calculadora Realista</span>
                <h3 style="font-size: 22px; font-weight: 800; margin-top: 10px;">Calculadora de Valor de Cuenta CODM</h3>
                <p style="font-size: 13px; color: var(--text-muted); margin-top: 6px;">Basada en la oferta y demanda real del mercado secundario actual.</p>
            </div>

            <div class="calc-container" style="max-width: 900px; margin: 0 auto;">
                <div style="background: rgba(7,7,12,0.5); padding: 24px; border-radius: 16px; border: 1px solid var(--border-color); display: flex; flex-direction: column; gap: 16px;">
                    <div class="form-group">
                        <label>Armas Míticas (Nivel Base / Max)</label>
                        <input type="number" id="calcMythics" min="0" value="0" oninput="calculateRealValue()" class="form-control">
                    </div>
                    <div class="form-group">
                        <label>Armas Legendarias</label>
                        <input type="number" id="calcLegendaries" min="0" value="0" oninput="calculateRealValue()" class="form-control">
                    </div>
                    <div class="form-group">
                        <label>Personajes Legendarios / Collabs</label>
                        <input type="number" id="calcChars" min="0" value="0" oninput="calculateRealValue()" class="form-control">
                    </div>
                    <div class="form-group">
                        <label>Camuflajes Especiales</label>
                        <select id="calcCamo" onchange="calculateRealValue()" class="form-control">
                            <option value="0">Ninguno</option>
                            <option value="15">Damascus / Oro Varios</option>
                            <option value="30">Diamond Múltiples</option>
                        </select>
                    </div>
                </div>

                <div class="calc-result-box">
                    <div>
                        <span style="font-size: 11px; text-transform: uppercase; color: var(--gaming-violet); font-weight: 700;">Valor Estimado de Mercado</span>
                        <div id="resultPrice" class="price-display">$15 - $25 USD</div>
                        <p style="font-size: 12px; color: var(--text-muted); line-height: 1.4;">Precio de reventa competitivo real. Las cuentas se deprecian respecto al gasto en ruletas.</p>
                    </div>
                    <a href="#publicar" class="btn-primary" style="justify-content: center; background: var(--gaming-violet); box-shadow: 0 0 15px rgba(168,85,247,0.4); margin-top: 20px;">
                        Vender con AZK GHOST
                    </a>
                </div>
            </div>
        </div>

        <!-- Recargas -->
        <div id="recargas" style="margin-top: 60px;">
            <div style="text-align: center; margin-bottom: 30px;">
                <span style="color: var(--gaming-gold); font-size: 11px; font-weight: 700; text-transform: uppercase; background: rgba(255,215,0,0.1); padding: 4px 12px; border-radius: 20px;">Tienda de Recargas</span>
                <h3 style="font-size: 22px; font-weight: 800; margin-top: 10px;">Recargas Oficiales & Servicios</h3>
            </div>

            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px;">
                <div class="service-card">
                    <div>
                        <div style="height: 100px; background: linear-gradient(135deg, var(--gaming-red), var(--bg-dark)); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 32px; margin-bottom: 16px;">🎯</div>
                        <h4 style="font-size: 15px; font-weight: bold; margin-bottom: 6px;">Call of Duty Mobile</h4>
                        <p style="font-size: 12px; color: var(--text-muted);">Recarga de CP 100% legal vía ID.</p>
                    </div>
                    <div style="margin-top: 20px;">
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20quiero%20recargar%20CP%20para%20CODM." target="_blank" class="btn-primary" style="width: 100%; justify-content: center; padding: 10px;">Recargar CP</a>
                    </div>
                </div>
                <div class="service-card">
                    <div>
                        <div style="height: 100px; background: linear-gradient(135deg, var(--gaming-violet), var(--bg-dark)); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 32px; margin-bottom: 16px;">💀</div>
                        <h4 style="font-size: 15px; font-weight: bold; margin-bottom: 6px;">Blood Strike</h4>
                        <p style="font-size: 12px; color: var(--text-muted);">Venta de cuentas y oro.</p>
                    </div>
                    <div style="margin-top: 20px;">
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20quiero%20comprar%20Oro%20o%20cuentas%20de%20Blood%20Strike." target="_blank" class="btn-primary" style="width: 100%; justify-content: center; padding: 10px; background: var(--gaming-violet);">Consultar</a>
                    </div>
                </div>
                <div class="service-card">
                    <div>
                        <div style="height: 100px; background: linear-gradient(135deg, var(--gaming-gold), var(--bg-dark)); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 32px; margin-bottom: 16px;">🔥</div>
                        <h4 style="font-size: 15px; font-weight: bold; margin-bottom: 6px;">Free Fire</h4>
                        <p style="font-size: 12px; color: var(--text-muted);">Diamantes y pases élite.</p>
                    </div>
                    <div style="margin-top: 20px;">
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20quiero%20diamantes%20de%20Free%20Fire." target="_blank" class="btn-primary" style="width: 100%; justify-content: center; padding: 10px; background: #f59e0b; color: var(--bg-dark);">Recargar</a>
                    </div>
                </div>
                <div class="service-card">
                    <div>
                        <div style="height: 100px; background: linear-gradient(135deg, #2563eb, var(--bg-dark)); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 32px; margin-bottom: 16px;">🎮</div>
                        <h4 style="font-size: 15px; font-weight: bold; margin-bottom: 6px;">Mobile Legends</h4>
                        <p style="font-size: 12px; color: var(--text-muted);">Diamantes y cuentas.</p>
                    </div>
                    <div style="margin-top: 20px;">
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20servicios%20de%20MLBB." target="_blank" class="btn-primary" style="width: 100%; justify-content: center; padding: 10px; background: #2563eb;">Ver Servicios</a>
                    </div>
                </div>
            </div>
        </div>

        <!-- Recuperación -->
        <div id="servicios" class="section-box">
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; align-items: center;">
                <div>
                    <span style="color: var(--gaming-red); font-size: 11px; font-weight: 700; text-transform: uppercase; background: rgba(255,42,75,0.1); padding: 4px 12px; border-radius: 20px;">Seguridad & Soporte</span>
                    <h3 style="font-size: 22px; font-weight: 800; margin-top: 10px;">Recuperación de Cuentas y Desvinculación</h3>
                    <p style="font-size: 13px; color: var(--text-muted); margin-top: 10px; line-height: 1.5;">¿Perdiste acceso o hay un hacker en tu cuenta de Activision, Facebook o Garena? AZK GHOST te ayuda a recuperarla.</p>
                    <div style="display: flex; gap: 12px; margin-top: 20px;">
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20necesito%20recuperar%20mi%20cuenta." target="_blank" class="btn-primary" style="padding: 10px 16px; font-size: 11px;">🔑 Recuperar Cuenta</a>
                    </div>
                </div>
                <div style="background: rgba(7,7,12,0.6); border: 1px solid var(--border-color); padding: 24px; border-radius: 16px; display: flex; flex-direction: column; gap: 12px; font-size: 13px;">
                    <div>✔ Desvinculación de Facebook / Line / Apple</div>
                    <div>✔ Soporte y restauración Activision ID</div>
                    <div>✔ Auditoría Antifraude para cuentas en venta</div>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <div class="footer-content">
            <div>
                <div style="font-weight: 900; font-size: 16px; background: linear-gradient(90deg, var(--gaming-red), var(--gaming-violet), var(--gaming-gold)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; margin-bottom: 6px;">CODM AZK GHOST</div>
                <p style="font-size: 12px; color: var(--text-muted);">Intermediario oficial en Venezuela. WhatsApp: +58 422 475 7006.</p>
            </div>
            <div style="font-size: 12px; color: var(--text-muted); text-align: center;">
                <p>© 2026 CODM AZK GHOST. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- Admin Modal -->
    <div id="adminModal" class="modal-overlay">
        <div class="modal-box">
            <button onclick="closeAdminModal()" class="modal-close">✕</button>
            <h3 style="font-size: 16px; font-weight: bold; margin-bottom: 16px; color: var(--gaming-violet);">🛡️ Panel Admin (AZK GHOST)</h3>
            <div id="adminLogin" style="display: flex; flex-direction: column; gap: 12px;">
                <p style="font-size: 12px; color: var(--text-muted);">Clave por defecto: <strong style="color:white;">azk2026</strong></p>
                <input type="password" id="adminPass" placeholder="••••••••" class="form-control">
                <button onclick="verifyAdmin()" class="btn-primary" style="justify-content: center; background: var(--gaming-violet);">Acceder</button>
            </div>
            <div id="adminPanelContent" style="display: none; flex-direction: column; gap: 12px;">
                <p style="font-size: 12px; color: var(--gaming-gold);">Sesión activa como Admin.</p>
                <button onclick="resetListings()" class="btn-primary" style="justify-content: center; background: var(--gaming-red);">Restaurar Anuncios</button>
                <button onclick="closeAdminModal()" class="form-control" style="background: var(--border-color); text-align: center; cursor: pointer; border: none; font-weight: bold;">Cerrar</button>
            </div>
        </div>
    </div>

    <script>
        let listings = [
            {
                id: 1,
                game: "CODM",
                title: "Cuenta Nivel 150 - 2 Míticas (M13 + Switchblade) + 8 Legendarias",
                price: 75,
                seller: "CarlosVzla",
                whatsapp: "+584120000000",
                desc: "Cuenta limpia Activision, nivel máximo, camuflajes y pase activo. Entrega inmediata con intermediario AZK GHOST.",
                verified: true
            },
            {
                id: 2,
                game: "Blood Strike",
                title: "Cuenta Veterana con Skins Exclusivas y Rango Striker Master",
                price: 35,
                seller: "GamerMaracay",
                whatsapp: "+584141111111",
                desc: "Correo limpio, sin baneos, excelente relación de bajas.",
                verified: true
            },
            {
                id: 3,
                game: "Free Fire",
                title: "Cuenta Veterana con Pase Élite Antiguo + Incubadoras",
                price: 40,
                seller: "JoseZulia",
                whatsapp: "+584242222222",
                desc: "Vinculada a VK limpio con acceso total a correo.",
                verified: true
            }
        ];

        if(localStorage.getItem('azk_listings')) {
            try { listings = JSON.parse(localStorage.getItem('azk_listings')); } catch(e) {}
        }

        function renderListings(items = listings) {
            const grid = document.getElementById('listingsGrid');
            if(items.length === 0) {
                grid.innerHTML = `<div style="grid-column: 1/-1; text-align: center; padding: 40px; color: var(--text-muted); font-size: 14px;">No se encontraron cuentas.</div>`;
                return;
            }

            grid.innerHTML = items.map(item => `
                <div class="listing-card">
                    <div class="card-body">
                        <div>
                            <span class="card-badge ${item.game === 'CODM' ? 'badge-codm' : item.game === 'Blood Strike' ? 'badge-blood' : 'badge-free'}">${item.game}</span>
                            <span style="font-size: 11px; color: var(--text-muted); float: right;">⭐ Verificado AZK</span>
                        </div>
                        <h4 class="listing-title">${item.title}</h4>
                        <p class="listing-desc">${item.desc}</p>
                        <div class="listing-seller">👤 Vendedor: <strong>${item.seller}</strong></div>
                    </div>
                    <div class="card-footer">
                        <div class="price-tag">
                            <span class="label">Intermediario</span>
                            <span class="val">$${item.price} <span style="font-size: 11px; font-weight: normal; color: var(--text-muted);">USD</span></span>
                        </div>
                        <a href="https://wa.me/584224757006?text=Hola%20AZK%20GHOST,%20estoy%20interesado%20en%20comprar%20la%20cuenta:%20${encodeURIComponent(item.title)}%20(Precio:%20$%${item.price}).%20Quiero%20hacer%20el%20trato%20con%20intermediario." target="_blank" class="btn-buy">
                            💬 Comprar con Intermediario
                        </a>
                    </div>
                </div>
            `).join('');
        }

        function filterListings() {
            const query = document.getElementById('searchInput').value.toLowerCase();
            const game = document.getElementById('gameFilter').value;
            const filtered = listings.filter(item => {
                const matchesQuery = item.title.toLowerCase().includes(query) || item.desc.toLowerCase().includes(query);
                const matchesGame = game === 'ALL' || item.game === game;
                return matchesQuery && matchesGame;
            });
            renderListings(filtered);
        }

        function handlePublish(e) {
            e.preventDefault();
            const newListing = {
                id: Date.now(),
                game: document.getElementById('pubGame').value,
                title: document.getElementById('pubTitle').value,
                price: parseFloat(document.getElementById('pubPrice').value),
                seller: "Usuario (Pendiente Verif)",
                whatsapp: document.getElementById('pubWhatsapp').value,
                desc: document.getElementById('pubDesc').value,
                verified: true
            };

            listings.unshift(newListing);
            localStorage.setItem('azk_listings', JSON.stringify(listings));
            renderListings();

            const msg = `Hola AZK GHOST, quiero publicar mi cuenta:%0A*Juego:* ${newListing.game}%0A*Título:* ${newListing.title}%0A*Precio:* $${newListing.price} USD%0A*WhatsApp:* ${newListing.whatsapp}%0A*Detalles:* ${newListing.desc}`;
            alert('¡Cuenta enviada! Se abrirá WhatsApp para enviar los detalles al intermediario.');
            window.open(`https://wa.me/584224757006?text=${msg}`, '_blank');
            document.getElementById('publishForm').reset();
        }

        function calculateRealValue() {
            const mythics = parseInt(document.getElementById('calcMythics').value) || 0;
            const legendaries = parseInt(document.getElementById('calcLegendaries').value) || 0;
            const chars = parseInt(document.getElementById('calcChars').value) || 0;
            const camoBonus = parseInt(document.getElementById('calcCamo').value) || 0;

            let base = 15;
            let total = base + (mythics * 25) + (legendaries * 8) + (chars * 12) + camoBonus;
            const minVal = Math.round(total * 0.9);
            const maxVal = Math.round(total * 1.2);

            document.getElementById('resultPrice').innerText = `$${minVal} - $${maxVal} USD`;
        }

        function openAdminModal() { document.getElementById('adminModal').style.display = 'flex'; }
        function closeAdminModal() { document.getElementById('adminModal').style.display = 'none'; }
        function verifyAdmin() {
            if(document.getElementById('adminPass').value === 'azk2026') {
                document.getElementById('adminLogin').style.display = 'none';
                document.getElementById('adminPanelContent').style.display = 'flex';
            } else { alert('Clave incorrecta (azk2026)'); }
        }
        function resetListings() { localStorage.removeItem('azk_listings'); location.reload(); }

        renderListings();
        calculateRealValue();
    </script>
</body>
</html>
