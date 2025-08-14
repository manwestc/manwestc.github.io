<style>
  :root{
    --ink:#1f2937; --muted:#64748b; --bd:#e5e7eb; --soft:#f8fafc;
    --card:#ffffff; --brand:#1565c0; --brand2:#0b67b8; --pill:#eef2ff;
    --ok:#16a34a; --warn:#f59e0b;
  }

  /* Título de sección con barra (igual que About/Publications) */
  .section h2{
    display:flex;align-items:center;gap:.5rem;
    font-size:1.3rem;font-weight:800;color:var(--ink);
    background:linear-gradient(90deg, rgba(21,101,192,.08), #fff);
    border-left:6px solid var(--brand); border-radius:12px;
    padding:.5rem .8rem; margin:1.2rem 0 .8rem;
  }
  .section h2::after{
    content:""; flex:1; height:3px; margin-left:.5rem;
    background:linear-gradient(to right,#4a90e2,#e91e63); border-radius:2px;
  }

  /* Contenedor general */
  .proj-wrap{max-width:1050px;margin:0 auto;padding:0 1rem}

  /* Cabeceras de subsección (Ongoing/Completed/…): pastilla */
  .subhead{
    display:inline-flex;align-items:center;gap:.5rem;
    background:var(--pill); border:1px solid var(--bd);
    color:#1f2937; font-weight:800; padding:.35rem .6rem; border-radius:999px;
    margin:.3rem 0 .8rem;
  }

  /* Rejilla de tarjetas */
  .proj-grid{
    display:grid; gap:.8rem;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
  }

  /* Tarjeta de proyecto */
  .proj-card{
    border:1px solid var(--bd); border-radius:12px; background:var(--card);
    padding:.85rem 1rem; box-shadow:0 2px 10px rgba(0,0,0,.03);
    display:flex; flex-direction:column; gap:.5rem;
  }
  /* Indicador lateral por estado */
  .proj-card.ongoing{border-left:6px solid var(--ok)}
  .proj-card.completed{border-left:6px solid #94a3b8}

  .proj-title{
    margin:0; color:#111827; font-weight:800; line-height:1.25;
    display:flex; gap:.5rem; align-items:flex-start;
  }
  .proj-role{color:#334155; font-weight:800}
  .proj-meta{
    display:flex; flex-wrap:wrap; gap:.4rem; margin-top:.1rem
  }
  .pill{
    display:inline-flex; align-items:center; gap:.35rem;
    font-size:.85rem; font-weight:700; color:#334155;
    background:#f1f5f9; border:1px solid var(--bd); border-radius:999px;
    padding:.18rem .55rem;
    white-space:nowrap;
  }
  .proj-desc{color:#374151; margin:.15rem 0 0}
</style>

<div class="proj-wrap">

  <div class="section"><h2>🚀 Competitive R&amp;D&amp;i Projects</h2></div>

  <div class="subhead">🟢 Ongoing</div>
  <div class="proj-grid">

    <article class="proj-card ongoing">
      <h3 class="proj-title">
        <span class="proj-role">Co-investigator</span>
      </h3>
      <p class="proj-desc"><em>“Cost-Effective Screening of Breast Cancer and Rheumatic Heart Disease Using Artificial Intelligence”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ State Agency for Investigation</span>
        <span class="pill">🆔 PID2023-150515OB-I00</span>
        <span class="pill">📅 Sept. 2024 – Aug. 2027</span>
        <span class="pill">📍 Spain</span>
      </div>
    </article>

    <article class="proj-card ongoing">
      <h3 class="proj-title">
        <span class="proj-role">Co-investigator</span>
      </h3>
      <p class="proj-desc"><em>“Development of HPC and data centre services and infrastructure”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ State Agency for Investigation</span>
        <span class="pill">🆔 PID2021-123627OB-C52</span>
        <span class="pill">📅 Sept. 2022 – Sept. 2025</span>
        <span class="pill">📍 Spain</span>
      </div>
    </article>

  </div>

  <div class="subhead" style="margin-top:1rem">🔵 Completed</div>
  <div class="proj-grid">

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Co-investigator</span></h3>
      <p class="proj-desc"><em>“Supercapacitor-based system for small electric vehicles and wireless devices”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ FONDECYT &amp; World Bank</span>
        <span class="pill">🆔 026-FONDECYT-BM-INC.INV</span>
        <span class="pill">📅 2020 – 2022</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Co-investigator</span></h3>
      <p class="proj-desc"><em>“Energy storage from microbial fuel cells for rural applications”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ FONDECYT</span>
        <span class="pill">🆔 401-FONDECYT</span>
        <span class="pill">📅 2020 – 2023</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Principal Investigator</span></h3>
      <p class="proj-desc"><em>“Smart Technologies for Ibero-American Cities”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ FONDECYT</span>
        <span class="pill">🆔 138-2017-FONDECYT</span>
        <span class="pill">📅 2017 – 2020</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Principal Investigator</span></h3>
      <p class="proj-desc"><em>“Citizen Safety and Road Applications in Smart Cities”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ Innóvate Perú / FINCyT</span>
        <span class="pill">🆔 PIAP-363</span>
        <span class="pill">📅 2014 – 2017</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Co-investigator</span></h3>
      <p class="proj-desc"><em>“Optimizing performance and energy in multimedia systems”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ Ministry of Science and Technology (CICYT)</span>
        <span class="pill">🆔 TIN2015-66972-C05-2-R</span>
        <span class="pill">📅 2017 – 2018</span>
        <span class="pill">📍 Spain</span>
      </div>
    </article>

    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Co-investigator</span></h3>
      <p class="proj-desc"><em>“Microgravity machine validation using parallel algorithms in GRID systems”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ FINCyT</span>
        <span class="pill">🆔 PIAP-1-P-622-13</span>
        <span class="pill">📅 2013 – 2016</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>

  </div>

  <div class="section"><h2>🌍 Social Development</h2></div>
  <div class="proj-grid">
    <article class="proj-card completed">
      <h3 class="proj-title"><span class="proj-role">Project Manager</span></h3>
      <p class="proj-desc"><em>“Smart Technologies and Education with Schoolchildren”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ Innóvate Perú</span>
        <span class="pill">📅 2017 – 2018</span>
        <span class="pill">📍 Peru</span>
      </div>
    </article>
  </div>

  <div class="section"><h2>🔗 Research Networks</h2></div>
  <div class="proj-grid">
    <article class="proj-card ongoing">
      <h3 class="proj-title"><span class="proj-role">Team Member</span></h3>
      <p class="proj-desc"><em>“AgIoT: Agricultural Internet of Things and Data Analytics for Precision Agriculture”</em></p>
      <div class="proj-meta">
        <span class="pill">🏛️ CYTED</span>
        <span class="pill">🆔 520RT0011</span>
        <span class="pill">📅 2021 – 2024</span>
        <a class="pill" href="http://www.cyted.org/AgIoT" target="_blank" rel="noopener">🔗 More Info</a>
      </div>
    </article>
  </div>

</div>