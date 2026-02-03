<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Palestra Gratuita para Times de Vendas | Tantra Restaurante</title>
  <meta name="description" content="Palestra gratuita (10h–11h30) para Diretores e Gerentes comerciais levarem seu time. Como criar uma experiência tão boa que o cliente não esquece, volta e indica." />

  <meta property="og:title" content="Palestra Gratuita para Times de Vendas | Tantra" />
  <meta property="og:description" content="Como criar uma experiência tão boa que o cliente não esquece, volta e indica. 10h–11h30. Vagas limitadas." />
  <meta property="og:type" content="website" />

  <style>
    :root{
      --bg: #0b0a08;
      --bg2:#12100c;
      --card:#14110c;
      --text:#f3efe6;
      --muted:#c9c2b3;
      --gold:#d8b36a;
      --gold2:#b48a3b;
      --line: rgba(216,179,106,.22);
      --shadow: 0 18px 60px rgba(0,0,0,.55);
      --radius: 18px;
      --radius2: 26px;
    }

    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Helvetica Neue", Helvetica, sans-serif;
      background:
        radial-gradient(1200px 600px at 20% 0%, rgba(216,179,106,.12), transparent 55%),
        radial-gradient(900px 600px at 80% 30%, rgba(216,179,106,.10), transparent 60%),
        linear-gradient(180deg, var(--bg) 0%, var(--bg2) 100%);
      color:var(--text);
      line-height:1.45;
    }

    a{ color:inherit; text-decoration:none; }
    .container{ width:min(1120px, 92vw); margin:0 auto; }

    /* Topbar */
    .topbar{
      position:sticky; top:0; z-index:50;
      backdrop-filter: blur(10px);
      background: rgba(11,10,8,.72);
      border-bottom:1px solid var(--line);
    }
    .topbar-inner{
      display:flex; align-items:center; justify-content:space-between;
      padding:14px 0;
      gap:16px;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
      font-weight:700; letter-spacing:.12em;
      text-transform:uppercase;
    }
    .brand-badge{
      width:38px; height:38px; border-radius:12px;
      background: linear-gradient(135deg, rgba(216,179,106,.32), rgba(180,138,59,.10));
      border:1px solid var(--line);
      display:grid; place-items:center;
      box-shadow: 0 10px 30px rgba(0,0,0,.35);
      font-weight:800;
      color:var(--gold);
    }
    .nav{
      display:flex; gap:14px; align-items:center;
      color:var(--muted);
      font-size:14px;
    }
    .nav a{
      padding:8px 10px; border-radius:999px;
      border:1px solid transparent;
    }
    .nav a:hover{
      border-color: var(--line);
      background: rgba(216,179,106,.06);
      color: var(--text);
    }

    /* Buttons */
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:10px;
      padding:12px 16px;
      border-radius:999px;
      border:1px solid var(--line);
      background: rgba(216,179,106,.08);
      color: var(--text);
      font-weight:650;
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
      box-shadow: 0 18px 45px rgba(216,179,106,.18);
    }
    .btn-primary:hover{
      filter: brightness(1.02);
      border-color: rgba(216,179,106,.75);
    }

    /* Hero */
    .hero{ padding:56px 0 28px; }
    .hero-grid{
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap:22px;
      align-items:stretch;
    }
    @media (max-width: 920px){ .hero-grid{ grid-template-columns: 1fr; } }

    .panel{
      background: linear-gradient(180deg, rgba(20,17,12,.86), rgba(20,17,12,.68));
      border:1px solid var(--line);
      border-radius: var(--radius2);
      box-shadow: var(--shadow);
    }
    .hero-left{ padding:28px; }
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
      margin:14px 0 12px;
      font-size: clamp(28px, 3.4vw, 44px);
      line-height:1.05;
      letter-spacing:-.02em;
    }
    .sub{
      margin:0;
      color: var(--muted);
      font-size: 16px;
      max-width: 62ch;
    }
    .hero-actions{
      display:flex; gap:12px; flex-wrap:wrap;
      margin-top:18px;
    }

    .bullets{
      margin-top:18px;
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:10px;
    }
    @media (max-width: 560px){ .bullets{ grid-template-columns:1fr; } }
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

    /* Right card (form) */
    .hero-right{ padding:22px; }
    .form-title{ font-weight:800; font-size:18px; margin:0 0 6px; }
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
    textarea{ min-height: 90px; resize: vertical; }

    .fineprint{
      margin:10px 0 0;
      color: rgba(201,194,179,.85);
      font-size:12px;
    }

    /* Sections */
    section{ padding: 22px 0; }
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
      box-shadow: 0 14px 40px rgba(0,0,0,.35);
    }
    .card h3{ margin:0 0 8px; font-size:16px; }
    .card p{ margin:0; color:var(--muted); font-size:14px; }

    /* Schedule block */
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
    .pill strong{ color: var(--text); font-weight:800; }

    /* Footer */
    footer{
      padding: 28px 0 40px;
      color: rgba(201,194,179,.85);
      border-top:1px solid var(--line);
      margin-top: 20px;
    }
    .footer-grid{
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:14px;
    }
    @media (max-width: 920px){ .footer-grid{ grid-template-columns:1fr; } }
    .small{ font-size:12px; line-height:1.5; }
    .muted{ color: rgba(201,194,179,.85); }

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
      width: 56px;
      height: 56px;
      border-radius: 999px;
      display: grid;
      place-items: center;
      z-index: 120;
      background: linear-gradient(135deg, rgba(216,179,106,.95), rgba(180,138,59,.88));
      border: 1px solid rgba(216,179,106,.55);
      box-shadow: 0 18px 55px rgba(0,0,0,.55);
      transition: transform .12s ease, filter .2s ease;
    }
    .wa-float:hover{ filter: brightness(1.03); transform: translateY(-1px); }
    .wa-float:active{ transform: translateY(1px); }

    .wa-float svg{
      width: 26px;
      height: 26px;
      fill: #1a1308;
    }

    .wa-hint{
      position: fixed;
      right: 84px;
      bottom: 28px;
      padding: 10px 12px;
      border-radius: 14px;
      border: 1px solid rgba(216,179,106,.22);
      background: rgba(10,9,7,.92);
      color: rgba(243,239,230,.92);
      font-size: 12px;
      box-shadow: 0 18px 55px rgba(0,0,0,.45);
      z-index: 119;
      max-width: 260px;
    }
    @media (max-width: 420px){
      .wa-hint{ display:none; }
    }
  </style>
