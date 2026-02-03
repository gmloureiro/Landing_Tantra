<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Palestra Gratuita para Times de Vendas | Tantra Restaurante</title>
  <meta name="description" content="Palestra gratuita (10h–11h30) para Diretores e Gerentes comerciais levarem seu time. Como criar uma experiência tão boa que o cliente não esquece, volta e indica." />

  <!-- FAVICON (arquivos no ROOT) -->
  <link rel="icon" href="favicon.ico" sizes="any">
  <link rel="icon" type="image/png" href="favicon-32.png" sizes="32x32">
  <link rel="icon" type="image/png" href="favicon-192.png" sizes="192x192">
  <link rel="apple-touch-icon" href="favicon-180.png">
  <meta name="theme-color" content="#0b0a08">

  <meta property="og:title" content="Palestra Gratuita para Times de Vendas | Tantra" />
  <meta property="og:description" content="Como criar uma experiência tão boa que o cliente não esquece, volta e indica. 10h–11h30. Vagas limitadas." />
  <meta property="og:type" content="website" />

  <style>
    :root{
      --bg: #0b0a08;
      --bg2:#12100c;
      --text:#f3efe6;
      --muted:#c9c2b3;
      --gold:#d8b36a;
      --gold2:#b48a3b;
      --line: rgba(216,179,106,.20);
      --shadow: 0 18px 60px rgba(0,0,0,.55);
      --radius: 18px;
      --radius2: 26px;
      --wa: #25D366;
    }

    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Helvetica Neue", Helvetica, sans-serif;
      background:
        radial-gradient(1200px 700px at 20% 0%, rgba(216,179,106,.10), transparent 56%),
        radial-gradient(900px 700px at 80% 35%, rgba(216,179,106,.08), transparent 62%),
        linear-gradient(180deg, var(--bg) 0%, var(--bg2) 100%);
      color:var(--text);
      line-height:1.45;
      overflow-x:hidden;
    }

    a{ color:inherit; text-decoration:none; }
    .container{ width:min(1100px, 92vw); margin:0 auto; }

    /* HEADER (mais bonito, sem “buracos”) */
    .topbar{
      position:sticky; top:0; z-index:50;
      backdrop-filter: blur(10px);
      background: rgba(11,10,8,.78);
      border-bottom:1px solid var(--line);
    }
    .topbar-inner{
      display:flex; align-items:center; justify-content:space-between;
      padding:14px 0;
      gap:14px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:12px;
      min-width: 220px;
    }
    .brand img{
      display:block;
      height:54px;
      width:auto;
    }

    .nav{
      display:flex;
      gap:10px;
      align-items:center;
      color:var(--muted);
      font-size:15px;
      flex-wrap:wrap;
      justify-content:flex-end;
    }
    .nav a{
      padding:8px 12px;
      border-radius:999px;
      border:1px solid transparent;
      transition:.2s;
    }
    .nav a:hover{
      border-color: var(--line);
      background: rgba(216,179,106,.06);
      color: var(--text);
    }

    @media (max-width: 860px){
      .nav{ display:none; }
      .brand{ min-width: unset; }
      .brand img{ height:48px; }
    }

    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:10px;
      padding:12px 16px;
      border-radius:999px;
      border:1px solid var(--line);
      background: rgba(216,179,106,.08);
      color: var(--text);
      font-weight:700;
      transition: transform .08s ease, background .2s ease, border-color .2s ease;
      cursor:pointer;
      user-select:none;
      white-space:nowrap;
    }
    .btn:hover{ background: rgba(216,179,106,.14); border-color: rgba(216,179,106,.35); }
    .btn:active{ transform: translateY(1px); }

    .btn-primary{
      background: linear-gradient(135deg, rgba(216,179,106,.95), rgba(180,138,59,.88));
      border-color: rgba(216,179,106,.55);
      color: #1a1308;
      box-shadow: 0 18px 45px rgba(216,179,106,.16);
    }

    /* HERO (centralizado + form logo no topo) */
    .hero{ padding: 34px 0 10px; }
    .hero-grid{
      display:grid;
      grid-template-columns: 1.05fr .95fr;
      gap:18px;
      align-items:stretch;
    }
    @media (max-width: 980px){
      .hero{ padding-top: 22px; }
      .hero-grid{ grid-template-columns: 1fr; }
    }

    .panel{
      background: linear-gradient(180deg, rgba(20,17,12,.86), rgba(20,17,12,.64));
      border:1px solid var(--line);
      border-radius: var(--radius2);
      box-shadow: var(--shadow);
    }

    .hero-left{ padding:26px; }
    .kicker{
      display:inline-flex; gap:10px; align-items:center;
      padding:8px 12px;
      border-radius:999px;
      border:1px solid var(--line);
      color: var(--muted);
      font-size:13px;
      background: rgba(216,179,106,.05);
    }
    .dot{
      width:8px; height:8px; border-radius:999px;
      background: var(--gold);
      box-shadow: 0 0 18px rgba(216,179,106,.35);
    }

    h1{
      margin:14px 0 10px;
      font-size: clamp(28px, 3.4vw, 44px);
      line-height:1.05;
      letter-spacing:-.02em;
    }

    .sub{
      margin:0;
      color: var(--muted);
      font-size: 16px;
      max-width: 64ch;
    }

    .hero-actions{
      display:flex; gap:12px; flex-wrap:wrap;
      margin-top:16px;
    }

    .bullets{
      margin-top:16px;
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:10px;
    }
    @media (max-width: 520px){ .bullets{ grid-template-columns:1fr; } }

    .bullet{
      display:flex; gap:10px; align-items:flex-start;
      padding:12px;
      border-radius: var(--radius);
      border:1px solid rgba(216,179,106,.18);
      background: rgba(11,10,8,.35);
      color: var(--muted);
      font-size:14px;
    }
    .check{
      width:22px; height:22px;
      border-radius: 8px;
      display:grid; place-items:center;
      color: #1a1308;
      background: linear-gradient(135deg, rgba(216,179,106,.95), rgba(180,138,59,.85));
      flex:0 0 auto;
      margin-top:1px;
      font-weight:900;
    }

    .hero-right{ padding:22px; }
    .form-title{ font-weight:900; font-size:18px; margin:0 0 6px; }
    .form-sub{ margin:0 0 14px; color:var(--muted); font-size:14px; }

    form{ display:grid; gap:10px; }
    .row2{ display:grid; gap:10px; grid-template-columns:1fr 1fr; }
    @media (max-width: 520px){ .row2{ grid-template-columns:1fr; } }

    label{ font-size:12px; color:var(--muted); }
    input, select, textarea{
      width:100%;
      padding:12px 12px;
      border-radius: 14px;
      border:1px solid rgba(216,179,106,.18);
      background: rgba(0,0,0,.22);
      color: var(--text);
      outline:none;
    }
    input:focus, select:focus, textarea:focus{
      border-color: rgba(216,179,106,.45);
      box-shadow: 0 0 0 4px rgba(216,179,106,.10);
    }
    textarea{ min-height: 84px; resize: vertical; }

    .fineprint{
      margin:10px 0 0;
      color: rgba(201,194,179,.85);
      font-size:12px;
    }

    /* SEÇÕES (sem “buracos”) */
    section{ padding: 18px 0; }
    .section-title{
      margin:0 0 10px;
      font-size: 20px;
      letter-spacing:-.01em;
    }

    .grid3{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
    }
    @media (max-width: 920px){ .grid3{ grid-template-columns:1fr; } }

    .card{
      padding:18px;
      border-radius: var(--radius2);
      border:1px solid var(--line);
      background: rgba(20,17,12,.55);
      box-shadow: 0 14px 40px rgba(0,0,0,.32);
    }
    .card h3{ margin:0 0 8px; font-size:16px; }
    .card p{ margin:0; color:var(--muted); font-size:14px; }

    .schedule{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:12px;
    }
    @media (max-width: 920px){ .schedule{ grid-template-columns:1fr; } }

    .pill{
      display:inline-flex; align-items:center; gap:10px;
      padding:10px 12px;
      border-radius: 999px;
      border:1px solid rgba(216,179,106,.22);
      background: rgba(216,179,106,.06);
      color: var(--muted);
      font-size: 13px;
      margin: 0 8px 8px 0;
    }
    .pill strong{ color: var(--text); font-weight:900; }

    /* GALERIA */
    .gallery-grid{
      display:grid;
      grid-template-columns: repeat(4, 1fr);
      gap:12px;
    }
    @media (max-width: 980px){ .gallery-grid{ grid-template-columns: repeat(3, 1fr); } }
    @media (max-width: 700px){ .gallery-grid{ grid-template-columns: repeat(2, 1fr); } }
    @media (max-width: 440px){ .gallery-grid{ grid-template-columns: 1fr; } }

    .g-item{
      position:relative;
      border-radius: 18px;
      overflow:hidden;
      border:1px solid rgba(216,179,106,.20);
      background: rgba(0,0,0,.18);
      cursor:pointer;
      min-height: 150px;
    }
    .g-item img{
      width:100%;
      height:100%;
      display:block;
      object-fit: cover;
      transform: scale(1.01);
      transition: transform .25s ease, filter .25s ease;
      filter: saturate(1.03) contrast(1.03);
    }
    .g-item:hover img{ transform: scale(1.06); filter: saturate(1.08) contrast(1.06); }
    .g-badge{
      position:absolute;
      left:10px; bottom:10px;
      padding:8px 10px;
      border-radius: 999px;
      border:1px solid rgba(255,255,255,.16);
      background: rgba(10,9,7,.75);
      font-size:12px;
      color: rgba(243,239,230,.92);
      backdrop-filter: blur(6px);
    }

    /* Lightbox */
    .lightbox{
      position:fixed; inset:0;
      background: rgba(0,0,0,.82);
      display:none;
      place-items:center;
      z-index: 200;
      padding: 18px;
    }
    .lightbox.open{ display:grid; }
    .lightbox-inner{
      width:min(1100px, 94vw);
      border-radius: 18px;
      overflow:hidden;
      border:1px solid rgba(216,179,106,.28);
      background: rgba(10,9,7,.92);
      box-shadow: 0 22px 80px rgba(0,0,0,.65);
      position:relative;
    }
    .lightbox-inner img{ width:100%; height:auto; display:block; }
    .lb-close{
      position:absolute;
      top:10px; right:10px;
      width:40px; height:40px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,.20);
      background: rgba(0,0,0,.35);
      color: rgba(243,239,230,.95);
      cursor:pointer;
      display:grid;
      place-items:center;
      font-size:18px;
    }

    /* Footer */
    footer{
      padding: 24px 0 40px;
      color: rgba(201,194,179,.85);
      border-top:1px solid var(--line);
      margin-top: 10px;
    }
    .footer-grid{
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:14px;
    }
    @media (max-width: 920px){ .footer-grid{ grid-template-columns:1fr; } }
    .small{ font-size:12px; line-height:1.5; }

    /* Toast */
    .toast{
      position: fixed;
      right: 16px;
      bottom: 16px;
      max-width: 360px;
      padding: 14px 14px;
      border-radius: 16px;
      border: 1px solid rgba(216,179,106,.28);
      background: rgba(10,9,7,.92);
      box-shadow: 0 20px 70px rgba(0,0,0,.55);
      color: var(--text);
      display:none;
      z-index: 100;
    }
    .toast strong{ color: var(--gold); }

    /* Floating WhatsApp */
    .wa-float{
      position: fixed;
      right: 18px;
      bottom: 18px;
      width: 60px;
      height: 60px;
      border-radius: 999px;
      display: grid;
      place-items: center;
      z-index: 120;
      background: var(--wa);
      border: 1px solid rgba(255,255,255,.18);
      box-shadow: 0 18px 55px rgba(0,0,0,.55);
      transition: transform .12s ease, filter .2s ease;
    }
    .wa-float:hover{ filter: brightness(1.03); transform: translateY(-1px); }
    .wa-float:active{ transform: translateY(1px); }
    .wa-float img{ width:30px; height:30px; display:block; }

    .wa-hint{
      position: fixed;
      right: 92px;
      bottom: 30px;
      padding: 10px 12px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.18);
      background: rgba(10,9,7,.92);
      color: rgba(243,239,230,.92);
      font-size: 12px;
      box-shadow: 0 18px 55px rgba(0,0,0,.45);
      z-index: 119;
      max-width: 260px;
    }
    @media (max-width: 420px){ .wa-hint{ display:none; } }
  </style>
