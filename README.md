# -juan1234567800000.hitguh.io
paguina sintetica
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cafetería Mendoza · Café &amp; Pastelería</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700&family=Libre+Franklin:wght@400;500;700&family=IBM+Plex+Mono:wght@500&display=swap" rel="stylesheet">
<style>
  :root{
    --coffee-900:#2B1810;
    --coffee-700:#4A2E1F;
    --paper:#F3E9DA;
    --caramel:#C68B4A;
    --caramel-dark:#A66C30;
    --sage:#8FA06E;
    --cream-text:#F3E9DA;
  }
  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    background:var(--coffee-900);
    color:var(--cream-text);
    font-family:'Libre Franklin',sans-serif;
    line-height:1.55;
  }
  h1,h2,h3{
    font-family:'Fraunces',serif;
    font-weight:600;
    margin:0 0 .3em;
  }
  .eyebrow{
    font-family:'IBM Plex Mono',monospace;
    font-size:.72rem;
    letter-spacing:.14em;
    text-transform:uppercase;
    color:var(--caramel);
  }
  a{color:var(--caramel);}
  .wrap{max-width:1080px;margin:0 auto;padding:0 24px;}
  section{padding:88px 0;}

  /* HERO */
  .hero{
    min-height:92vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    position:relative;
    background:
      radial-gradient(ellipse at 80% 0%, rgba(198,139,74,.25), transparent 55%),
      var(--coffee-900);
    border-bottom:1px solid rgba(243,233,218,.12);
  }
  .hero .wrap{width:100%;}
  .hero h1{
    font-size:clamp(2.6rem,7vw,5.2rem);
    line-height:.98;
    max-width:11ch;
  }
  .hero p.tag{
    font-size:1.15rem;
    max-width:42ch;
    color:rgba(243,233,218,.82);
    margin-top:18px;
  }
  .hero-cta{display:flex;gap:14px;margin-top:36px;flex-wrap:wrap;}
  .btn{
    font-family:'IBM Plex Mono',monospace;
    font-size:.82rem;
    letter-spacing:.04em;
    text-decoration:none;
    padding:14px 24px;
    border-radius:2px;
    display:inline-block;
    transition:transform .15s ease;
  }
  .btn:hover{transform:translateY(-2px);}
  .btn-solid{background:var(--caramel);color:var(--coffee-900);font-weight:700;}
  .btn-line{border:1px solid rgba(243,233,218,.4);color:var(--cream-text);}

  .hero-address{
    position:absolute;
    right:24px;
    bottom:28px;
    font-family:'IBM Plex Mono',monospace;
    font-size:.75rem;
    color:rgba(243,233,218,.55);
    text-align:right;
  }

  /* GALLERY */
  .gallery-grid{
    display:grid;
    grid-template-columns:repeat(6,1fr);
    grid-auto-rows:130px;
    gap:10px;
    margin-top:40px;
  }
  .ph{
    background:linear-gradient(135deg,var(--coffee-700),var(--coffee-900));
    border:1px dashed rgba(198,139,74,.5);
    border-radius:4px;
    display:flex;align-items:center;justify-content:center;
    color:rgba(243,233,218,.45);
    font-family:'IBM Plex Mono',monospace;
    font-size:.68rem;
    text-align:center;
    padding:8px;
  }
  .g1{grid-column:span 3;grid-row:span 2;}
  .g2{grid-column:span 3;grid-row:span 1;}
  .g3{grid-column:span 3;grid-row:span 1;}
  .g4{grid-column:span 2;grid-row:span 1;}
  .g5{grid-column:span 2;grid-row:span 1;}
  .g6{grid-column:span 2;grid-row:span 1;}

  /* ABOUT */
  .about{
    background:var(--paper);
    color:var(--coffee-900);
    border-radius:4px;
  }
  .about h2{color:var(--coffee-900);}
  .about-inner{padding:64px 40px;display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:center;}
  .about p{font-size:1.05rem;color:var(--coffee-700);}
  .menu-ticket{
    background:var(--coffee-900);
    color:var(--cream-text);
    border-radius:2px;
    padding:26px 22px;
    font-family:'IBM Plex Mono',monospace;
    font-size:.85rem;
    position:relative;
  }
  .menu-ticket::before,.menu-ticket::after{
    content:"";
    position:absolute;left:0;right:0;height:14px;
    background:
      radial-gradient(circle 7px at 0 50%, transparent 98%, var(--paper)) ,
      radial-gradient(circle 7px at 16px 50%, var(--paper) 99%, transparent 0) ;
    background-size:16px 14px;
    background-repeat:repeat-x;
  }
  .menu-ticket::before{top:-7px;}
  .menu-ticket::after{bottom:-7px;transform:rotate(180deg);}
  .menu-ticket .row{display:flex;justify-content:space-between;padding:6px 0;border-bottom:1px dashed rgba(243,233,218,.2);}
  .menu-ticket .row:last-child{border-bottom:none;}

  /* REVIEWS */
  .reviews-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:36px;}
  .review-card{
    background:var(--coffee-700);
    border-radius:4px;
    padding:26px;
    border-top:3px solid var(--sage);
  }
  .review-card p{font-size:.95rem;color:rgba(243,233,218,.9);}
  .review-source{font-family:'IBM Plex Mono',monospace;font-size:.72rem;color:var(--sage);margin-top:14px;display:block;}

  /* LOCATION */
  .loc-grid{display:grid;grid-template-columns:1.1fr 1fr;gap:32px;margin-top:36px;align-items:stretch;}
  .loc-info{background:var(--coffee-700);border-radius:4px;padding:32px;}
  .loc-info dt{font-family:'IBM Plex Mono',monospace;font-size:.7rem;color:var(--caramel);text-transform:uppercase;letter-spacing:.1em;margin-top:18px;}
  .loc-info dt:first-child{margin-top:0;}
  .loc-info dd{margin:4px 0 0;font-size:1.02rem;}
  iframe{width:100%;height:100%;min-height:280px;border:0;border-radius:4px;filter:sepia(15%) saturate(85%);}

  /* CONTACT */
  .contact{text-align:center;}
  .contact h2{font-size:clamp(1.8rem,4vw,2.8rem);}
  .contact-links{display:flex;justify-content:center;gap:16px;flex-wrap:wrap;margin-top:30px;}

  footer{
    padding:32px 0;
    text-align:center;
    font-family:'IBM Plex Mono',monospace;
    font-size:.75rem;
    color:rgba(243,233,218,.45);
    border-top:1px solid rgba(243,233,218,.1);
  }

  @media (max-width:760px){
    .about-inner{grid-template-columns:1fr;}
    .reviews-grid{grid-template-columns:1fr;}
    .loc-grid{grid-template-columns:1fr;}
    .gallery-grid{grid-template-columns:repeat(3,1fr);grid-auto-rows:110px;}
    .g1{grid-column:span 3;}
    .g2,.g3,.g4,.g5,.g6{grid-column:span 3;}
    .hero-address{position:static;margin-top:40px;text-align:left;}
  }
