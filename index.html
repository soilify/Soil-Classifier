<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>Soil Classifier — AASHTO · USDA · USCS (with D10/D30/D60 interp)</title>
<style>
:root{
--bg:#f5f5dc; /* beige background */
--card:#ffffff; /* clean white cards */
--muted:#5c4a32; /* muted brown text */
--accent:#DEB887; /* medium brown accent */
--accent2:#DEB887; /* light brown accent */
}
*{box-sizing:border-box}
body{
margin:0;
font-family:Inter,system-ui,Arial,sans-serif;
background:var(--bg);
color:#3e2723; /* deep brown text */
}
header{
background:linear-gradient(90deg,var(--accent2),var(--accent));
color:beige;
padding:14px;
text-align:center;
}
.app{max-width:980px;margin:12px auto;padding:12px}
.tabs{display:flex;gap:8px;justify-content:center;margin-top:12px;flex-wrap:wrap}
.tab{padding:8px 14px;border-radius:999px;background:#fff;border:1px solid rgba(92,74,50,.15);cursor:pointer}
.tab.active{background:linear-gradient(90deg,var(--accent2),var(--accent));color:beige}
.panel{background:var(--card);border-radius:12px;padding:14px;margin-top:12px;box-shadow:0 6px 20px rgba(92,74,50,.1)}
.grid{display:grid;grid-template-columns:1fr 360px;gap:12px}
@media(max-width:880px){.grid{grid-template-columns:1fr}}
label{display:block;font-size:13px;color:var(--muted);margin-bottom:6px}
input[type=number], textarea{width:100%;padding:10px;border-radius:8px;border:1px solid #d7ccc8;font-size:14px;background:#fdfbf9}
.row{display:flex;gap:8px;align-items:center}
button{padding:10px 12px;border-radius:8px;border:none;background:var(--accent2);color:#3e2723;cursor:pointer}
.ghost{background:#f1edea}
.result{background:#f9f7f5;border-radius:8px;padding:10px;border:1px solid #e0d6cf}
pre{background:#4e342e;color:#fbe9e7;padding:10px;border-radius:8px;overflow:auto}
.kpi{display:flex;flex-direction:column;gap:6px;margin-bottom:8px}
.kpi .item{background:#f9f7f5;padding:8px;border-radius:8px;border:1px solid #e0d6cf}
.small{font-size:13px;padding:8px 10px;border-radius:8px}
footer{color:var(--muted);text-align:center;margin-top:12px;font-size:13px}
</style>
</head>
<body>
<header>
<h1>Soil Classifier — AASHTO · USDA · USCS</h1>
<div style="font-size:15px;opacity:.95">Quick, reliable, and precise soil classification for engineers and learners.</div>
</header>

<div class="app">
  <div class="tabs" role="tablist">
    <button class="tab active" data-tab="aashto">AASHTO</button>
    <button class="tab" data-tab="usda">USDA</button>
    <button class="tab" data-tab="uscs">USCS</button>
  </div>


  <div class="grid">
    <main>
      <!-- AASHTO -->
      <section id="aashto" class="panel" role="region">
        <h2 style="margin-top:0">AASHTO Soil Classification System</h2>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
          <div>
            <label for="a_p10">% Passing No.10 (2.00 mm)</label>
            <input id="a_p10" type="number" min="0" max="100" step="0.1" value="90">
          </div>
          <div>
            <label for="a_p40">% Passing No.40 (0.425 mm)</label>
            <input id="a_p40" type="number" min="0" max="100" step="0.1" value="74">
          </div>
          <div>
            <label for="a_p200">% Passing No.200 (0.075 mm)</label>
            <input id="a_p200" type="number" min="0" max="100" step="0.1" value="50">
          </div>
          <div>
            <label for="a_ll">Liquid Limit (LL) %</label>
            <input id="a_ll" type="number" min="0" max="200" step="0.1" value="38">
          </div>
          <div>
            <label for="a_pi">Plasticity Index (PI) %</label>
            <input id="a_pi" type="number" min="0" max="200" step="0.1" value="9">
          </div>

          <div style="display:flex;align-items:end">
            <div style="width:100%" class="row">
              <button id="runAASHTO" class="small">Classify</button>
              <button id="resetAASHTO" class="small ghost">Reset</button>
            </div> 
          </div>
        </div>
        
        <div id="outAASHTO" style="margin-top:12px;display:none">
          <div class="kpi">
            <div class="item"><strong>Group:</strong> <span id="a_group"></span></div>
            <div class="item"><strong>Subgroup:</strong> <span id="a_subgroup"></span></div>
            <div class="item"><strong>Coarse/Fine:</strong> <span id="a_coarse"></span></div>
            <div class="item"><strong>Group Index (GI):</strong> <span id="a_gi"></span></div>
          </div>
          <div><strong>Reasoning</strong><div class="result" id="a_reason"></div></div>
          <div style="margin-top:10px"><strong>Computed details</strong><pre id="a_computed"></pre></div>
        </div>
      </section>

      <!-- USDA -->
      <section id="usda" class="panel" role="region" style="display:none">
        <h2 style="margin-top:0">USDA Textural Soil Classification System</h2>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
          <div>
            <label for="u_gravel">Gravel % (optional)</label>
            <input id="u_gravel" type="number" min="0" max="100" step="0.1" value="0">
          </div>
          <div>
            <label for="u_sand">Sand %</label>
            <input id="u_sand" type="number" min="0" max="100" step="0.1" value="45">
          </div>
          <div>
            <label for="u_silt">Silt %</label>
            <input id="u_silt" type="number" min="0" max="100" step="0.1" value="35">
          </div>
          <div>
            <label for="u_clay">Clay %</label>
            <input id="u_clay" type="number" min="0" max="100" step="0.1" value="20">
          </div>
          <div style="grid-column:1/-1;display:flex;gap:8px;justify-content:flex-start">
            <button id="runUSDA" class="small">Classify</button>
            <button id="resetUSDA" class="small ghost">Reset</button>
          </div>
        </div>

        <div id="outUSDA" style="margin-top:12px;display:none">
          <div class="kpi">
            <div class="item"><strong>Texture:</strong> <span id="u_texture"></span></div>
            <div class="item"><strong>Fine-earth % (normalized):</strong> <span id="u_finepct"></span></div>
          </div>
          <div style="margin-top:8px"><strong>Modified percents used for triangle</strong>
            <div class="result"><pre id="u_computed"></pre></div>
          </div>
          <div style="margin-top:8px"><strong>Reasoning</strong><div class="result" id="u_reason"></div></div>
        </div>
      </section>

      <!-- USCS -->
      <section id="uscs" class="panel" role="region" style="display:none">
        <h2 style="margin-top:0">USCS (Unified Soil Classification System)</h2>
        <div>
          <label for="sieveCSV">Sieve data (CSV lines: sieve_name,diameter_mm,%passing). Include No.4 (4.75 mm) and No.200 (0.075 mm) if available.</label>
          <textarea id="sieveCSV" rows="7">10,2.00,90
40,0.425,74
200,0.075,50</textarea>
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:8px">
          <div>
            <label for="u_ll">Liquid Limit (LL) %</label>
            <input id="u_ll" type="number" min="0" max="200" step="0.1" value="38">
          </div>
          <div>
            <label for="u_pl">Plastic Limit (PL) %</label>
            <input id="u_pl" type="number" min="0" max="200" step="0.1" value="29">
          </div>
          <div style="grid-column:1/-1;display:flex;gap:8px;margin-top:6px">
            <button id="runUSCS" class="small">Classify</button>
            <button id="resetUSCS" class="small ghost">Reset</button>
          </div>
        </div>

        <div id="outUSCS" style="margin-top:12px;display:none">
          <div class="kpi">
            <div class="item"><strong>Symbol:</strong> <span id="uscs_symbol"></span></div>
            <div class="item"><strong>Group:</strong> <span id="uscs_group"></span></div>
          </div>
          <div style="margin-top:8px"><strong>Details & reasoning</strong>
            <div class="result"><pre id="uscs_details"></pre></div>
          </div>
          <div style="margin-top:8px"><strong>Computed D10, D30, D60, Cu, Cc (if interpolated)</strong>
            <div class="result"><pre id="uscs_sizes"></pre></div>
          </div>
        </div>
      </section>
    </main>

    <aside>
      <div class="panel">
        <h3 style="margin-top:0">How to use</h3>
        <ol style="padding-left:18px">
          <li>Choose AASHTO, USDA or USCS tab.</li>
          <li>Enter lab values (sieve % passing and Atterberg limits).</li>
          <li>Press <em>Classify</em>. Review computed D-values (D10/D30/D60), Cu/Cc, GI, and step-by-step reasoning.</li>
          <li>For USCS: provide sieve points that bracket 10%, 30%, and 60% for accurate interpolation.</li>
           <li>For both LL and PI = NP: it classified as A-3 (0).</li>
        </ol>
      </div>

      <div class="panel" style="margin-top:12px">
        <h4 style="margin:0">Notes</h4>
        <p style="color:var(--muted);font-size:13px">This app implements practical engineering logic: log-diameter interpolation for D-values, percent-based sand/gravel splits (sand = P4 − P200, gravel = 100 − P4), A-line PI checks, and AASHTO GI formula. This application or website is currently under development. Features and functions may change as improvements are made.</p>
      </div>
    </aside>
  </div>


<script>
/* Small helpers */
const $ = sel => document.querySelector(sel);
const $$ = sel => document.querySelectorAll(sel);
const toN = v => { const x = Number(v); return isFinite(x) ? x : 0; }
const r1 = v => Math.round(v*10)/10;

/* Tabs */
$$('.tab').forEach(b => b.addEventListener('click', () => {
  $$('.tab').forEach(x => x.classList.remove('active'));
  b.classList.add('active');
  const t = b.dataset.tab;
  ['aashto','usda','uscs'].forEach(id => $( '#' + id ).style.display = id === t ? 'block' : 'none');
}));

/* ---------- AASHTO ---------- */
function computeGI(F, LL, PI){
  let gi = (F - 35) * (0.2 + 0.005 * (LL - 40)) + 0.01 * (F - 15) * (PI - 10);
  if(!isFinite(gi) || isNaN(gi)) gi = 0;
  gi = Math.round(gi);
  if(gi < 0) gi = 0;
  return gi;
}

function classifyAASHTO(p10,p40,p200,LL,PI){
  const F = p200;
  const res = {group:'', subgroup:'', GI:0, coarseFine:'', reasoning:[], computed:''};
  const isFine = F > 35;
  res.coarseFine = isFine ? 'Fine (>35% passing #200)' : 'Coarse (≤35% passing #200)';
  res.reasoning.push(`P200 = ${F}% → ${res.coarseFine} (threshold 35%).`);

  if(!isFine){
    if(F <= 15 && p40 <= 30 && PI <= 6){
      res.group='A-1'; res.subgroup='A-1-a'; res.reasoning.push('Meets A-1-a: P200 ≤15%, P40 ≤30%, PI ≤6.');
    } else if(F <= 25 && PI <= 6){
      res.group='A-1'; res.subgroup='A-1-b'; res.reasoning.push('Meets A-1-b: P200 ≤25% and PI ≤6.');
    } else if(F <= 10 && (PI === 0 || p40 >= 50)){
      res.group='A-3'; res.subgroup='A-3'; res.reasoning.push('Fine sand behavior → A-3.');
    } else {
      res.group='A-2';
      if(LL > 40) res.subgroup = PI <= 10 ? 'A-2-5' : 'A-2-7';
      else res.subgroup = PI <= 10 ? 'A-2-4' : 'A-2-6';
      res.reasoning.push(`Assigned to A-2 family → ${res.subgroup}.`);
    }

    if(res.subgroup === 'A-2-6' || res.subgroup === 'A-2-7'){
      res.GI = Math.max(0, Math.round(0.01 * Math.max(0,(F - 15)) * Math.max(0,(PI - 10))));
      res.reasoning.push('GI computed using PI portion (common practical approach for A-2-6/A-2-7).');
    } else {
      res.GI = computeGI(F, LL, PI);
    }
  } else {
    if(LL > 40){
      if(PI <= 10){ res.group='A-5'; res.subgroup='A-5'; res.reasoning.push('LL >40 & PI ≤10 → A-5.'); }
      else { res.group='A-7'; res.subgroup = PI <= (LL - 30) ? 'A-7-5' : 'A-7-6'; res.reasoning.push(`LL >40 → ${res.subgroup}.`); }
    } else {
      if(PI <= 10){ res.group='A-4'; res.subgroup='A-4'; res.reasoning.push('LL ≤40 & PI ≤10 → A-4.'); }
      else { res.group='A-6'; res.subgroup='A-6'; res.reasoning.push('LL ≤40 & PI >10 → A-6.'); }
    }
    res.GI = computeGI(F, LL, PI);
  }
  res.computed = `Inputs:\nP10=${p10}%, P40=${p40}%, P200=${p200}%, LL=${LL}%, PI=${PI}%\n\nGI formula used:\nGI = (F-35)[0.2 + 0.005(LL-40)] + 0.01(F-15)(PI-10)\nComputed GI = ${res.GI}`;
  return res;
}

$('#runAASHTO').addEventListener('click', ()=>{
  const p10 = toN($('#a_p10').value), p40 = toN($('#a_p40').value), p200 = toN($('#a_p200').value), LL = toN($('#a_ll').value), PI = toN($('#a_pi').value);
  const r = classifyAASHTO(p10,p40,p200,LL,PI);
  $('#a_group').textContent = r.group; $('#a_subgroup').textContent = r.subgroup; $('#a_coarse').textContent = r.coarseFine; $('#a_gi').textContent = r.GI;
  $('#a_reason').innerHTML = r.reasoning.map(x=>'• '+x).join('<br>');
  $('#a_computed').textContent = r.computed; $('#outAASHTO').style.display = 'block';
});

$('#resetAASHTO').addEventListener('click', ()=>{
  $('#a_p10').value=90; $('#a_p40').value=74; $('#a_p200').value=50; $('#a_ll').value=38; $('#a_pi').value=9;
  $('#outAASHTO').style.display = 'none';
});

/* ---------- USDA ---------- */
function classifyUSDA(gravel,sand,silt,clay){
  const total = gravel + sand + silt + clay;
  if(total <= 0) return {error:'No data'};
  const fine = sand + silt + clay;
  const finePct = fine===0 ? 0 : r1((fine/total)*100);
  const modSand = fine===0 ? 0 : r1((sand/fine)*100);
  const modSilt = fine===0 ? 0 : r1((silt/fine)*100);
  const modClay = fine===0 ? 0 : r1((clay/fine)*100);
  let prefix = '';
  if(gravel >= 15) prefix = 'Gravelly ';
  // simple but practical classification rules (covers common classes)
  const S = modSand, Si = modSilt, C = modClay;
  let texture = 'Loam';
  if(C >= 40 && Si < 40) texture = 'Clay';
  else if(Si >= 40 && C < 40) texture = 'Silt';
  else if(S >= 85 && C < 10) texture = 'Sand';
  else if(S >= 70 && C <= 15) texture = 'Sandy loam';
  else if(S >= 50 && C <= 20) texture = 'Sandy loam';
  else if(S >= 43 && C >= 20 && C < 35) texture = 'Loam';
  else if(C >= 27 && C < 40 && S <= 45) texture = 'Clay loam';
  else if(Si > C && Si >= 40) texture = 'Silty loam';
  else texture = 'Loam (approx)';
  return {prefix, texture, finePct, modSand, modSilt, modClay};
}

$('#runUSDA').addEventListener('click', ()=>{
  const g = toN($('#u_gravel').value), s = toN($('#u_sand').value), si = toN($('#u_silt').value), c = toN($('#u_clay').value);
  const r = classifyUSDA(g,s,si,c);
  if(r.error){ $('#u_computed').textContent = r.error; $('#outUSDA').style.display='block'; return; }
  $('#u_texture').textContent = (r.prefix? r.prefix : '') + r.texture;
  $('#u_finepct').textContent = r.finePct + '%';
  $('#u_computed').textContent = `Fine-earth normalized (exclude gravel):\nSand = ${r.modSand}%\nSilt = ${r.modSilt}%\nClay = ${r.modClay}%`;
  $('#u_reason').textContent = `Gravel = ${g}%. Fine-earth used for triangle = ${r.finePct}%.`;
  $('#outUSDA').style.display='block';
});

$('#resetUSDA').addEventListener('click', ()=>{
  $('#u_gravel').value=0; $('#u_sand').value=45; $('#u_silt').value=35; $('#u_clay').value=20;
  $('#outUSDA').style.display='none';
});

/* ---------- USCS ---------- */
/* Parsing & interpolation helpers */
function parseCSV(txt){
  const lines = txt.split(/\r?\n/).map(l=>l.trim()).filter(l=>l && !l.startsWith('#'));
  const arr = [];
  for(const ln of lines){
    const p = ln.split(',').map(x=>x.trim());
    if(p.length < 3) continue;
    const name = p[0], d = parseFloat(p[1]), pct = parseFloat(p[2]);
    if(isFinite(d) && isFinite(pct)) arr.push({name,d,p:pct});
  }
  arr.sort((a,b)=>b.d - a.d);
  return arr;
}

/* Interpolate diameter at a given percent passing using linear interp in log(d) vs percent */
function interpDiameterAtPercent(sieves, Pt){
  if(sieves.length === 0) return null;
  // if Pt >= top percent -> return max diameter
  if(Pt >= sieves[0].p) return sieves[0].d;
  if(Pt <= sieves[sieves.length-1].p) return sieves[sieves.length-1].d;
  for(let i=0;i<sieves.length-1;i++){
    const p1 = sieves[i].p, p2 = sieves[i+1].p;
    const d1 = sieves[i].d, d2 = sieves[i+1].d;
    // bracket
    if((p1 >= Pt && Pt >= p2) || (p2 >= Pt && Pt >= p1)){
      const x1 = Math.log(d1), x2 = Math.log(d2);
      const t = (Pt - p1) / (p2 - p1);
      const x = x1 + t*(x2 - x1);
      return Math.exp(x);
    }
  }
  return null;
}

/* Find percent passing at a given diameter by log-d interpolation of percent vs log(d) */
function interpPercentAtDiameter(sieves, D){
  if(sieves.length === 0) return null;
  const xD = Math.log(D);
  const x0 = Math.log(sieves[0].d), p0 = sieves[0].p;
  const xN = Math.log(sieves[sieves.length-1].d), pN = sieves[sieves.length-1].p;
  if(D >= sieves[0].d) return sieves[0].p;
  if(D <= sieves[sieves.length-1].d) return sieves[sieves.length-1].p;
  for(let i=0;i<sieves.length-1;i++){
    const x1 = Math.log(sieves[i].d), x2 = Math.log(sieves[i+1].d);
    if((x1 >= xD && xD >= x2) || (x2 >= xD && xD >= x1)){
      const p1 = sieves[i].p, p2 = sieves[i+1].p;
      const t = (xD - x1) / (x2 - x1);
      return p1 + t*(p2 - p1);
    }
  }
  return null;
}

/* USCS classification wrapper */
function classifyUSCS(sieves, LL, PL){
  const PI = LL - PL;
  const details = [];
  if(sieves.length === 0) return {symbol:'Unknown', group:'No data', details:'No sieve data provided.'};

  // percent passing #200
  let p200 = null;
  for(const s of sieves){ if(s.d <= 0.075 + 1e-9){ p200 = s.p; break; } }
  if(p200 == null){
    const ip = interpPercentAtDiameter(sieves, 0.075);
    if(ip != null){ p200 = ip; details.push('Interpolated % passing #200 (log-d interpolation).'); }
    else { p200 = sieves[sieves.length-1].p; details.push('Could not bracket #200; using smallest sieve %passing.'); }
  }
  p200 = r1(p200);
  details.push(`P200 ≈ ${p200}%`);

  // percent passing #4 (4.75 mm)
  let p4 = null;
  for(const s of sieves){ if(s.d <= 4.75 + 1e-9){ p4 = s.p; break; } }
  if(p4 == null){
    const ip = interpPercentAtDiameter(sieves, 4.75);
    if(ip != null){ p4 = ip; details.push('Interpolated % passing #4 (log-d interpolation).'); }
    else { p4 = sieves[0].p; details.push('Could not bracket #4; using largest sieve %passing.'); }
  }
  p4 = r1(p4);
  details.push(`P4 ≈ ${p4}%`);

  // sand and gravel
  const gravelPct = r1(100 - p4);               // % retained on #4
  const sandPct = r1(p4 - p200);                // between #4 and #200
  const finesPct = p200;                        // passing #200
  details.push(`Computed coarse split: Gravel = ${gravelPct}%, Sand = ${sandPct}%, Fines = ${finesPct}%`);

  // decide who is dominant among sand vs gravel as user requested
  const dominantCoarse = gravelPct > sandPct ? 'gravel' : (sandPct > gravelPct ? 'sand' : 'equal');

  // compute D10, D30, D60 by interpolation (if sieve covers)
  const D10 = interpDiameterAtPercent(sieves, 10);
  const D30 = interpDiameterAtPercent(sieves, 30);
  const D60 = interpDiameterAtPercent(sieves, 60);
  let sizesText = '';
  if(D10 && D30 && D60){
    sizesText += `D10=${r1(D10)} mm, D30=${r1(D30)} mm, D60=${r1(D60)} mm\n`;
    const Cu = D60 / D10, Cc = (D30*D30) / (D10 * D60);
    sizesText += `Cu=${r1(Cu)}, Cc=${r1(Cc)}\n`;
  } else {
    sizesText = 'D10/D30/D60 not fully determined (need gradation bracketing 10%,30%,60%).';
  }

  // Now classification logic:
  // If fines <= 50% -> coarse-grained family
  // else -> fine-grained (use LL and PI with A-line)
  if(finesPct <= 50){
    // coarse-grained: check for "clean" (fines<=5) vs with fines
    if(finesPct <= 5){
      details.push('Fines ≤ 5% → clean coarse-grained soil. Use Cu/Cc to check well-graded vs poorly-graded.');
      // choose sand vs gravel using dominantCoarse
      if(D10 && D30 && D60){
        const Cu = D60 / D10, Cc = (D30*D30) / (D10 * D60);
        details.push(`Cu=${r1(Cu)}, Cc=${r1(Cc)} (from interpolated D-values).`);
        if(dominantCoarse === 'sand'){
          if(Cu >= 6 && Cc >=1 && Cc <=3) return {symbol:'SW', group:'Well-graded sand (SW)', details:details.join('\n'), sizes:sizesText};
          else return {symbol:'SP', group:'Poorly-graded sand (SP)', details:details.join('\n'), sizes:sizesText};
        } else { // gravel dominant or equal
          if(Cu >= 4 && Cc >=1 && Cc <=3) return {symbol:'GW', group:'Well-graded gravel (GW)', details:details.join('\n'), sizes:sizesText};
          else return {symbol:'GP', group:'Poorly-graded gravel (GP)', details:details.join('\n'), sizes:sizesText};
        }
      } else {
        details.push('Insufficient D-values → choose coarse symbol approximate by dominant coarse type.');
        return {symbol: dominantCoarse === 'gravel' ? 'GP/GW (approx)' : 'SP/SW (approx)', group:'Coarse-grained (approx)', details:details.join('\n'), sizes:sizesText};
      }
    } else if(finesPct >5 && finesPct <= 12){
      // dual symbol area: e.g., SW-SM or SP-SM or GW-GM etc., depending on plasticity of fines
      details.push('Fines between 5% and 12% → dual symbol (coarse with nonplastic/plastic fines). Check PI to decide M (nonplastic) or C (plastic).');
      const PI = LL - PL;
      const finesPlastic = PI >= 4;
      if(dominantCoarse === 'sand'){
        return {symbol: finesPlastic ? 'SP-SC (approx)' : 'SP-SM (approx)', group:'Sandy with fines', details:details.join('\n'), sizes:sizesText};
      } else {
        return {symbol: finesPlastic ? 'GP-GC (approx)' : 'GP-GM (approx)', group:'Gravelly with fines', details:details.join('\n'), sizes:sizesText};
      }
    } else {
      // fines >12% and <=50% -> coarse with significant fines => classify as SM/SC/GM/GC depending on plasticity
      details.push('Fines > 12% → classify as sand/gravel with significant fines (SM/SC or GM/GC). Use PI to decide M vs C.');
      const PI = LL - PL;
      const finesPlastic = PI >= 4;
      if(dominantCoarse === 'sand'){
        return {symbol: finesPlastic ? 'SC (approx)' : 'SM (approx)', group: 'Sandy with fines', details:details.join('\n'), sizes:sizesText};
      } else {
        return {symbol: finesPlastic ? 'GC (approx)' : 'GM (approx)', group: 'Gravelly with fines', details:details.join('\n'), sizes:sizesText};
      }
    }
  } else {
    // fines > 50% => fine-grained. Use LL & PI and A-line
    details.push('Fine-grained soil (>50% passing #200). Use Atterberg limits and A-line to classify (ML/CL/MH/CH).');
    const AlinePI = 0.73 * (LL - 20);
    const PI = LL - PL;
    details.push(`LL=${LL}, PL=${PL}, PI=${PI}. A-line PI = ${r1(AlinePI)}.`);
    if(LL < 50){
      if(PI >= AlinePI) return {symbol:'CL', group:'Lean clay (CL)', details:details.join('\n'), sizes:sizesText};
      else return {symbol:'ML', group:'Silt (ML)', details:details.join('\n'), sizes:sizesText};
    } else {
      if(PI >= AlinePI) return {symbol:'CH', group:'High-plasticity clay (CH)', details:details.join('\n'), sizes:sizesText};
      else return {symbol:'MH', group:'Elastic silt (MH)', details:details.join('\n'), sizes:sizesText};
    }
  }
}

/* UI wiring for USCS wrapper */
$('#runUSCS').addEventListener('click', ()=>{
  const csv = $('#sieveCSV').value;
  const sieves = parseCSV(csv);
  const LL = toN($('#u_ll').value), PL = toN($('#u_pl').value);
  const res = classifyUSCS(sieves, LL, PL);
  $('#uscs_symbol').textContent = res.symbol || '—';
  $('#uscs_group').textContent = res.group || '—';
  $('#uscs_details').textContent = res.details || '—';
  $('#uscs_sizes').textContent = res.sizes || (res.sizes === '' ? '' : 'D-values not computed.');
  $('#outUSCS').style.display = 'block';
});

$('#resetUSCS').addEventListener('click', ()=>{
  $('#sieveCSV').value = '10,2.00,90\n40,0.425,74\n200,0.075,50';
  $('#u_ll').value = 38; $('#u_pl').value = 29;
  $('#outUSCS').style.display = 'none';
});
</script>
</body>
</html>
