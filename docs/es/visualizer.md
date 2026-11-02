---
lang: es
lang_alt: visualizer/
---

# 📊 Visualizador Interactivo de Monitoreo Geotécnico

Explore un modelo visual interactivo de sistemas de instrumentación geotécnica, física de sensores, topologías de adquisición automatizada de datos y perfiles de desplazamiento en tiempo real.

---

<div style="background: #1e1e24; border-radius: 12px; padding: 24px; color: #f0f0f5; box-shadow: 0 8px 24px rgba(0,0,0,0.3); margin-bottom: 30px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;">
  <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; border-bottom: 1px solid #333; padding-bottom: 16px; margin-bottom: 20px; gap: 12px;">
    <div>
      <h2 style="margin: 0; color: #ff6b35; font-size: 22px;">🛠️ Banco de Pruebas de Instrumentación Geotécnica</h2>
      <p style="margin: 4px 0 0 0; color: #8c8c9e; font-size: 14px;">Seleccione un escenario de ingeniería para simular instrumentación de campo, deformación estructural y arreglos de sensores</p>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 8px;">
      <button id="btn-dam" onclick="switchScenario('dam')" style="background: #ff6b35; color: white; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Presa de Tierra</button>
      <button id="btn-excavation" onclick="switchScenario('excavation')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Excavación Profunda</button>
      <button id="btn-slope" onclick="switchScenario('slope')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Inclinómetro en Talud</button>
      <button id="btn-tunnel" onclick="switchScenario('tunnel')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Convergencia de Túnel</button>
      <button id="btn-pile" onclick="switchScenario('pile')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Ensayo de Pilote Perforado</button>
      <button id="btn-retaining" onclick="switchScenario('retaining')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Muro con Tirantes</button>
    </div>
  </div>

  <!-- Lienzo interactivo y viewport SVG -->
  <div style="display: grid; grid-template-columns: 1fr 340px; gap: 20px;">
    <!-- Corte transversal gráfico -->
    <div style="background: #121217; border-radius: 8px; padding: 16px; border: 1px solid #2a2a35; position: relative;">
      <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
        <span style="font-size: 12px; color: #00e5ff; font-weight: bold; text-transform: uppercase; letter-spacing: 1px;">Corte Transversal y Arreglo de Sensores</span>
        <span id="scenario-tag" style="font-size: 12px; color: #aaa;">Presa de Terraplén de Tierra (Dunnicliff Cap. 21)</span>
      </div>
      <svg id="geo-svg" viewBox="0 0 600 340" style="width: 100%; height: 320px; background: #0d0d11; border-radius: 6px;">
        <!-- Renderizado dinámico vía JS -->
      </svg>
      <div style="margin-top: 10px; display: flex; flex-wrap: wrap; gap: 12px; font-size: 11px; color: #8c8c9e;">
        <div><span style="display:inline-block; width:9px; height:9px; background:#00e5ff; border-radius:50%; margin-right:4px;"></span> Piezómetro (VWP)</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ff4081; border-radius:50%; margin-right:4px;"></span> Inclinómetro (IPI/MEMS)</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ffea00; border-radius:50%; margin-right:4px;"></span> Extensómetro / Objetivo</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ff6b35; border-radius:50%; margin-right:4px;"></span> Célula de Carga / Galga de Deformación</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#b388ff; border-radius:50%; margin-right:4px;"></span> Célula de Presión de Tierras</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#00e676; border-radius:50%; margin-right:4px;"></span> Concentrador Inalámbrico</div>
      </div>
    </div>

    <!-- Panel de telemetría en vivo y control -->
    <div style="background: #181820; border-radius: 8px; padding: 16px; border: 1px solid #2a2a35; display: flex; flex-direction: column; justify-content: space-between;">
      <div>
        <h4 style="margin: 0 0 12px 0; color: #f0f0f5; font-size: 15px; border-bottom: 1px solid #2a2a35; padding-bottom: 6px;">Diagnóstico ADAS en Vivo</h4>

        <div style="margin-bottom: 12px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span id="label-slider-1">Carga Hidrostática Simulada:</span>
            <strong id="val-head" style="color: #00e5ff;">18.5 m</strong>
          </label>
          <input type="range" id="slider-head" min="5" max="30" value="18.5" step="0.5" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #00e5ff;">
        </div>

        <div style="margin-bottom: 14px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span id="label-slider-2">Desplazamiento / Tensión de Carga:</span>
            <strong id="val-disp" style="color: #ff4081;">1.2 mm/día</strong>
          </label>
          <input type="range" id="slider-disp" min="0" max="10" value="1.2" step="0.1" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #ff4081;">
        </div>

        <div style="background: #121217; padding: 10px; border-radius: 6px; margin-bottom: 10px;">
          <div style="font-size: 11px; color: #888;">Estado de Disparo TARP</div>
          <div id="tarp-badge" style="display: inline-block; padding: 3px 8px; border-radius: 4px; font-size: 12px; font-weight: bold; background: #004d40; color: #00e676; margin-top: 4px;">NORMAL (Nivel 0)</div>
        </div>

        <div style="font-size: 11px; color: #aaa; line-height: 1.5;">
          <div>📡 <strong>Telemetría:</strong> LoRaWAN 915 MHz / Malla</div>
          <div>🔋 <strong>Batería del Concentrador:</strong> 3.65V (SAFT LSH20)</div>
          <div>📶 <strong>RSSI:</strong> -44 dBm (Enlace Estable)</div>
          <div>⏱️ <strong>Intervalo:</strong> 15 min (Continuo)</div>
        </div>
      </div>

      <div id="sensor-readout-box" style="background: #0d0d11; padding: 10px; border-radius: 6px; border-left: 3px solid #ff6b35; font-family: monospace; font-size: 11px; color: #e0e0e0; margin-top: 10px;">
        P_vw1: 181.4 kPa<br>
        T_vw1: 14.2 °C<br>
        Incli_max: 3.4 mm @ -12m
      </div>
    </div>
  </div>