</style>
</head>
<body>

<header class="hero">
  <div class="wrap">
    <div class="eyebrow">Café &amp; Pastelería · Ciudad de Mendoza</div>
    <h1>Cafetería Mendoza</h1>
    <p class="tag">Café de buena materia prima, pastelería de la casa y brunch de vereda, en pleno centro. Para reservas, escribinos por WhatsApp.</p>
    <div class="hero-cta">
      <a class="btn btn-solid" href="#ubicacion">Ver ubicación</a>
      <a class="btn btn-line" href="https://www.instagram.com/coffeeoclockok/" target="_blank" rel="noopener">Instagram @coffeeoclockok</a>
    </div>
  </div>
  <div class="hero-address">Luzuriaga 583, Ciudad, Mendoza</div>
</header>

<section class="wrap">
  <div class="eyebrow">Galería</div>
  <h2>Lo que se cocina adentro</h2>
  <div class="gallery-grid">
    <div class="ph g1">FOTO PLACEHOLDER<br>[reemplazar por foto real subida por el cliente]</div>
    <div class="ph g2">FOTO PLACEHOLDER</div>
    <div class="ph g3">FOTO PLACEHOLDER</div>
    <div class="ph g4">FOTO PLACEHOLDER</div>
    <div class="ph g5">FOTO PLACEHOLDER</div>
    <div class="ph g6">FOTO PLACEHOLDER</div>
  </div>