</head>

<body>
  <!-- Header -->
  <div class="topbar">
    <div class="container topbar-inner">
      <div class="brand" aria-label="Restaurante Tantra">
        <img
          src="tantra-logo-clean-400.webp"
          srcset="tantra-logo-clean-400.webp 400w, tantra-logo-clean-800.webp 800w, tantra-logo-clean-1200.webp 1200w"
          sizes="(max-width: 520px) 160px, 220px"
          alt="Restaurante Tantra – Mongolian Grill"
        />
      </div>

      <nav class="nav" aria-label="Navegação">
        <a href="#inscricao">Inscrição</a>
        <a href="#como-funciona">Como funciona</a>
        <a href="#conteudo">Conteúdo</a>
        <a href="#galeria">Galeria</a>
        <a href="#local">Local</a>
      </nav>

      <a class="btn btn-primary" href="#inscricao">Reservar vaga</a>
    </div>
  </div>

  <!-- Hero -->
  <header class="hero">
    <div class="container hero-grid">

      <div class="panel hero-left">
        <div class="kicker"><span class="dot"></span> Encontro gratuito • 10h–11h30 • Times comerciais</div>
        <h1>Como fazer o cliente <span style="color:var(--gold);">não esquecer</span> da sua empresa</h1>
        <p class="sub">
          Uma palestra prática para <strong>Diretores e Gerentes Comerciais</strong> levarem seu time
          e aprenderem como criar uma experiência que gera <strong>lembrança, retorno e indicação</strong>.
        </p>

        <div class="hero-actions">
          <a class="btn btn-primary" href="#inscricao">Quero levar meu time</a>
          <a class="btn" href="#conteudo">Ver conteúdo</a>
        </div>

        <div class="bullets">
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Retenção</strong><br><span>Menos cliente “one-shot” e mais recorrência.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Indicação</strong><br><span>Experiência memorável vira conversa e recomendação.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Valor percebido</strong><br><span>Menos disputa por preço, mais preferência.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Aplicável</strong><br><span>Ideias práticas para o dia a dia do vendedor.</span></div></div>
        </div>

        <p class="fineprint">* Vagas limitadas por data para manter a experiência focada (times pequenos funcionam melhor).</p>
      </div>

      <!-- Form (logo no início do site) -->
      <div class="panel hero-right" id="inscricao">
        <p class="form-title">Inscreva sua empresa (gratuito)</p>
        <p class="form-sub">Preencha abaixo para reservar a vaga do seu time. Você recebe confirmação por WhatsApp.</p>

        <form id="leadForm" action="https://formspree.io/f/mzdvqaen" method="POST">
          <div class="row2">
            <div>
              <label for="nome">Nome</label>
              <input id="nome" name="nome" placeholder="Seu nome" required />
            </div>
            <div>
              <label for="cargo">Cargo</label>
              <input id="cargo" name="cargo" placeholder="Diretor/Gerente Comercial" required />
            </div>
          </div>

          <div class="row2">
            <div>
              <label for="empresa">Empresa</label>
              <input id="empresa" name="empresa" placeholder="Nome da empresa" required />
            </div>
            <div>
              <label for="tamanho_time">Quantas pessoas?</label>
              <select id="tamanho_time" name="tamanho_time" required>
                <option value="" disabled selected>Selecione</option>
                <option>3 a 5</option>
                <option>6 a 10</option>
                <option>11 a 15</option>
                <option>16+</option>
              </select>
            </div>
          </div>

          <div class="row2">
            <div>
              <label for="whats">WhatsApp (com DDD)</label>
              <input id="whats" name="whats" placeholder="(11) 9xxxx-xxxx" required />
            </div>
            <div>
              <label for="email">E-mail corporativo</label>
              <input id="email" name="email" type="email" placeholder="voce@empresa.com" required />
            </div>
          </div>

          <div class="row2">
            <div>
              <label for="data">Data desejada</label>
              <select id="data" name="data" required>
                <option value="" disabled selected>Escolha uma data</option>
                <option>Próxima Semana (a combinar)</option>
                <option>Quinzenal (a combinar)</option>
                <option>Outra (informar abaixo)</option>
              </select>
            </div>
            <div>
              <label for="horario">Horário</label>
              <input id="horario" name="horario" value="10:00 – 11:30" readonly />
            </div>
          </div>

          <div>
            <label for="observacoes">Observações (opcional)</label>
            <textarea id="observacoes" name="observacoes" placeholder="Ex.: queremos focar em retenção, indicação, pós-venda, etc."></textarea>
          </div>

          <input type="hidden" id="page_url" name="page_url" value="">
          <input type="hidden" name="_subject" value="Nova inscrição - Palestra Tantra (Time de Vendas)">

          <button class="btn btn-primary" type="submit">Enviar inscrição</button>

          <p class="fineprint">Ao enviar, sua empresa entra na lista de confirmação. O Eric confirma os detalhes por WhatsApp.</p>
        </form>
      </div>

    </div>
  </header>

  <!-- Como funciona -->
  <section id="como-funciona">
    <div class="container">
      <h2 class="section-title">Como funciona</h2>
      <div class="grid3">
        <div class="card">
          <h3>1) Você inscreve sua empresa</h3>
          <p>Escolhe o tamanho do time e indica a melhor data (semanal/quinzenal). A inscrição é gratuita.</p>
        </div>
        <div class="card">
          <h3>2) Confirmação por WhatsApp</h3>
          <p>Após o cadastro, o Eric entra em contato para confirmar e alinhar os detalhes do encontro.</p>
        </div>
        <div class="card">
          <h3>3) Palestra prática (10h–11h30)</h3>
          <p>Conteúdo aplicável para vendas: como criar experiência que fixa a marca e aumenta recorrência/indicação.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Conteúdo -->
  <section id="conteudo">
    <div class="container schedule">
      <div class="card">
        <h2 class="section-title">O que seu time vai levar</h2>
        <div class="pill"><strong>Experiência</strong> que vira lembrança</div>
        <div class="pill"><strong>Percepção de valor</strong> sem desconto</div>
        <div class="pill"><strong>Fidelização</strong> e retorno</div>
        <div class="pill"><strong>Indicação</strong> e boca a boca</div>
        <p style="margin-top:10px; color:var(--muted);">
          O cliente pode esquecer a proposta, mas raramente esquece como você fez ele se sentir.
          A palestra mostra como desenhar isso na prática.
        </p>
      </div>

      <div class="card">
        <h2 class="section-title">Agenda do encontro</h2>
        <p style="margin:0 0 10px; color:var(--muted);">Formato pensado para times comerciais (dinâmico e direto).</p>
        <div class="pill"><strong>10:00</strong> • Abertura e contexto</div>
        <div class="pill"><strong>10:15</strong> • Método: “inesquecível por design”</div>
        <div class="pill"><strong>10:45</strong> • Exemplos aplicáveis para vendas</div>
        <div class="pill"><strong>11:10</strong> • Perguntas e próximos passos</div>
        <p class="fineprint">* Duração total: 1h30. Sem venda no meio. Só conteúdo e prática.</p>
      </div>
    </div>
  </section>

  <!-- Galeria -->
  <section id="galeria">
    <div class="container">
      <h2 class="section-title">Galeria • O clima do Tantra</h2>
      <p style="margin:0 0 12px; color:var(--muted);">Clique nas fotos para ampliar.</p>

      <div class="gallery-grid">
        <div class="g-item" data-full="tantra-gallery-1-1600.webp"><img src="tantra-gallery-1-450.webp" srcset="tantra-gallery-1-450.webp 450w, tantra-gallery-1-900.webp 900w, tantra-gallery-1-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - ambiente" loading="lazy"><div class="g-badge">Ambiente</div></div>
        <div class="g-item" data-full="tantra-gallery-2-1600.webp"><img src="tantra-gallery-2-450.webp" srcset="tantra-gallery-2-450.webp 450w, tantra-gallery-2-900.webp 900w, tantra-gallery-2-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - chapa" loading="lazy"><div class="g-badge">Chapa</div></div>
        <div class="g-item" data-full="tantra-gallery-3-1600.webp"><img src="tantra-gallery-3-450.webp" srcset="tantra-gallery-3-450.webp 450w, tantra-gallery-3-900.webp 900w, tantra-gallery-3-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - jardim" loading="lazy"><div class="g-badge">Jardim</div></div>
        <div class="g-item" data-full="tantra-gallery-4-1600.webp"><img src="tantra-gallery-4-450.webp" srcset="tantra-gallery-4-450.webp 450w, tantra-gallery-4-900.webp 900w, tantra-gallery-4-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - prato" loading="lazy"><div class="g-badge">Prato</div></div>
        <div class="g-item" data-full="tantra-gallery-5-1600.webp"><img src="tantra-gallery-5-450.webp" srcset="tantra-gallery-5-450.webp 450w, tantra-gallery-5-900.webp 900w, tantra-gallery-5-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - salão" loading="lazy"><div class="g-badge">Salão</div></div>
        <div class="g-item" data-full="tantra-gallery-6-1600.webp"><img src="tantra-gallery-6-450.webp" srcset="tantra-gallery-6-450.webp 450w, tantra-gallery-6-900.webp 900w, tantra-gallery-6-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - buffet" loading="lazy"><div class="g-badge">Buffet</div></div>
        <div class="g-item" data-full="tantra-gallery-7-1600.webp"><img src="tantra-gallery-7-450.webp" srcset="tantra-gallery-7-450.webp 450w, tantra-gallery-7-900.webp 900w, tantra-gallery-7-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - bar" loading="lazy"><div class="g-badge">Bar</div></div>
        <div class="g-item" data-full="tantra-gallery-8-1600.webp"><img src="tantra-gallery-8-450.webp" srcset="tantra-gallery-8-450.webp 450w, tantra-gallery-8-900.webp 900w, tantra-gallery-8-1600.webp 1600w" sizes="(max-width:700px) 48vw, (max-width:980px) 32vw, 23vw" alt="Tantra - lounge" loading="lazy"><div class="g-badge">Lounge</div></div>
      </div>
    </div>
  </section>

  <!-- Local -->
  <section id="local">
    <div class="container schedule">
      <div class="card">
        <h2 class="section-title">Local</h2>
        <p style="margin:0 0 10px; color:var(--muted);">
          <strong>Tantra Restaurante</strong><br>
          Vila Olímpia • São Paulo
        </p>
        <p class="fineprint">* Após a inscrição, a confirmação e detalhes chegam pelo WhatsApp.</p>
      </div>

      <div class="card">
        <h2 class="section-title">Perguntas rápidas</h2>
        <p style="color:var(--muted); margin:0 0 6px;"><strong>Quanto custa?</strong> É gratuito.</p>
        <p style="color:var(--muted); margin:0 0 6px;"><strong>Quantas pessoas?</strong> Recomendado de 5 a 15 (pode variar).</p>
        <p style="color:var(--muted); margin:0 0 6px;"><strong>Tem apresentação comercial?</strong> Não. O foco é conteúdo e experiência.</p>
        <p style="color:var(--muted); margin:0;"><strong>Como escolho a data?</strong> Você sinaliza no formulário e confirmamos por WhatsApp.</p>
      </div>
    </div>
  </section>

  <footer>
    <div class="container footer-grid">
      <div>
        <img
          src="tantra-logo-transparent-400.webp"
          srcset="tantra-logo-transparent-400.webp 400w, tantra-logo-transparent-800.webp 800w, tantra-logo-transparent-1200.webp 1200w"
          sizes="160px"
          alt="Tantra Restaurante"
          style="height:40px; width:auto; opacity:.95; margin-bottom:8px;"
        />
        <div class="small">© <span id="year"></span> • Página de inscrição (palestra gratuita)</div>
      </div>
      <div class="small">
        Dúvidas? Clique no WhatsApp e fale direto com o Eric.
        <br><br>
        <a class="btn" href="#inscricao">Voltar para inscrição</a>
      </div>
    </div>
  </footer>

  <div class="toast" id="toast"></div>

  <!-- Lightbox -->
  <div class="lightbox" id="lightbox" aria-hidden="true">
    <div class="lightbox-inner">
      <button class="lb-close" id="lbClose" aria-label="Fechar">✕</button>
      <img id="lbImg" src="" alt="Foto ampliada">
    </div>
  </div>

  <!-- Whats -->
  <div class="wa-hint">Fale com o Eric no WhatsApp</div>
  <a class="wa-float" id="waFloat" href="#" target="_blank" rel="noopener" aria-label="WhatsApp Eric">
    <img src="whatsapp-icon-64.png" alt="WhatsApp" />
  </a>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
    document.getElementById("page_url").value = window.location.href;

    // Smooth scroll
    document.querySelectorAll('a[href^="#"]').forEach(a => {
      a.addEventListener("click", (e) => {
        const href = a.getAttribute("href");
        const target = document.querySelector(href);
        if (!target) return;
        e.preventDefault();
        target.scrollIntoView({ behavior: "smooth", block: "start" });
      });
    });

    // Máscara WhatsApp input
    const whats = document.getElementById("whats");
    whats.addEventListener("input", () => {
      let v = whats.value.replace(/\D/g, "").slice(0, 11);
      if (v.length <= 2) whats.value = v ? `(${v}` : "";
      else if (v.length <= 7) whats.value = `(${v.slice(0,2)}) ${v.slice(2)}`;
      else whats.value = `(${v.slice(0,2)}) ${v.slice(2,7)}-${v.slice(7)}`;
    });

    // Toast
    const form = document.getElementById("leadForm");
    const toast = document.getElementById("toast");
    function showToast(msg){
      toast.innerHTML = msg;
      toast.style.display = "block";
      setTimeout(() => toast.style.display = "none", 5200);
    }
    form.addEventListener("submit", () => {
      showToast("<strong>Enviado!</strong> Se os dados estiverem corretos, você receberá confirmação por WhatsApp.");
    });

    // WhatsApp (Eric): +55 11 99653-9632 => 5511996539632
    const waNumber = "5511996539632";
    const defaultMsg =
      "Oi Eric! Tudo bem? Acabei de ver a landing da palestra gratuita (10h–11h30) para times de vendas. " +
      "Queria confirmar detalhes e disponibilidade de datas para levar meu time.";
    document.getElementById("waFloat").href = `https://wa.me/${waNumber}?text=${encodeURIComponent(defaultMsg)}`;

    // Lightbox (galeria)
    const lb = document.getElementById("lightbox");
    const lbImg = document.getElementById("lbImg");
    const lbClose = document.getElementById("lbClose");

    document.querySelectorAll(".g-item").forEach(item => {
      item.addEventListener("click", () => {
        const full = item.getAttribute("data-full");
        lbImg.src = full;
        lb.classList.add("open");
        lb.setAttribute("aria-hidden", "false");
      });
    });

    function closeLb(){
      lb.classList.remove("open");
      lb.setAttribute("aria-hidden", "true");
      lbImg.src = "";
    }
    lbClose.addEventListener("click", closeLb);
    lb.addEventListener("click", (e) => { if (e.target === lb) closeLb(); });
    document.addEventListener("keydown", (e) => { if (e.key === "Escape") closeLb(); });
  </script>
</body>
</html>