</div>

<script>
let currentScenario = 'dam';

const scenarioConfigs = {
  dam: {
    name: 'Presa de Terraplén de Tierra (Dunnicliff Cap. 21)',
    slider1: 'Carga Hidrostática Simulada:',
    slider2: 'Velocidad de Filtración / Presión de Poros:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  excavation: {
    name: 'Excavación Profunda Arriostrada y Muro (Dunnicliff Cap. 19)',
    slider1: 'Diferencial de Carga de Aguas Subterráneas:',
    slider2: 'Tasa de Deflexión del Muro:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  slope: {
    name: 'Estabilidad de Talud y Perfilado del Plano de Cizalla (Dunnicliff Cap. 22)',
    slider1: 'Nivel de Superficie Piezométrica:',
    slider2: 'Tasa de Cizalla de la Superficie de Deslizamiento:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  tunnel: {
    name: 'Tunelización con Escudo y Convergencia NATM (Dunnicliff Cap. 23)',
    slider1: 'Presión de Terreno de Recubrimiento:',
    slider2: 'Tasa de Convergencia Radial:',
    s1Unit: ' bar', s2Unit: ' mm/sem'
  },
  pile: {
    name: 'Ensayo de Carga Estática de Pilote Perforado (Dunnicliff Cap. 24)',
    slider1: 'Carga de Ensayo Hidráulica Aplicada:',
    slider2: 'Asentamiento en la Cabeza del Pilote:',
    s1Unit: ' kN', s2Unit: ' mm'
  },
  retaining: {
    name: 'Muro Anclado con Tirantes y Clavos de Suelo (Dunnicliff Cap. 20)',
    slider1: 'Altura de Filtración de Aguas Subterráneas:',
    slider2: 'Desplazamiento Lateral del Muro:',
    s1Unit: ' m', s2Unit: ' mm'
  }
};

function switchScenario(sc) {
  currentScenario = sc;
  const btnIds = ['dam', 'excavation', 'slope', 'tunnel', 'pile', 'retaining'];
  btnIds.forEach(id => {
    const el = document.getElementById('btn-' + id);
    if (el) {
      el.style.background = (sc === id) ? '#ff6b35' : '#2a2a35';
      el.style.color = (sc === id) ? 'white' : '#ccc';
    }
  });

  const cfg = scenarioConfigs[sc];
  if (cfg) {
    document.getElementById('scenario-tag').innerText = cfg.name;
    document.getElementById('label-slider-1').innerText = cfg.slider1;
    document.getElementById('label-slider-2').innerText = cfg.slider2;
  }
  renderScene();
}

