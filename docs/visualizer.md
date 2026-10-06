---
lang: en
lang_alt: vi/visualizer/
---

# 📊 Interactive Geotechnical Monitoring Visualizer

Experience an interactive visual model of geotechnical instrumentation systems, sensor physics, automated data acquisition topologies, and real-time displacement profiles.

---

<div style="background: #1e1e24; border-radius: 12px; padding: 24px; color: #f0f0f5; box-shadow: 0 8px 24px rgba(0,0,0,0.3); margin-bottom: 30px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;">
  <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; border-bottom: 1px solid #333; padding-bottom: 16px; margin-bottom: 20px; gap: 12px;">
    <div>
      <h2 style="margin: 0; color: #ff6b35; font-size: 22px;">🛠️ Geotech Instrumentation Sandbox</h2>
      <p style="margin: 4px 0 0 0; color: #8c8c9e; font-size: 14px;">Select an engineering scenario to simulate field instrumentation, structural deformation, and sensor arrays</p>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 8px;">
      <button id="btn-dam" onclick="switchScenario('dam')" style="background: #ff6b35; color: white; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Earth Dam</button>
      <button id="btn-excavation" onclick="switchScenario('excavation')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Deep Excavation</button>
      <button id="btn-slope" onclick="switchScenario('slope')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Slope Inclinometer</button>
      <button id="btn-tunnel" onclick="switchScenario('tunnel')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Tunnel Convergence</button>
      <button id="btn-pile" onclick="switchScenario('pile')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Bored Pile Test</button>
      <button id="btn-retaining" onclick="switchScenario('retaining')" style="background: #2a2a35; color: #ccc; border: none; padding: 7px 13px; border-radius: 6px; cursor: pointer; font-weight: 600; font-size: 12px;">Tieback Wall</button>
    </div>
  </div>

  <!-- Interactive Canvas and SVG Viewport -->
  <div style="display: grid; grid-template-columns: 1fr 340px; gap: 20px;">
    <!-- Graphical Cross Section -->
    <div style="background: #121217; border-radius: 8px; padding: 16px; border: 1px solid #2a2a35; position: relative;">
      <div style="display: flex; justify-content: space-between; margin-bottom: 8px;">
        <span style="font-size: 12px; color: #00e5ff; font-weight: bold; text-transform: uppercase; letter-spacing: 1px;">Cross-Section & Sensor Array</span>
        <span id="scenario-tag" style="font-size: 12px; color: #aaa;">Earth Embankment Dam (Dunnicliff Ch. 21)</span>
      </div>
      <svg id="geo-svg" viewBox="0 0 600 340" style="width: 100%; height: 320px; background: #0d0d11; border-radius: 6px;">
        <!-- Dynamically rendered via JS -->
      </svg>
      <div style="margin-top: 10px; display: flex; flex-wrap: wrap; gap: 12px; font-size: 11px; color: #8c8c9e;">
        <div><span style="display:inline-block; width:9px; height:9px; background:#00e5ff; border-radius:50%; margin-right:4px;"></span> Piezometer (VWP)</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ff4081; border-radius:50%; margin-right:4px;"></span> Inclinometer (IPI/MEMS)</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ffea00; border-radius:50%; margin-right:4px;"></span> Extensometer / Target</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#ff6b35; border-radius:50%; margin-right:4px;"></span> Load Cell / Strain Gauge</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#b388ff; border-radius:50%; margin-right:4px;"></span> Earth Pressure Cell</div>
        <div><span style="display:inline-block; width:9px; height:9px; background:#00e676; border-radius:50%; margin-right:4px;"></span> Wireless Hub</div>
      </div>
    </div>

    <!-- Live Telemetry & Control Panel -->
    <div style="background: #181820; border-radius: 8px; padding: 16px; border: 1px solid #2a2a35; display: flex; flex-direction: column; justify-content: space-between;">
      <div>
        <h4 style="margin: 0 0 12px 0; color: #f0f0f5; font-size: 15px; border-bottom: 1px solid #2a2a35; padding-bottom: 6px;">Live ADAS Diagnostics</h4>
        
        <div style="margin-bottom: 12px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span id="label-slider-1">Simulated Hydrostatic Head:</span>
            <strong id="val-head" style="color: #00e5ff;">18.5 m</strong>
          </label>
          <input type="range" id="slider-head" min="5" max="30" value="18.5" step="0.5" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #00e5ff;">
        </div>

        <div style="margin-bottom: 14px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span id="label-slider-2">Displacement / Load Stress:</span>
            <strong id="val-disp" style="color: #ff4081;">1.2 mm/day</strong>
          </label>
          <input type="range" id="slider-disp" min="0" max="10" value="1.2" step="0.1" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #ff4081;">
        </div>

        <div style="background: #121217; padding: 10px; border-radius: 6px; margin-bottom: 10px;">
          <div style="font-size: 11px; color: #888;">TARP Trigger State</div>
          <div id="tarp-badge" style="display: inline-block; padding: 3px 8px; border-radius: 4px; font-size: 12px; font-weight: bold; background: #004d40; color: #00e676; margin-top: 4px;">NORMAL (Level 0)</div>
        </div>

        <div style="font-size: 11px; color: #aaa; line-height: 1.5;">
          <div>📡 <strong>Telemetry:</strong> LoRaWAN 915 MHz / Mesh</div>
          <div>🔋 <strong>Hub Battery:</strong> 3.65V (SAFT LSH20)</div>
          <div>📶 <strong>RSSI:</strong> -44 dBm (Stable Link)</div>
          <div>⏱️ <strong>Interval:</strong> 15 mins (Continuous)</div>
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
    name: 'Earth Embankment Dam (Dunnicliff Ch. 21)',
    slider1: 'Simulated Hydrostatic Head:',
    slider2: 'Seepage / Pore Pressure Velocity:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  excavation: {
    name: 'Braced Deep Excavation & Wall (Dunnicliff Ch. 19)',
    slider1: 'Groundwater Head Differential:',
    slider2: 'Wall Deflection Rate:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  slope: {
    name: 'Slope Stability & Shear Plane Profiling (Dunnicliff Ch. 22)',
    slider1: 'Piezometric Surface Level:',
    slider2: 'Slip Surface Shear Rate:',
    s1Unit: ' m', s2Unit: ' mm/d'
  },
  tunnel: {
    name: 'Shield Tunneling & NATM Convergence (Dunnicliff Ch. 23)',
    slider1: 'Overburden Ground Pressure:',
    slider2: 'Radial Convergence Rate:',
    s1Unit: ' bar', s2Unit: ' mm/w'
  },
  pile: {
    name: 'Bored Pile Static Load Test (Dunnicliff Ch. 24)',
    slider1: 'Applied Hydraulic Test Load:',
    slider2: 'Pile Top Settlement:',
    s1Unit: ' kN', s2Unit: ' mm'
  },
  retaining: {
    name: 'Tieback Anchored Wall & Soil Nails (Dunnicliff Ch. 20)',
    slider1: 'Groundwater Seepage Height:',
    slider2: 'Lateral Wall Displacement:',
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
    badge.innerText = 'ACTION REQUIRED (Level 2 - Red)';
    badge.style.background = '#b71c1c';
    badge.style.color = '#ff8a80';
  } else if (s2 > 2.5 || s1 > 20.0) {
    badge.innerText = 'ALERT (Level 1 - Amber)';
    badge.style.background = '#e65100';
    badge.style.color = '#ffd180';
  } else {
    badge.innerText = 'NORMAL (Level 0 - Green)';
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
      <text x="20" y="320" fill="#665" font-size="12">Bedrock / Impermeable Base</text>
      
      <polygon points="100,220 220,100 320,100 500,220" fill="#4a3f35" stroke="#635446" stroke-width="2" />
      <polygon points="230,220 255,100 285,100 310,220" fill="#3a2e26" />
      <text x="250" y="180" fill="#887" font-size="11">Clay Core</text>

      <polygon points="0,${waterHeight} 170,${waterHeight} 170,220 0,220" fill="rgba(0, 229, 255, 0.25)" />
      <line x1="0" y1="${waterHeight}" x2="170" y2="${waterHeight}" stroke="#00e5ff" stroke-width="2" stroke-dasharray="4,4" />
      <text x="20" y="${waterHeight - 8}" fill="#00e5ff" font-size="11">Reservoir Head: ${head}m</text>

      <path d="M 170,${waterHeight} Q 260,${waterHeight + 40} 420,220" fill="none" stroke="#00e5ff" stroke-width="2" stroke-dasharray="3,3" />

      <line x1="220" y1="100" x2="220" y2="220" stroke="#ff4081" stroke-width="2" />
      <circle cx="220" cy="180" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-01</title></circle>
      <circle cx="220" cy="210" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-02</title></circle>

      <line x1="360" y1="130" x2="360" y2="220" stroke="#ffea00" stroke-width="2" />
      <circle cx="360" cy="190" r="5" fill="#00e5ff" stroke="#fff" stroke-width="1.5"><title>VWP-03 (Downstream)</title></circle>

      <line x1="270" y1="100" x2="270" y2="230" stroke="#ffea00" stroke-width="2" stroke-dasharray="2,2" />
      <rect x="265" y="140" width="10" height="3" fill="#ffea00" />
      <rect x="265" y="180" width="10" height="3" fill="#ffea00" />

      <rect x="260" y="85" width="20" height="15" fill="#00e676" rx="2" />
      <line x1="270" y1="85" x2="270" y2="70" stroke="#00e676" stroke-width="2" />
      <circle cx="270" cy="70" r="3" fill="#00e676" />
      <text x="290" y="82" fill="#00e676" font-size="11">Wireless Hub</text>
    `;
  } else if (currentScenario === 'excavation') {
    const wallDeflect = disp * 4;
    svg.innerHTML = `
      <rect x="0" y="60" width="240" height="280" fill="#3a3028" />
      <rect x="360" y="60" width="240" height="280" fill="#3a3028" />
      <rect x="240" y="60" width="120" height="180" fill="#0d0d11" />
      <text x="260" y="160" fill="#555" font-size="13">Excavation Base</text>

      <path d="M 240,60 Q ${240 + wallDeflect},150 240,280" fill="none" stroke="#90a4ae" stroke-width="6" />
      <path d="M 360,60 Q ${360 - wallDeflect},150 360,280" fill="none" stroke="#90a4ae" stroke-width="6" />

      <line x1="242" y1="90" x2="358" y2="90" stroke="#ff6b35" stroke-width="4" />
      <circle cx="242" cy="90" r="6" fill="#ffea00" stroke="#fff"><title>VW Load Cell 1</title></circle>
      
      <line x1="245" y1="160" x2="355" y2="160" stroke="#ff6b35" stroke-width="4" />
      <circle cx="245" cy="160" r="6" fill="#ffea00" stroke="#fff"><title>VW Load Cell 2</title></circle>

      <circle cx="${240 + wallDeflect * 0.7}" cy="120" r="4" fill="#ff4081" />
      <circle cx="${240 + wallDeflect}" cy="150" r="4" fill="#ff4081" />
      <circle cx="${240 + wallDeflect * 0.7}" cy="180" r="4" fill="#ff4081" />
      <text x="110" y="155" fill="#ff4081" font-size="11">IPI Array (Max Δ: ${disp}mm)</text>

      <path d="M 0,60 Q 180,${60 + disp * 2} 240,60" fill="none" stroke="#00e5ff" stroke-width="2" stroke-dasharray="3,3" />
      <text x="50" y="45" fill="#00e5ff" font-size="11">Settlement Trough</text>
    `;
  } else if (currentScenario === 'slope') {
    const slipShift = disp * 3;
    svg.innerHTML = `
      <polygon points="50,280 180,80 400,80 550,280" fill="#2d2b28" />
      
      <path d="M 120,260 Q 250,260 380,80" fill="none" stroke="#f44336" stroke-width="3" stroke-dasharray="4,4" />
      <text x="210" y="275" fill="#f44336" font-size="12">Critical Shear Plane</text>

      <line x1="240" y1="80" x2="240" y2="170" stroke="#ff4081" stroke-width="3" />
      <path d="M 240,170 Q ${240 - slipShift},210 240,280" fill="none" stroke="#ff4081" stroke-width="3" />
      
      <circle cx="240" cy="110" r="4" fill="#ff4081" />
      <circle cx="240" cy="140" r="4" fill="#ff4081" />
      <circle cx="${240 - slipShift * 0.8}" cy="190" r="5" fill="#ffea00" stroke="#fff"><title>Shear Zone Displaced</title></circle>
      <circle cx="240" cy="240" r="4" fill="#ff4081" />
      <text x="260" y="195" fill="#ffea00" font-size="11">Shear Horizon @ -14.5m</text>

      <line x1="310" y1="80" x2="310" y2="220" stroke="#00e5ff" stroke-width="2" />
      <circle cx="310" cy="210" r="6" fill="#00e5ff" stroke="#fff"><title>Piezometer VWP</title></circle>
      <text x="325" y="215" fill="#00e5ff" font-size="11">Pore Pressure Hub</text>
    `;
  } else if (currentScenario === 'tunnel') {
    const conv = disp * 2.5;
    const sag = disp * 2.0;
    const troughSag = disp * 2.5;
    svg.innerHTML = `
      <!-- Ground surface & soil layers -->
      <rect x="0" y="45" width="600" height="85" fill="#3a3028" />
      <rect x="0" y="130" width="600" height="210" fill="#25242d" />
      <line x1="0" y1="130" x2="600" y2="130" stroke="#444254" stroke-dasharray="4,4" />
      <text x="15" y="122" fill="#888" font-size="10">Overburden Soil / Weathered Rock Boundary</text>

      <!-- Surface Settlement Trough -->
      <path d="M 50,45 Q 300,${45 + troughSag} 550,45" fill="none" stroke="#00e5ff" stroke-width="2.5" stroke-dasharray="3,3" />
      <circle cx="300" cy="${45 + troughSag}" r="4" fill="#00e5ff" />
      <text x="315" y="40" fill="#00e5ff" font-size="11">Surface Trough Sag: ${(disp * 1.5).toFixed(1)} mm</text>

      <!-- MPBX Borehole from surface to tunnel crown -->
      <line x1="300" y1="45" x2="300" y2="${195 - sag}" stroke="#ffea00" stroke-width="2" />
      <rect x="295" y="100" width="10" height="3" fill="#ffea00" />
      <rect x="295" y="150" width="10" height="3" fill="#ffea00" />
      <circle cx="300" cy="45" r="4" fill="#ffea00" stroke="#fff"><title>MPBX Head</title></circle>
      <text x="312" y="105" fill="#ffea00" font-size="10">MPBX Anchor 1</text>
      <text x="312" y="155" fill="#ffea00" font-size="10">MPBX Anchor 2</text>

      <!-- Tunnel Lining (Segmental Ring with Ovalization Deformation) -->
      <ellipse cx="300" cy="${240 - sag * 0.3}" rx="${80 - conv * 0.7}" ry="${80 - sag * 0.6}" fill="#16161f" stroke="#78909c" stroke-width="8" />

      <!-- Radial Earth Pressure Cells on Exterior -->
      <rect x="215" y="235" width="6" height="12" fill="#b388ff" rx="1" />
      <rect x="379" y="235" width="6" height="12" fill="#b388ff" rx="1" />
      <rect x="296" y="${154 - sag * 0.6}" width="12" height="6" fill="#b388ff" rx="1" />
      <text x="400" y="242" fill="#b388ff" font-size="10">Radial EPC</text>

      <!-- Optical Convergence Chords & Pins -->
      <!-- Horizontal Chord -->
      <line x1="${225 + conv * 0.7}" y1="240" x2="${375 - conv * 0.7}" y2="240" stroke="#ff4081" stroke-width="1.5" stroke-dasharray="4,3" />
      <circle cx="${225 + conv * 0.7}" cy="240" r="5" fill="#ff4081" stroke="#fff" />
      <circle cx="${375 - conv * 0.7}" cy="240" r="5" fill="#ff4081" stroke="#fff" />
      <text x="250" y="234" fill="#ff4081" font-size="10">Convergence: ${(disp * 2.2).toFixed(1)} mm</text>

      <!-- Crown Settlement Target -->
      <circle cx="300" cy="${164 - sag * 0.6}" r="5" fill="#ffea00" stroke="#fff" />
      <text x="270" y="${180 - sag * 0.6}" fill="#ffea00" font-size="10">Crown Pin</text>

      <!-- Tunnel Center Label -->
      <text x="260" y="270" fill="#555" font-size="11">Tunnel Track</text>

      <!-- Inclinometer casing adjacent to tunnel -->
      <line x1="160" y1="45" x2="160" y2="330" stroke="#ff4081" stroke-width="2" />
      <circle cx="160" cy="200" r="4" fill="#ff4081" />
      <circle cx="160" cy="240" r="4" fill="#ff4081" />
      <circle cx="160" cy="280" r="4" fill="#ff4081" />
      <text x="90" y="240" fill="#ff4081" font-size="10">Side IPI Casing</text>

      <!-- Wireless Gateway -->
      <rect x="220" y="255" width="14" height="10" fill="#00e676" rx="2" />
      <circle cx="227" cy="250" r="2.5" fill="#00e676" />
      <text x="180" y="280" fill="#00e676" font-size="10">Sub-GHz Node</text>
    `;
  } else if (currentScenario === 'pile') {
    const pileTopSag = disp * 2.2;
    const jackP = head * 12;
    svg.innerHTML = `
      <!-- Geological layers -->
      <rect x="0" y="55" width="600" height="90" fill="#3a3028" />
      <text x="20" y="85" fill="#776" font-size="11">Soft Clay / Silt Layer</text>

      <rect x="0" y="145" width="600" height="95" fill="#332c25" />
      <text x="20" y="175" fill="#887" font-size="11">Dense Sand / Gravel Strata</text>

      <rect x="0" y="240" width="600" height="100" fill="#1f1d24" />
      <text x="20" y="270" fill="#665" font-size="11">Weathered Siltstone Bedrock</text>

      <!-- Reaction Beam & Jack Arrangement on surface -->
      <rect x="210" y="25" width="180" height="12" fill="#78909c" rx="2" />
      <text x="260" y="20" fill="#b0bec5" font-size="10">Reaction Steel Girder</text>
      
      <!-- Hydraulic Jack -->
      <rect x="280" y="37" width="40" height="${18 + pileTopSag * 0.3}" fill="#ff6b35" rx="2" />
      <text x="325" y="47" fill="#ff6b35" font-size="10">${jackP.toFixed(0)} kN Jack</text>

      <!-- Reference Beam & Dial Gauges -->
      <line x1="200" y1="50" x2="400" y2="50" stroke="#00e5ff" stroke-width="1.5" stroke-dasharray="2,2" />
      <circle cx="260" cy="${55 + pileTopSag}" r="4" fill="#ffea00" stroke="#fff"><title>LVDT 1</title></circle>
      <circle cx="340" cy="${55 + pileTopSag}" r="4" fill="#ffea00" stroke="#fff"><title>LVDT 2</title></circle>
      <text x="350" y="${60 + pileTopSag}" fill="#ffea00" font-size="10">LVDT Δ: ${(disp * 1.8).toFixed(2)}mm</text>

      <!-- Bored Pile Concrete Shaft -->
      <rect x="270" y="${55 + pileTopSag}" width="60" height="${240 - pileTopSag}" fill="#455a64" stroke="#607d8b" stroke-width="2" />

      <!-- Internal Strain Gauge Levels (Sister Bars) -->
      <!-- Level 1 -->
      <rect x="275" y="90" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="90" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="94" fill="#ff6b35" font-size="9">SG Level 1 (Clay)</text>

      <!-- Level 2 -->
      <rect x="275" y="160" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="160" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="164" fill="#ff6b35" font-size="9">SG Level 2 (Sand)</text>

      <!-- Level 3 -->
      <rect x="275" y="230" width="10" height="4" fill="#ff6b35" />
      <rect x="315" y="230" width="10" height="4" fill="#ff6b35" />
      <text x="330" y="234" fill="#ff6b35" font-size="9">SG Level 3 (Socket)</text>

      <!-- Telltale Rod to Pile Toe -->
      <line x1="290" y1="${55 + pileTopSag}" x2="290" y2="290" stroke="#ffea00" stroke-width="1.5" />
      <circle cx="290" cy="290" r="4" fill="#ffea00" stroke="#fff" />
      <text x="210" y="292" fill="#ffea00" font-size="9">Toe Telltale Anchor</text>

      <!-- Pile Base Pressure Cell / O-cell -->
      <rect x="272" y="290" width="56" height="6" fill="#b388ff" />
      <text x="280" y="308" fill="#b388ff" font-size="9">End Bearing Cell</text>

      <!-- Surrounding VWP Monitoring Excess Pore Pressure -->
      <line x1="180" y1="55" x2="180" y2="180" stroke="#00e5ff" stroke-width="1.5" />
      <circle cx="180" cy="120" r="5" fill="#00e5ff" stroke="#fff"><title>VWP Piezometer in Clay</title></circle>
      <text x="110" y="125" fill="#00e5ff" font-size="10">Pore Pressure Δu</text>

      <!-- Automated Datalogger -->
      <rect x="420" y="40" width="22" height="16" fill="#00e676" rx="2" />
      <circle cx="431" cy="35" r="3" fill="#00e676" />
      <text x="448" y="52" fill="#00e676" font-size="10">Logger DT2055</text>
    `;
  } else if (currentScenario === 'retaining') {
    const wallTilt = disp * 3.0;
    const waterTable = 140 - (head - 5) * 2.5;
    svg.innerHTML = `
      <!-- Retained Soil & Base -->
      <rect x="0" y="60" width="220" height="280" fill="#3a3028" />
      <rect x="220" y="220" width="380" height="120" fill="#242220" />
      <text x="260" y="260" fill="#555" font-size="13">Excavation Pit Invert</text>

      <!-- Groundwater & Phreatic Line behind wall -->
      <polygon points="0,${waterTable} 210,${waterTable + 30} 210,220 0,220" fill="rgba(0, 229, 255, 0.2)" />
      <line x1="0" y1="${waterTable}" x2="210" y2="${waterTable + 30}" stroke="#00e5ff" stroke-width="1.5" stroke-dasharray="3,3" />
      <text x="20" y="${waterTable - 6}" fill="#00e5ff" font-size="10">Groundwater Table</text>

      <!-- Retaining Wall Facing (with tilt deformation) -->
      <polygon points="210,60 ${210 + wallTilt},60 ${210 + wallTilt * 0.2},220 210,220" fill="#607d8b" stroke="#78909c" stroke-width="2" />

      <!-- Anchor Tier 1 (Tieback) -->
      <line x1="${210 + wallTilt}" y1="95" x2="60" y2="155" stroke="#ff6b35" stroke-width="3" />
      <!-- Bonded Anchor Zone -->
      <line x1="100" y1="140" x2="50" y2="160" stroke="#ff6b35" stroke-width="7" stroke-linecap="round" />
      <!-- Center Hole Load Cell at Wall Head -->
      <circle cx="${210 + wallTilt}" cy="95" r="6" fill="#ff6b35" stroke="#fff"><title>Anchor Load Cell 1</title></circle>
      <text x="${222 + wallTilt}" y="98" fill="#ff6b35" font-size="10">Load Cell 1</text>

      <!-- Anchor Tier 2 -->
      <line x1="${210 + wallTilt * 0.5}" y1="160" x2="90" y2="210" stroke="#ff6b35" stroke-width="3" />
      <line x1="120" y1="198" x2="80" y2="214" stroke="#ff6b35" stroke-width="7" stroke-linecap="round" />
      <circle cx="${210 + wallTilt * 0.5}" cy="160" r="6" fill="#ff6b35" stroke="#fff"><title>Anchor Load Cell 2</title></circle>
      <text x="${222 + wallTilt * 0.5}" y="164" fill="#ff6b35" font-size="10">Load Cell 2</text>

      <!-- Wall Facing Tiltmeter -->
      <rect x="${205 + wallTilt * 0.7}" y="125" width="10" height="12" fill="#ff4081" rx="1" />
      <text x="145" y="133" fill="#ff4081" font-size="9">Tilt: ${(disp * 0.12).toFixed(2)}°</text>

      <!-- Borehole Inclinometer behind wall (shows S-curve deformation) -->
      <path d="M 170,60 Q ${170 + wallTilt * 0.8},130 170,280" fill="none" stroke="#ff4081" stroke-width="2.5" />
      <circle cx="${170 + wallTilt * 0.75}" cy="120" r="4" fill="#ff4081" />
      <circle cx="${170 + wallTilt * 0.6}" cy="170" r="4" fill="#ff4081" />
      <circle cx="170" cy="230" r="4" fill="#ff4081" />
      <text x="110" y="75" fill="#ff4081" font-size="10">IPI Casing</text>

      <!-- Settlement Array behind wall -->
      <circle cx="140" cy="60" r="3.5" fill="#ffea00" />
      <circle cx="80" cy="60" r="3.5" fill="#ffea00" />
      <text x="60" y="52" fill="#ffea00" font-size="9">Settlement Pins</text>

      <!-- Wireless Hub at Wall Crest -->
      <rect x="215" y="35" width="18" height="14" fill="#00e676" rx="2" />
      <line x1="224" y1="35" x2="224" y2="25" stroke="#00e676" stroke-width="2" />
      <circle cx="224" cy="25" r="2.5" fill="#00e676" />
      <text x="240" y="45" fill="#00e676" font-size="10">Gateway Node</text>
    `;
  }
}

switchScenario('dam');
</script>

---

## 🏗️ End-to-End ADAS Telemetry Architecture

The diagram below illustrates how field sensors feed into the wireless cloud intelligence architecture:

```mermaid
graph TD
    subgraph Subsurface_Sensors["1. Subsurface Instruments"]
        VWP["Vibrating Wire Piezometers<br/>(VW2100 / VMP)"]
        IPI["In-Place Inclinometers<br/>(MEMS / Digital Bus)"]
        MPBX["Multi-Point Extensometers<br/>(Rod / Magnetic)"]
        LC["Load Cells & Strain Gauges<br/>(VW Load Cells / VWSG)"]
        SAA["Shape array<br/>(SAA3D deformations)"]
        EPC["Earth Pressure Cells<br/>(Hydraulic / VW)"]
    end

    subgraph Field_Logging_Telemetry["2. Autonomous Field Nodes & ADAS"]
        DT["DT Loggers<br/>(DT2011B / DT2055B / DT2485)"]
        L900["Wireless Nodes<br/>(900 MHz / 2.4 GHz Mesh)"]
        CR6["Data acquisition logger<br/>(multiplexed inputs)"]
        HUB["Wireless Gateway<br/>(Cellular / Satellite / LoRaWAN)"]
    end

    subgraph Cloud_Intelligence["3. Cloud Platform & Real-Time Analytics"]
        GEO["Cloud platform<br/>(web dashboard)"]
        CALC["Displacement & Velocity Vectors<br/>(Trend Lines / Spiral Corrections)"]
        TARP["Trigger Action Response Plans<br/>(Automated Alarms & Static Reports)"]
        GTI["GTI Doctor AI<br/>(Corpus-Grounded Assistant)"]
    end

    VWP -->|Analog VW Coil| DT
    IPI -->|RS-485 Digital Bus| DT
    MPBX -->|Potentiometer / VW| DT
    LC -->|Frequency Excitation| CR6
    SAA -->|Serial SAA Bus| CR6
    EPC -->|Hydraulic Diaphragm VW| DT

    DT -->|Low-Power RF| L900
    L900 -->|Wireless Mesh| HUB
    CR6 -->|Modbus / SDI-12| HUB
    
    HUB -->|MQTT / HTTPS TLS| GEO
    GEO --> CALC
    GEO --> TARP
    GEO --> GTI
```