</head>

<body>
  <!-- Topbar -->
  <div class="topbar">
    <div class="container topbar-inner">
      <div class="brand" aria-label="Tantra">
        <div class="brand-badge">T</div>
        <div>
          <div style="font-size:12px; color:var(--muted); letter-spacing:.18em;">TANTRA</div>
          <div style="font-size:14px; font-weight:800; letter-spacing:.06em;">Palestra para Times de Vendas</div>
        </div>
      </div>

      <div style="display:flex; gap:12px; align-items:center;">
        <nav class="nav" aria-label="Navegação">
          <a href="#como-funciona">Como funciona</a>
          <a href="#conteudo">Conteúdo</a>
          <a href="#local">Local</a>
          <a href="#inscricao">Inscrição</a>
        </nav>
        <a class="btn btn-primary" href="#inscricao">Reservar vaga</a>
      </div>
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
          <a class="btn" href="#como-funciona">Ver como funciona</a>
        </div>

        <div class="bullets" aria-label="Benefícios principais">
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Retenção</strong><br><span>Menos cliente “one-shot” e mais recorrência.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Indicação</strong><br><span>Experiência memorável vira conversa e recomendação.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Valor percebido</strong><br><span>Menos disputa por preço, mais preferência.</span></div></div>
          <div class="bullet"><div class="check">✓</div><div><strong style="color:var(--text)">Aplicável</strong><br><span>Ideias práticas para o dia a dia do vendedor.</span></div></div>
        </div>

        <p class="fineprint">
          * Vagas limitadas por data para manter a experiência focada (times pequenos funcionam melhor).
        </p>
      </div>

      <!-- Form -->
      <div class="panel hero-right" id="inscricao">
        <p class="form-title">Inscreva sua empresa (gratuito)</p>
        <p class="form-sub">Preencha abaixo para reservar a vaga do seu time. Você recebe confirmação por WhatsApp.</p>

        <!-- FORMSPREE -->
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
              <!-- Formspree precisa do campo email para reply -->
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

          <!-- Extras úteis -->
          <input type="hidden" id="utm_source" name="utm_source" value="">
          <input type="hidden" id="utm_campaign" name="utm_campaign" value="">
          <input type="hidden" id="page_url" name="page_url" value="">
          <input type="hidden" name="_subject" value="Nova inscrição - Palestra Tantra (Time de Vendas)">
          <!-- Opcional: redirecionar para uma página de obrigado (se você criar /thanks.html)
          <input type="hidden" name="_redirect" value="https://SEUUSUARIO.github.io/SEUREPO/thanks.html">
          -->

          <button class="btn btn-primary" type="submit">Enviar inscrição</button>

          <p class="fineprint">
            Ao enviar, sua empresa entra na lista de confirmação. O Eric confirma os detalhes por WhatsApp.
          </p>
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

  <!-- Conteúdo + Agenda -->
  <section id="conteudo">
    <div class="container schedule">
      <div class="card">
        <h2 class="section-title">O que seu time vai levar</h2>

        <div class="pill"><strong>Experiência</strong> que vira lembrança</div>
        <div class="pill"><strong>Percepção de valor</strong> sem desconto</div>
        <div class="pill"><strong>Fidelização</strong> e retorno</div>
        <div class="pill"><strong>Indicação</strong> e boca a boca</div>

        <p class="muted" style="margin-top:10px;">
          A lógica é simples: o cliente pode esquecer a proposta, mas raramente esquece
          como você fez ele se sentir. A palestra mostra como desenhar isso na prática.
        </p>
      </div>

      <div class="card">
        <h2 class="section-title">Agenda do encontro</h2>
        <p class="muted" style="margin:0 0 10px;">Formato pensado para times comerciais (dinâmico e direto).</p>

        <div class="pill"><strong>10:00</strong> • Abertura e contexto</div>
        <div class="pill"><strong>10:15</strong> • Método: “inesquecível por design”</div>
        <div class="pill"><strong>10:45</strong> • Exemplos aplicáveis para vendas</div>
        <div class="pill"><strong>11:10</strong> • Perguntas e próximos passos</div>

        <p class="fineprint">* Duração total: 1h30. Sem venda no meio. Só conteúdo e prática.</p>
      </div>
    </div>
  </section>

  <!-- Local -->
  <section id="local">
    <div class="container schedule">
      <div class="card">
        <h2 class="section-title">Local</h2>
        <p class="muted" style="margin:0 0 10px;">
          <strong>Tantra Restaurante</strong><br>
          Vila Olímpia • São Paulo
        </p>

        <p class="fineprint">* Após a inscrição, a confirmação e detalhes chegam pelo WhatsApp.</p>
      </div>

      <div class="card">
        <h2 class="section-title">Perguntas rápidas</h2>
        <p class="muted"><strong>Quanto custa?</strong> É gratuito.</p>
        <p class="muted"><strong>Precisa levar quantas pessoas?</strong> Recomendado de 5 a 15 (mas pode variar).</p>
        <p class="muted"><strong>Tem apresentação comercial?</strong> Não. O foco é conteúdo e experiência.</p>
        <p class="muted"><strong>Como escolho a data?</strong> Você sinaliza no formulário e confirmamos por WhatsApp.</p>
      </div>
    </div>
  </section>

  <footer>
    <div class="container footer-grid">
      <div>
        <div style="display:flex; align-items:center; gap:10px; margin-bottom:8px;">
          <div class="brand-badge" style="width:34px; height:34px;">T</div>
          <div style="font-weight:900; letter-spacing:.12em;">TANTRA</div>
        </div>
        <div class="small muted">
          © <span id="year"></span> • Página de inscrição (palestra gratuita)
        </div>
      </div>
      <div class="small muted">
        Dúvidas? Clique no WhatsApp e fale direto com o Eric.
        <br><br>
        <a class="btn" href="#inscricao">Voltar para inscrição</a>
      </div>
    </div>
  </footer>

  <div class="toast" id="toast"></div>

  <!-- WhatsApp floating button -->
  <div class="wa-hint">Fale com o Eric no WhatsApp</div>
  <a class="wa-float" id="waFloat" href="#" target="_blank" rel="noopener" aria-label="WhatsApp Eric">
    <!-- WhatsApp icon (svg) -->
    <svg viewBox="0 0 32 32" aria-hidden="true">
      <path d="M19.11 17.53c-.27-.14-1.6-.79-1.85-.88-.25-.09-.43-.14-.61.14-.18.27-.7.88-.86 1.06-.16.18-.32.2-.59.07-.27-.14-1.13-.42-2.15-1.33-.79-.71-1.33-1.58-1.49-1.85-.16-.27-.02-.42.12-.56.12-.12.27-.32.41-.48.14-.16.18-.27.27-.45.09-.18.05-.34-.02-.48-.07-.14-.61-1.47-.84-2.01-.22-.53-.45-.46-.61-.47-.16-.01-.34-.01-.52-.01-.18 0-.48.07-.73.34-.25.27-.95.93-.95 2.26 0 1.33.98 2.62 1.12 2.8.14.18 1.92 2.93 4.66 4.11.65.28 1.16.45 1.56.58.66.21 1.26.18 1.74.11.53-.08 1.6-.65 1.82-1.28.22-.63.22-1.17.16-1.28-.06-.11-.25-.18-.52-.32zM16.02 3C9.39 3 4 8.39 4 15.02c0 2.31.66 4.47 1.81 6.3L4 29l7.87-1.75c1.75.95 3.75 1.49 5.94 1.49C24.61 28.74 30 23.35 30 16.72 30 10.09 22.65 3 16.02 3zm0 23.6c-2.01 0-3.88-.57-5.47-1.56l-.39-.24-4.67 1.04.99-4.55-.25-.4a10.5 10.5 0 0 1-1.66-5.68c0-5.83 4.74-10.57 10.57-10.57S26.59 9.38 26.59 15.21c0 5.83-4.74 10.57-10.57 10.57z"/>
    </svg>
  </a>

  <script>
    // Ano automático
    document.getElementById("year").textContent = new Date().getFullYear();

    // Captura UTM + URL da página
    const params = new URLSearchParams(window.location.search);
    document.getElementById("utm_source").value = params.get("utm_source") || "";
    document.getElementById("utm_campaign").value = params.get("utm_campaign") || "";
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

    // Mini máscara WhatsApp
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

    // WhatsApp floating link (Eric)
    // Número: +55 11 99653-9632 -> wa.me/5511996539632
    const waNumber = "5511996539632";

    // Mensagem pré-preenchida (edite se quiser)
    const defaultMsg =
      "Oi Eric! Tudo bem? Acabei de ver a landing da palestra gratuita (10h–11h30) para times de vendas. " +
      "Queria confirmar detalhes e disponibilidade de datas para levar meu time.";

    const waLink = `https://wa.me/${waNumber}?text=${encodeURIComponent(defaultMsg)}`;
    document.getElementById("waFloat").href = waLink;
  </script>
</body>
</html>