function updateSimulation() {
  const s1 = parseFloat(document.getElementById('slider-head').value);
  const s2 = parseFloat(document.getElementById('slider-disp').value);
  const cfg = scenarioConfigs[currentScenario] || scenarioConfigs.dam;

  document.getElementById('val-head').innerText = s1.toFixed(1) + cfg.s1Unit;
  document.getElementById('val-disp').innerText = s2.toFixed(1) + cfg.s2Unit;

  const badge = document.getElementById('tarp-badge');
  if (s2 > 5.0 || s1 > 25.0) {
    badge.innerText = 'ACCIÓN REQUERIDA (Nivel 2 - Rojo)';
    badge.style.background = '#b71c1c';
    badge.style.color = '#ff8a80';
  } else if (s2 > 2.5 || s1 > 20.0) {
    badge.innerText = 'ALERTA (Nivel 1 - Ámbar)';
    badge.style.background = '#e65100';
    badge.style.color = '#ffd180';
  } else {
    badge.innerText = 'NORMAL (Nivel 0 - Verde)';
    badge.style.background = '#004d40';
    badge.style.color = '#00e676';
  }

  const readout = document.getElementById('sensor-readout-box');
  if (currentScenario === 'dam') {
    const pKpa = (s1 * 9.81).toFixed(1);
    readout.innerHTML = `P_pore: ${pKpa} kPa<br>Disp_rate: ${s2.toFixed(1)} mm/d<br>Sweep: 2145 Hz (Linear)`;
  } else if (currentScenario === 'excavation') {
    const strutT = (s2 * 120 + 250).toFixed(0);
    readout.innerHTML = `Wall_Δmax: ${(s2 * 3.5).toFixed(1)} mm<br>Strut_Load: ${strutT} kN<br>Trough_Sag: ${(s2 * 1.8).toFixed(1)} mm`;
  } else if (currentScenario === 'slope') {
    const shearZ = 14.5;
    readout.innerHTML = `Shear_Depth: -${shearZ} m<br>Slip_Velocity: ${s2.toFixed(1)} mm/d<br>P_water: ${(s1 * 9.81).toFixed(1)} kPa`;
  } else if (currentScenario === 'tunnel') {
    const convH = (s2 * 2.2).toFixed(1);
    const sagCrown = (s2 * 1.5).toFixed(1);
    const epcRadial = (s1 * 12.5).toFixed(1);
    readout.innerHTML = `ΔD_horizontal: ${convH} mm<br>Crown_Sag: ${sagCrown} mm<br>Radial_EPC: ${epcRadial} kPa`;
  } else if (currentScenario === 'pile') {
    const loadKN = (s1 * 150).toFixed(0);
    const setMM = (s2 * 1.8).toFixed(2);
    const skinFriction = (s2 * 24.5).toFixed(1);
    readout.innerHTML = `Jack_Load: ${loadKN} kN<br>Top_Settlement: ${setMM} mm<br>Skin_Friction: ${skinFriction} kPa`;
  } else if (currentScenario === 'retaining') {
    const anchorT = (s2 * 45 + 180).toFixed(0);
    const wallTilt = (s2 * 0.12).toFixed(2);
    readout.innerHTML = `Anchor_Tension: ${anchorT} kN<br>Facing_Tilt: ${wallTilt}°<br>Pore_Drawdown: ${s1.toFixed(1)} m`;
  }

  renderScene();
}

