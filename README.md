/* Стиль сайту — коментарі українською, редагуй за потреби */
:root{
  --blue:#0b66c3;
  --yellow:#ffd400;
  --bg-gradient: linear-gradient(135deg, #0b66c3 0%, #4aa3ff 40%, #ffd400 100%);
  --max-width:980px;
  --radius:12px;
  --accent: #ffd400;
  --text:#0b2340;
}
*{box-sizing:border-box}
body{
  margin:0;
  font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  color:var(--text);
  background: var(--bg-gradient);
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  min-height:100vh;
  display:flex;
  flex-direction:column;
}
.container{max-width:var(--max-width);margin:0 auto;padding:0 20px;}
.site-header{background:transparent;padding:18px 0;color:white}
.header-inner{display:flex;align-items:center;justify-content:space-between;gap:12px}
.brand{display:flex;align-items:center;gap:12px;text-decoration:none;color:inherit}
.logo{width:84px;height:84px;object-fit:cover;border-radius:12px;border:3px solid rgba(255,255,255,0.12)}
.titles h1{margin:0;font-size:20px;letter-spacing:1px;color:white}
.titles h2{margin:0;font-size:12px;color:rgba(255,255,255,0.9)}
.nav a{margin-left:16px;text-decoration:none;color:white;padding:8px 10px;border-radius:8px}
.nav .donate-btn{background:rgba(255,255,255,0.12);font-weight:600}
.hero{padding:56px 0;display:grid;place-items:center;text-align:center;color:white}
.hero .card{background:rgba(255,255,255,0.06);padding:32px;border-radius:16px;backdrop-filter:blur(6px)}
.hero h3{margin:8px 0 4px;font-size:22px}
.hero p{margin:0 0 12px;font-size:16px}
.buttons{display:flex;gap:12px;flex-wrap:wrap;justify-content:center}
.btn{padding:10px 16px;border-radius:10px;text-decoration:none;font-weight:600;background:rgba(255,255,255,0.95);color:var(--text)}
.btn.secondary{background:transparent;color:white;border:2px solid rgba(255,255,255,0.12)}
.section{padding:48px 0;background:transparent}
.card-light{background:white;padding:20px;border-radius:12px;box-shadow:0 6px 18px rgba(11,35,64,0.08)}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px}
.site-footer{padding:20px 0;color:white;opacity:0.95}
.burger{display:none;background:transparent;border:0;color:white;font-size:22px}

/* Small screens */
@media(max-width:820px){
  .nav{display:none}
  .burger{display:block}
  .header-inner{align-items:center}
}

