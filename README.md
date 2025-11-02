<!doctype html>

<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Portfolio -- Chaldin Mulongo</title>
  <meta name="description" content="Portfolio professionnel -- Développeur web | UI/UX | Projets, compétences et contact." />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--muted:#94a3b8;--accent:#5eead4;--glass:rgba(255,255,255,0.04);--glass-2:rgba(255,255,255,0.02);font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;}
    *{box-sizing:border-box}html,body{height:100%;margin:0;background:linear-gradient(180deg,#071023 0%, #0b1220 100%);color:#e6eef8}
    .container{max-width:1100px;margin:32px auto;padding:28px}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:54px;height:54px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#60a5fa);display:flex;align-items:center;justify-content:center;font-weight:800;color:#052022}
    nav{display:flex;gap:12px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;font-weight:600;padding:8px 12px;border-radius:8px}
    nav a:hover{color:var(--accent);background:var(--glass)}
    .cta{background:linear-gradient(90deg,var(--accent),#60a5fa);color:#052022;padding:10px 14px;border-radius:10px;font-weight:700;text-decoration:none}/* Hero */
.hero{display:grid;grid-template-columns:1fr 380px;gap:28px;margin-top:28px;align-items:center}
.intro h1{font-size:clamp(28px,4.2vw,40px);margin:0 0 8px 0;line-height:1.02}
.eyebrow{color:var(--accent);font-weight:700;font-size:13px;letter-spacing:0.6px}
.lead{color:var(--muted);margin:12px 0 18px;max-width:62ch}
.buttons{display:flex;gap:12px}
.buttons a{padding:10px 14px;border-radius:10px;background:var(--glass);text-decoration:none;color:#dfeeff;font-weight:700}

.card{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);padding:18px;border-radius:14px;box-shadow:0 6px 18px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}
.profile{display:flex;gap:14px;align-items:center}
.avatar{width:84px;height:84px;border-radius:14px;background:linear-gradient(135deg,#1e293b,#0ea5a9);display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:800;color:#052022}
.meta h3{margin:0;font-size:18px}
.meta p{margin:4px 0 0;color:var(--muted);font-size:13px}

/* Skills & projects grid */
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:22px}
.skill-list{display:flex;flex-direction:column;gap:10px}
.skill-item{display:flex;justify-content:space-between;align-items:center;padding:10px;border-radius:10px;background:var(--glass-2);border:1px solid rgba(255,255,255,0.02)}
.progress{height:8px;background:rgba(255,255,255,0.04);border-radius:8px;width:100%;overflow:hidden;margin-top:8px}
.progress > i{display:block;height:100%;border-radius:8px;background:linear-gradient(90deg,var(--accent),#60a5fa)}

.projects{display:flex;flex-direction:column;gap:12px}
.project-card{display:flex;gap:12px;align-items:center;padding:12px;border-radius:12px;background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);border:1px solid rgba(255,255,255,0.03)}
.project-thumb{width:84px;height:56px;border-radius:8px;background:linear-gradient(135deg,#334155,#0ea5a9);display:flex;align-items:center;justify-content:center;font-weight:700}
.project-info h4{margin:0;font-size:16px}
.meta small{color:var(--muted)}

/* Experience & contact */
.two-col{display:grid;grid-template-columns:1fr 1fr;gap:18px;margin-top:22px}
.experience li{margin-bottom:12px}

form input,form textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}
form button{margin-top:8px;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#60a5fa);border:none;color:#052022;font-weight:700}

footer{margin-top:28px;text-align:center;color:var(--muted);font-size:13px}

/* Responsiveness */
@media (max-width:980px){.hero{grid-template-columns:1fr}.grid{grid-template-columns:repeat(2,1fr)}.two-col{grid-template-columns:1fr}}
@media (max-width:560px){.grid{grid-template-columns:1fr}.brand .logo{width:44px;height:44px}.container{padding:18px}}

/* micro interactions */
a,button{transition:all .2s ease}
.project-card:hover{transform:translateY(-6px)}

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">CM</div>
        <div>
          <div style="font-weight:800">Chaldin Mulongo</div>
          <div style="font-size:12px;color:var(--muted)">Développeur Web • UI/UX</div>
        </div>
      </div>
      <nav>
        <a href="#projets">Projets</a>
        <a href="#competences">Compétences</a>
        <a href="#experience">Expérience</a>
        <a href="#contact" class="cta">Contact</a>
      </nav>
    </header>

<section class="hero">
  <div>
    <div class="eyebrow">Bonjour -- je suis</div>
    <div class="intro">
      <h1>Chaldin Mulongo -- Développeur Web & UI/UX</h1>
      <p class="lead">Je conçois et développe des expériences web rapides, accessibles et esthétiques. Spécialisé en interfaces intuitives, performance front-end et intégration d'APIs. Je transforme des idées en produits digitaux utilisables et évolutifs.</p>
      <div class="buttons">
        <a href="#projets">Voir mes projets</a>
        <a href="#contact">Engager</a>
      </div>
    </div>

    <div class="grid">
      <div class="card">
        <h3 id="competences">Compétences</h3>
        <div class="skill-list">
          <div>
            <div class="skill-item"><strong>HTML &amp; CSS</strong><span>Expert</span></div>
            <div class="progress" aria-hidden><i style="width:95%"></i></div>
          </div>
          <div>
            <div class="skill-item"><strong>JavaScript (ES6+)</strong><span>Avancé</span></div>
            <div class="progress" aria-hidden><i style="width:85%"></i></div>
          </div>
          <div>
            <div class="skill-item"><strong>React / Next.js</strong><span>Intermédiaire</span></div>
            <div class="progress" aria-hidden><i style="width:70%"></i></div>
          </div>
          <div>
            <div class="skill-item"><strong>UI / Prototypage</strong><span>Avancé</span></div>
            <div class="progress" aria-hidden><i style="width:80%"></i></div>
          </div>
        </div>
      </div>

      <div class="card projects" id="projets">
        <h3>Projets récents</h3>

        <article class="project-card">
          <div class="project-thumb">K1</div>
          <div class="project-info">
            <h4>KinEcom -- MarketPlace</h4>
            <small class="meta">Plateforme e‑commerce • HTML/CSS/JS • API</small>
          </div>
        </article>

        <article class="project-card">
          <div class="project-thumb">UI</div>
          <div class="project-info">
            <h4>Dashboard Admin</h4>
            <small class="meta">Design UI/UX • Prototype • Accessibilité</small>
          </div>
        </article>

        <article class="project-card">
          <div class="project-thumb">TP</div>
          <div class="project-info">
            <h4>Outils pédagogiques</h4>
            <small class="meta">Exercices &amp; TP interactifs</small>
          </div>
        </article>

        <div style="margin-top:8px"><a href="#contact">Voir plus de projets →</a></div>
      </div>

      <div class="card">
        <h3>Profil</h3>
        <div class="profile">
          <div class="avatar">CM</div>
          <div class="meta">
            <h3>Chaldin Mulongo</h3>
            <p>Développeur Web -- Passionné par la performance front-end et l'UX. Disponible pour missions freelance et CDI.</p>
          </div>
        </div>
        <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap">
          <a class="cta" href="#">Télécharger CV</a>
          <a href="mailto:chaldinmulongo977@gmail.com">chaldinmulongo977@gmail.com</a>
        </div>
      </div>
    </div>
  </div>

  <aside>
    <div class="card">
      <h3>Contact rapide</h3>
      <p class="meta">Tu veux travailler avec moi ? Envoie un message.</p>
      <form id="contact" onsubmit="return contactSubmit(event)">
        <label class="sr-only">Nom</label>
        <input type="text" name="name" placeholder="Ton nom" required />
        <label class="sr-only">Email</label>
        <input type="email" name="email" placeholder="Ton email" required />
        <label class="sr-only">Message</label>
        <textarea name="message" rows="5" placeholder="Ton message" required></textarea>
        <button type="submit">Envoyer</button>
      </form>
    </div>

    <div class="card" style="margin-top:12px">
      <h4>Compétences techniques</h4>
      <p class="meta">HTML · CSS · JS · React · Next.js · Git · Figma · Accessibilité · SEO</p>
    </div>
  </aside>
</section>

<section class="two-col">
  <div class="card">
    <h3 id="experience">Expérience</h3>
    <ul class="experience">
      <li>
        <strong>Développeur Web -- Freelance</strong>
        <div class="meta"><small>2022 -- Présent • Projets e‑commerce, dashboards</small></div>
      </li>
      <li>
        <strong>Assistant pédagogique</strong>
        <div class="meta"><small>2021 -- 2022 • Conception d'exercices & TP</small></div>
      </li>
    </ul>
  </div>

  <div class="card">
    <h3>Services</h3>
    <ul>
      <li>Conception UI/UX & prototypage rapide</li>
      <li>Développement front‑end (HTML/CSS/JS)</li>
      <li>Intégration d'API & optimisation performance</li>
    </ul>
  </div>
</section>

<footer>
  <div>© <span id="year"></span> Chaldin Mulongo -- Tous droits réservés • <a href="#" style="color:var(--muted)">Mentions</a></div>
</footer>

  </div>  
<script>
  document.getElementById('year').textContent = new Date().getFullYear();

  function contactSubmit(e){
    e.preventDefault();
    const form = e.target;
    const data = new FormData(form);
    const name = data.get('name');
    const email = data.get('email');
    const message = data.get('message');
    const subject = encodeURIComponent('Contact portfolio -- ' + name);
    const body = encodeURIComponent(message + '\n\n' + name + ' -- ' + email);
    window.location.href = `mailto:chaldinmulongo977@gmail.com?subject=${subject}&body=${body}`;
    return false;
  }
</script>
</body>
</html>