function renderScene() {
  const svg = document.getElementById('geo-svg');
  const head = parseFloat(document.getElementById('slider-head').value);
  const disp = parseFloat(document.getElementById('slider-disp').value);

  if (currentScenario === 'dam') {
    const waterHeight = 120 - (head - 5) * 3;
    svg.innerHTML = `
      <rect x="0" y="220" width="600" height="120" fill="#2d261e" />
      <text x="20" y="320" fill="#665" font-size="12">Roca Base / Base Impermeable</text>

      <polygon points="100,220 220,100 320,100 500,220" fill="#4a3f35" stroke="#635446" stroke-width="2" />
      <polygon points="230,220 255,100 285,100 310,220" fill="#3a2e26" />
      <text x="250" y="180" fill="#887" font-size="11">Núcleo de Arcilla</text>

      <polygon points="0,${waterHeight} 170,${waterHeight} 170,220 0,220" fill="rgba(0, 229, 255, 0.25)" />
      <line x1="0" y1="${waterHeight}" x2="170" y2="${waterHeight}" stroke="#00e5ff" stroke-width="2" stroke-dasharray="4,4" />
      <text x="20" y="${waterHeight - 8}" fill="#00e5ff" font-size="11">Carga del Embalse: ${head}m</text>

      <path d="M 170,${waterHeight} Q 260,${waterHeight + 40} 420,220" fill="none" stroke="#00e5ff" stroke-width="2" stroke-dasharray="3,3" />

      <line x1="220" y1="100" x2="220" y2="220" stroke="#ff4081" stroke-width="2" />
      <circle cx="220" cy="180" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-01</title></circle>
      <circle cx="220" cy="210" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-02</title></circle>

      <line x1="360" y1="130" x2="360" y2="220" stroke="#ffea00" stroke-width="2" />
      <circle cx="360" cy="190" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-03 (Aguas Abajo)</title></circle>

      <line x1="270" y1="100" x2="270" y2="230" stroke="#ffea00" stroke-width="2" stroke-dasharray="2,2" />
      <rect x="265" y="140" width="10" height="3" fill="#ffea00" />
      <rect x="265" y="180" width="10" height="3" fill="#ffea00" />

      <rect x="260" y="85" width="20" height="15" fill="#00e676" rx="2" />
      <line x1="270" y1="85" x2="270" y2="70" stroke="#00e676" stroke-width="2" />
      <circle cx="270" cy="70" r="3" fill="#00e676" />
      <text x="290" y="82" fill="#00e676" font-size="11">Concentrador Inalámbrico</text>
    `;
  } else if (currentScenario === 'excavation') {
    const wallDeflect = disp * 4;
    svg.innerHTML = `
      <rect x="0" y="60" width="240" height="280" fill="#3a3028" />
      <rect x="360" y="60" width="240" height="280" fill="#3a3028" />
      <rect x="240" y="60" width="120" height="180" fill="#0d0d11" />
      <text x="260" y="160" fill="#555" font-size="13">Base de Excavación</text>

      <path d="M 240,60 Q ${240 + wallDeflect},150 240,280" fill="none" stroke="#90a4ae" stroke-width="6" />
      <path d="M 360,60 Q ${360 - wallDeflect},150 360,280" fill="none" stroke="#90a4ae" stroke-width="6" />

      <line x1="242" y1="90" x2="358" y2="90" stroke="#ff6b35" stroke-width="4" />
      <circle cx="242" cy="90" r="6" fill="#ffea00" stroke="#fff"><title>VW Load Cell 1</title></circle>

      <line x1="245" y1="160" x2="355" y2="160" stroke="#ff6b35" stroke-width="4" />
      <circle cx="245" cy="160" r="6" fill="#ffea00" stroke="#fff"><title>VW Load Cell 2</title></circle>

      <circle cx="${240 + wallDeflect * 0.7}" cy="120" r="4" fill="#ff4081" />
      <circle cx="${240 + wallDeflect}" cy="150" r="4" fill="#ff4081" />
      <circle cx="${240 + wallDeflect * 0.7}" cy="180" r="4" fill="#ff4081" />
      <text x="110" y="155" fill="#ff4081" font-size="11">Arreglo IPI (Δ Máx: ${disp}mm)</text>

      <path d="M 0,60 Q 180,${60 + disp * 2} 240,60" fill="none" stroke="#00e5ff" stroke-width="2" stroke-dasharray="3,3" />
      <text x="50" y="45" fill="#00e5ff" font-size="11">Depresión de Asentamiento</text>
    `;
  } else if (currentScenario === 'slope') {
    const slipShift = disp * 3;
    svg.innerHTML = `
      <polygon points="50,280 180,80 400,80 550,280" fill="#2d2b28" />

      <path d="M 120,260 Q 250,260 380,80" fill="none" stroke="#f44336" stroke-width="3" stroke-dasharray="4,4" />
      <text x="210" y="275" fill="#f44336" font-size="12">Plano de Cizalla Crítico</text>

      <line x1="240" y1="80" x2="240" y2="170" stroke="#ff4081" stroke-width="3" />
      <path d="M 240,170 Q ${240 - slipShift},210 240,280" fill="none" stroke="#ff4081" stroke-width="3" />

      <circle cx="240" cy="110" r="4" fill="#ff4081" />
      <circle cx="240" cy="140" r="4" fill="#ff4081" />
      <circle cx="${240 - slipShift * 0.8}" cy="190" r="5" fill="#ffea00" stroke="#fff"><title>Zona de Cizalla Desplazada</title></circle>
      <circle cx="240" cy="240" r="4" fill="#ff4081" />
      <text x="260" y="195" fill="#ffea00" font-size="11">Horizonte de Cizalla @ -14.5m</text>

      <line x1="310" y1="80" x2="310" y2="220" stroke="#00e5ff" stroke-width="2" />
      <circle cx="310" cy="210" r="6" fill="#00e5ff" stroke="#fff"><title>Piezómetro VWP</title></circle>
      <text x="325" y="215" fill="#00e5ff" font-size="11">Concentrador de Presión de Poros</text>
    `;
  } else if (currentScenario === 'tunnel') {
    const conv = disp * 2.5;
    const sag = disp * 2.0;
    const troughSag = disp * 2.5;
    svg.innerHTML = `
      <!-- Superficie del terreno y capas de suelo -->
      <rect x="0" y="45" width="600" height="85" fill="#3a3028" />
      <rect x="0" y="130" width="600" height="210" fill="#25242d" />
      <line x1="0" y1="130" x2="600" y2="130" stroke="#444254" stroke-dasharray="4,4" />
      <text x="15" y="122" fill="#888" font-size="10">Límite de Suelo de Recubrimiento / Roca Meteorizada</text>

      <!-- Depresión de asentamiento superficial -->
      <path d="M 50,45 Q 300,${45 + troughSag} 550,45" fill="none" stroke="#00e5ff" stroke-width="2.5" stroke-dasharray="3,3" />
      <circle cx="300" cy="${45 + troughSag}" r="4" fill="#00e5ff" />
      <text x="315" y="40" fill="#00e5ff" font-size="11">Hundimiento de la Depresión Superficial: ${(disp * 1.5).toFixed(1)} mm</text>

      <!-- Sondeo MPBX desde la superficie hasta la coronación del túnel -->
      <line x1="300" y1="45" x2="300" y2="${195 - sag}" stroke="#ffea00" stroke-width="2" />
      <rect x="295" y="100" width="10" height="3" fill="#ffea00" />
      <rect x="295" y="150" width="10" height="3" fill="#ffea00" />
      <circle cx="300" cy="45" r="4" fill="#ffea00" stroke="#fff"><title>Cabeza MPBX</title></circle>
      <text x="312" y="105" fill="#ffea00" font-size="10">Ancla MPBX 1</text>
      <text x="312" y="155" fill="#ffea00" font-size="10">Ancla MPBX 2</text>

      <!-- Revestimiento del túnel (anillo segmentado con deformación ovalada) -->
      <ellipse cx="300" cy="${240 - sag * 0.3}" rx="${80 - conv * 0.7}" ry="${80 - sag * 0.6}" fill="#16161f" stroke="#78909c" stroke-width="8" />

      <!-- Células de presión de tierras radiales en el exterior -->
      <rect x="215" y="235" width="6" height="12" fill="#b388ff" rx="1" />
      <rect x="379" y="235" width="6" height="12" fill="#b388ff" rx="1" />
      <rect x="296" y="${154 - sag * 0.6}" width="12" height="6" fill="#b388ff" rx="1" />
      <text x="400" y="242" fill="#b388ff" font-size="10">EPC Radial</text>

      <!-- Cuerdas y clavijas de convergencia óptica -->
      <!-- Cuerda horizontal -->
      <line x1="${225 + conv * 0.7}" y1="240" x2="${375 - conv * 0.7}" y2="240" stroke="#ff4081" stroke-width="1.5" stroke-dasharray="4,3" />
      <circle cx="${225 + conv * 0.7}" cy="240" r="5" fill="#ff4081" stroke="#fff" />
      <circle cx="${375 - conv * 0.7}" cy="240" r="5" fill="#ff4081" stroke="#fff" />
      <text x="250" y="234" fill="#ff4081" font-size="10">Convergencia: ${(disp * 2.2).toFixed(1)} mm</text>

      <!-- Clavija de coronación -->
      <circle cx="300" cy="${164 - sag * 0.6}" r="5" fill="#ffea00" stroke="#fff" />
      <text x="270" y="${180 - sag * 0.6}" fill="#ffea00" font-size="10">Clavija de Coronación</text>

      <!-- Etiqueta central del túnel -->
      <text x="260" y="270" fill="#555" font-size="11">Vía del Túnel</text>

      <!-- Tubo de inclinómetro adyacente al túnel -->
      <line x1="160" y1="45" x2="160" y2="330" stroke="#ff4081" stroke-width="2" />
      <circle cx="160" cy="200" r="4" fill="#ff4081" />
      <circle cx="160" cy="240" r="4" fill="#ff4081" />
      <circle cx="160" cy="280" r="4" fill="#ff4081" />
      <text x="90" y="240" fill="#ff4081" font-size="10">Tubo IPI Lateral</text>

      <!-- Pasarela inalámbrica -->
      <rect x="220" y="255" width="14" height="10" fill="#00e676" rx="2" />
      <circle cx="227" cy="250" r="2.5" fill="#00e676" />
      <text x="180" y="280" fill="#00e676" font-size="10">Nodo Sub-GHz</text>
    `;
  } else if (currentScenario === 'pile') {
    const pileTopSag = disp * 2.2;
    const jackP = head * 12;
    svg.innerHTML = `
      <!-- Capas geológicas -->
      <rect x="0" y="55" width="600" height="90" fill="#3a3028" />
      <text x="20" y="85" fill="#776" font-size="11">Capa de Arcilla Blanda / Limo</text>

      <rect x="0" y="145" width="600" height="95" fill="#332c25" />
      <text x="20" y="175" fill="#887" font-size="11">Estratos de Arena Densa / Grava</text>

      <rect x="0" y="240" width="600" height="100" fill="#1f1d24" />
      <text x="20" y="270" fill="#665" font-size="11">Roca Base de Siltolita Meteorizada</text>

      <!-- Viga de reacción y arreglo del gato en superficie -->
      <rect x="210" y="25" width="180" height="12" fill="#78909c" rx="2" />
      <text x="260" y="20" fill="#b0bec5" font-size="10">Viga de Acero de Reacción</text>

      <!-- Gato hidráulico -->
      <rect x="280" y="37" width="40" height="${18 + pileTopSag * 0.3}" fill="#ff6b35" rx="2" />
      <text x="325" y="47" fill="#ff6b35" font-size="10">${jackP.toFixed(0)} kN Gato</text>

      <!-- Viga de referencia y relojes comparadores -->
      <line x1="200" y1="50" x2="400" y2="50" stroke="#00e5ff" stroke-width="1.5" stroke-dasharray="2,2" />
      <circle cx="260" cy="${55 + pileTopSag}" r="4" fill="#ffea00" stroke="#fff"><title>LVDT 1</title></circle>
      <circle cx="340" cy="${55 + pileTopSag}" r="4" fill="#ffea00" stroke="#fff"><title>LVDT 2</title></circle>
      <text x="350" y="${60 + pileTopSag}" fill="#ffea00" font-size="10">LVDT Δ: ${(disp * 1.8).toFixed(2)}mm</text>

      <!-- Fuste de concreto del pilote perforado -->
      <rect x="270" y="${55 + pileTopSag}" width="60" height="${240 - pileTopSag}" fill="#455a64" stroke="#607d8b" stroke-width="2" />

      <!-- Niveles internos de galgas de deformación (barras gemelas) -->
      <!-- Nivel 1 -->
      <rect x="275" y="90" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="90" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="94" fill="#ff6b35" font-size="9">Galga Nivel 1 (Arcilla)</text>

      <!-- Nivel 2 -->
      <rect x="275" y="160" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="160" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="164" fill="#ff6b35" font-size="9">Galga Nivel 2 (Arena)</text>

      <!-- Nivel 3 -->
      <rect x="275" y="230" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="230" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="234" fill="#ff6b35" font-size="9">Galga Nivel 3 (Encaje)</text>

      <!-- Varilla indicadora hasta la punta del pilote -->
      <line x1="290" y1="${55 + pileTopSag}" x2="290" y2="290" stroke="#ffea00" stroke-width="1.5" />
      <circle cx="290" cy="290" r="4" fill="#ffea00" stroke="#fff" />
      <text x="210" y="292" fill="#ffea00" font-size="9">Ancla Indicadora en la Punta</text>

      <!-- Célula de presión en la base del pilote / O-cell -->
      <rect x="272" y="290" width="56" height="6" fill="#b388ff" />
      <text x="280" y="308" fill="#b388ff" font-size="9">Célula de Apoyo en Extremo</text>

      <!-- Monitoreo VWP de presión de poros excedente circundante -->
      <line x1="180" y1="55" x2="180" y2="180" stroke="#00e5ff" stroke-width="1.5" />
      <circle cx="180" cy="120" r="5" fill="#00e5ff" stroke="#fff"><title>Piezómetro VWP en Arcilla</title></circle>
      <text x="110" y="125" fill="#00e5ff" font-size="10">Presión de Poros Δu</text>

      <!-- Registrador automatizado -->
      <rect x="420" y="40" width="22" height="16" fill="#00e676" rx="2" />
      <circle cx="431" cy="35" r="3" fill="#00e676" />
      <text x="448" y="52" fill="#00e676" font-size="10">Registrador DT2055</text>
    `;
  } else if (currentScenario === 'retaining') {
    const wallTilt = disp * 3.0;
    const waterTable = 140 - (head - 5) * 2.5;
    svg.innerHTML = `
      <!-- Suelo retenido y base -->
      <rect x="0" y="60" width="220" height="280" fill="#3a3028" />
      <rect x="220" y="220" width="380" height="120" fill="#242220" />
      <text x="260" y="260" fill="#555" font-size="13">Fondo de la Excavación</text>

      <!-- Aguas subterráneas y línea freática detrás del muro -->
      <polygon points="0,${waterTable} 210,${waterTable + 30} 210,220 0,220" fill="rgba(0, 229, 255, 0.2)" />
      <line x1="0" y1="${waterTable}" x2="210" y2="${waterTable + 30}" stroke="#00e5ff" stroke-width="1.5" stroke-dasharray="3,3" />
      <text x="20" y="${waterTable - 6}" fill="#00e5ff" font-size="10">Nivel Freático</text>

      <!-- Frente del muro de contención (con deformación por inclinación) -->
      <polygon points="210,60 ${210 + wallTilt},60 ${210 + wallTilt * 0.2},220 210,220" fill="#607d8b" stroke="#78909c" stroke-width="2" />

      <!-- Nivel 1 de anclaje (tirante) -->
      <line x1="${210 + wallTilt}" y1="95" x2="60" y2="155" stroke="#ff6b35" stroke-width="3" />
      <!-- Zona de anclaje adherida -->
      <line x1="100" y1="140" x2="50" y2="160" stroke="#ff6b35" stroke-width="7" stroke-linecap="round" />
      <!-- Célula de carga de orificio pasante en la cabeza del muro -->
      <circle cx="${210 + wallTilt}" cy="95" r="6" fill="#ff6b35" stroke="#fff"><title>Célula de Carga de Anclaje 1</title></circle>
      <text x="${222 + wallTilt}" y="98" fill="#ff6b35" font-size="10">Célula de Carga 1</text>

      <!-- Nivel 2 de anclaje -->
      <line x1="${210 + wallTilt * 0.5}" y1="160" x2="90" y2="210" stroke="#ff6b35" stroke-width="3" />
      <line x1="120" y1="198" x2="80" y2="214" stroke="#ff6b35" stroke-width="7" stroke-linecap="round" />
      <circle cx="${210 + wallTilt * 0.5}" cy="160" r="6" fill="#ff6b35" stroke="#fff"><title>Célula de Carga de Anclaje 2</title></circle>
      <text x="${222 + wallTilt * 0.5}" y="164" fill="#ff6b35" font-size="10">Célula de Carga 2</text>

      <!-- Tiltímetro en el frente del muro -->
      <rect x="${205 + wallTilt * 0.7}" y="125" width="10" height="12" fill="#ff4081" rx="1" />
      <text x="145" y="133" fill="#ff4081" font-size="9">Inclinación: ${(disp * 0.12).toFixed(2)}°</text>

      <!-- Inclinómetro de sondeo detrás del muro (muestra deformación en S) -->
      <path d="M 170,60 Q ${170 + wallTilt * 0.8},130 170,280" fill="none" stroke="#ff4081" stroke-width="2.5" />
      <circle cx="${170 + wallTilt * 0.75}" cy="120" r="4" fill="#ff4081" />
      <circle cx="${170 + wallTilt * 0.6}" cy="170" r="4" fill="#ff4081" />
      <circle cx="170" cy="230" r="4" fill="#ff4081" />
      <text x="110" y="75" fill="#ff4081" font-size="10">Tubo IPI</text>

      <!-- Arreglo de asentamiento detrás del muro -->
      <circle cx="140" cy="60" r="3.5" fill="#ffea00" />
      <circle cx="80" cy="60" r="3.5" fill="#ffea00" />
      <text x="60" y="52" fill="#ffea00" font-size="9">Clavijas de Asentamiento</text>

      <!-- Concentrador inalámbrico en la corona del muro -->
      <rect x="215" y="35" width="18" height="14" fill="#00e676" rx="2" />
      <line x1="224" y1="35" x2="224" y2="25" stroke="#00e676" stroke-width="2" />
      <circle cx="224" cy="25" r="2.5" fill="#00e676" />
      <text x="240" y="45" fill="#00e676" font-size="10">Nodo de Pasarela</text>
    `;
  }
}