</section>

<section class="wrap about">
  <div class="about-inner">
    <div>
      <div class="eyebrow">Sobre nosotros</div>
      <h2>Cafetería &amp; Pastelería</h2>
      <p>Un local pensado para la merienda de vereda: café bien extraído, pastelería casera y una carta que va cambiando. La materia prima se nota — es lo primero que resaltan quienes vuelven.</p>
      <p>Abierto en el centro de Mendoza, sobre Luzuriaga. Recomendado para desayunos largos, meriendas y ese ratito de brunch de fin de semana.</p>
    </div>
    <div class="menu-ticket">
      <div class="row"><span>Brunch para 2</span><span>$4.500</span></div>
      <div class="row"><span>Porción de torta</span><span>$1.000</span></div>
      <div class="row"><span>Bagel</span><span>$1.300</span></div>
      <div class="row"><span>Croissant relleno</span><span>$1.300</span></div>
      <div class="row"><span>Café bombón</span><span>$750</span></div>
    </div>
  </div>
</section>

<section class="wrap">
  <div class="eyebrow">Reseñas</div>
  <h2>Lo que dicen quienes vuelven</h2>
  <div class="reviews-grid">
    <div class="review-card">
      <p>Destacan la calidad de la materia prima por sobre todo — se nota la diferencia frente a otros locales de la zona, especialmente en la pastelería.</p>
      <span class="review-source">— Reseña pública en redes sociales</span>
    </div>
    <div class="review-card">
      <p>El brunch y los waffles son de los platos más pedidos; buena opción para una merienda de fin de semana en el centro.</p>
      <span class="review-source">— Reseña pública en redes sociales</span>
    </div>
    <div class="review-card">
      <p>[Espacio reservado — agregar un testimonio propio o una reseña de Google Maps cuando el negocio la confirme]</p>
      <span class="review-source">— Pendiente de confirmar</span>
    </div>
  </div>
</section>

<section class="wrap" id="ubicacion">
  <div class="eyebrow">Ubicación</div>
  <h2>Encontranos en el centro</h2>
  <div class="loc-grid">
    <div class="loc-info">
      <dl>
        <dt>Dirección</dt>
        <dd>Luzuriaga 583, Ciudad, Mendoza, Argentina</dd>
        <dt>Reservas</dt>
        <dd>Por WhatsApp (agregar número real del negocio)</dd>
        <dt>Horario</dt>
        <dd>[Confirmar con el negocio]</dd>
      </dl>
    </div>
    <iframe loading="lazy" src="https://www.google.com/maps?q=Luzuriaga+583,+Ciudad,+Mendoza,+Argentina&output=embed"></iframe>
  </div>
</section>

<section class="wrap contact">
  <div class="eyebrow">Contacto</div>
  <h2>¿Nos hacemos un lugar?</h2>
  <div class="contact-links">
    <a class="btn btn-solid" href="https://wa.me/5492610000000" target="_blank" rel="noopener">Escribinos por WhatsApp</a>
    <a class="btn btn-line" href="https://www.instagram.com/coffeeoclockok/" target="_blank" rel="noopener">Seguinos en Instagram</a>
  </div>
</section>

<footer>Cafetería Mendoza — 2026 · Sitio generado a partir del perfil de Instagram @coffeeoclockok</footer>

</body>
</html>