switchScenario('dam');
</script>

---

## 🏗️ Arquitectura de Telemetría ADAS de Extremo a Extremo

El diagrama a continuación ilustra cómo los sensores de campo se integran en la arquitectura inalámbrica de inteligencia en la nube:

```mermaid
graph TD
    subgraph Subsurface_Sensors["1. Instrumentos del Subsuelo"]
        VWP["Piezómetros de Cuerda Vibrante<br/>(VW2100 / VMP)"]
        IPI["Inclinómetros In Situ<br/>(MEMS / Bus Digital)"]
        MPBX["Extensómetros Multipunto<br/>(Varilla / Magnético)"]
        LC["Células de Carga y Galgas de Deformación<br/>(Células VW / VWSG)"]
        SAA["Arreglo de Forma<br/>(Deformaciones SAA3D)"]
        EPC["Células de Presión de Tierras<br/>(Hidráulica / VW)"]
    end

    subgraph Field_Logging_Telemetry["2. Nodos de Campo Autónomos y ADAS"]
        DT["Registradores DT<br/>(DT2011B / DT2055B / DT2485)"]
        L900["Nodos Inalámbricos<br/>(900 MHz / 2.4 GHz Malla)"]
        CR6["Registrador de Adquisición de Datos<br/>(entradas multiplexadas)"]
        HUB["Pasarela Inalámbrica<br/>(Celular / Satelital / LoRaWAN)"]
    end

    subgraph Cloud_Intelligence["3. Plataforma en la Nube y Análisis en Tiempo Real"]
        GEO["Plataforma en la Nube<br/>(panel web)"]
        CALC["Vectores de Desplazamiento y Velocidad<br/>(Líneas de Tendencia / Correcciones en Espiral)"]
        TARP["Planes de Acción y Respuesta ante Umbrales<br/>(Alarmas Automatizadas e Informes Estáticos)"]
        GTI["Asistente IA GTI Doctor<br/>(Asistente Basado en Corpus)"]
    end

    VWP -->|Bobina VW Analógica| DT
    IPI -->|Bus Digital RS-485| DT
    MPBX -->|Potenciómetro / VW| DT
    LC -->|Excitatión por Frecuencia| CR6
    SAA -->|Bus Serie SAA| CR6
    EPC -->|Diafragma Hidráulico VW| DT

    DT -->|RF Baja Potencia| L900
    L900 -->|Malla Inalámbrica| HUB
    CR6 -->|Modbus / SDI-12| HUB

    HUB -->|MQTT / HTTPS TLS| GEO
    GEO --> CALC
    GEO --> TARP
    GEO --> GTI
```
