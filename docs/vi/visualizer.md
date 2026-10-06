---
lang: vi
lang_alt: visualizer/
---

# 📊 Môi trường thử nghiệm tương tác

Trải nghiệm mô hình trực quan tương tác của các hệ thống thiết bị quan trắc địa kỹ thuật, vật lý cảm biến, cấu trúc mạng thu thập dữ liệu tự động, và biểu đồ chuyển vị thời gian thực.

---

<div style="background: #1e1e24; border-radius: 12px; padding: 24px; color: #f0f0f5; box-shadow: 0 8px 24px rgba(0,0,0,0.3); margin-bottom: 30px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;">
  <div style="display: flex; justify-content: space-between; align-items: center; border-bottom: 1px solid #333; padding-bottom: 16px; margin-bottom: 20px;">
    <div>
      <h2 style="margin: 0; color: #ff6b35; font-size: 22px;">🛠️ Geotech Instrumentation Sandbox</h2>
      <p style="margin: 4px 0 0 0; color: #8c8c9e; font-size: 14px;">Select an engineering scenario to simulate field instrumentation and data profiles</p>
    </div>
    <div style="display: flex; gap: 10px;">
      <button id="btn-dam" onclick="switchScenario('dam')" style="background: #ff6b35; color: white; border: none; padding: 8px 16px; border-radius: 6px; cursor: pointer; font-weight: 600;">Earth Dam Seepage</button>
      <button id="btn-excavation" onclick="switchScenario('excavation')" style="background: #2a2a35; color: #ccc; border: none; padding: 8px 16px; border-radius: 6px; cursor: pointer; font-weight: 600;">Deep Excavation</button>
      <button id="btn-slope" onclick="switchScenario('slope')" style="background: #2a2a35; color: #ccc; border: none; padding: 8px 16px; border-radius: 6px; cursor: pointer; font-weight: 600;">Slope Inclinometer</button>
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
      <div style="margin-top: 10px; display: flex; gap: 15px; font-size: 12px; color: #8c8c9e;">
        <div><span style="display:inline-block; width:10px; height:10px; background:#00e5ff; border-radius:50%; margin-right:4px;"></span> Piezometer (VWP)</div>
        <div><span style="display:inline-block; width:10px; height:10px; background:#ff4081; border-radius:50%; margin-right:4px;"></span> Inclinometer (IPI/MEMS)</div>
        <div><span style="display:inline-block; width:10px; height:10px; background:#ffea00; border-radius:50%; margin-right:4px;"></span> Extensometer / Settlement</div>
        <div><span style="display:inline-block; width:10px; height:10px; background:#00e676; border-radius:50%; margin-right:4px;"></span> Wireless Node</div>
      </div>
    </div>

    <!-- Live Telemetry & Control Panel -->
    <div style="background: #181820; border-radius: 8px; padding: 16px; border: 1px solid #2a2a35; display: flex; flex-direction: column; justify-content: space-between;">
      <div>
        <h4 style="margin: 0 0 12px 0; color: #f0f0f5; font-size: 15px; border-bottom: 1px solid #2a2a35; padding-bottom: 6px;">Live ADAS Diagnostics</h4>
        
        <div style="margin-bottom: 12px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span>Simulated Hydrostatic Head:</span>
            <strong id="val-head" style="color: #00e5ff;">18.5 m</strong>
          </label>
          <input type="range" id="slider-head" min="5" max="30" value="18.5" step="0.5" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #00e5ff;">
        </div>

        <div style="margin-bottom: 14px;">
          <label style="font-size: 12px; color: #aaa; display: flex; justify-content: space-between;">
            <span>Ground Displacement Velocity:</span>
            <strong id="val-disp" style="color: #ff4081;">1.2 mm/day</strong>
          </label>
          <input type="range" id="slider-disp" min="0" max="10" value="1.2" step="0.1" oninput="updateSimulation()" style="width: 100%; margin-top: 4px; accent-color: #ff4081;">
        </div>

        <div style="background: #121217; padding: 10px; border-radius: 6px; margin-bottom: 10px;">
          <div style="font-size: 11px; color: #888;">TARP Trigger State</div>
          <div id="tarp-badge" style="display: inline-block; padding: 3px 8px; border-radius: 4px; font-size: 12px; font-weight: bold; background: #004d40; color: #00e676; margin-top: 4px;">NORMAL (Level 0)</div>
        </div>

        <div style="font-size: 11px; color: #aaa; line-height: 1.5;">
          <div>📡 <strong>Telemetry:</strong> LoRaWAN 915 MHz</div>
          <div>🔋 <strong>Hub Battery:</strong> 3.65V (SAFT LSH20)</div>
          <div>📶 <strong>RSSI:</strong> -42 dBm (Excellent)</div>
          <div>⏱️ <strong>Interval:</strong> 15 mins (Continuous)</div>
        </div>
      </div>

      <div id="sensor-readout-box" style="background: #0d0d11; padding: 10px; border-radius: 6px; border-left: 3px solid #ff6b35; font-family: monospace; font-size: 11px; color: #e0e0e0;">
        P_vw1: 181.4 kPa<br>
        T_vw1: 14.2 °C<br>
        Incli_max: 3.4 mm @ -12m
      </div>
    </div>
  </div>
</div>

<script>
let currentScenario = 'dam';

function switchScenario(sc) {
  currentScenario = sc;
  document.getElementById('btn-dam').style.background = sc === 'dam' ? '#ff6b35' : '#2a2a35';
  document.getElementById('btn-dam').style.color = sc === 'dam' ? 'white' : '#ccc';
  document.getElementById('btn-excavation').style.background = sc === 'excavation' ? '#ff6b35' : '#2a2a35';
  document.getElementById('btn-excavation').style.color = sc === 'excavation' ? 'white' : '#ccc';
  document.getElementById('btn-slope').style.background = sc === 'slope' ? '#ff6b35' : '#2a2a35';
  document.getElementById('btn-slope').style.color = sc === 'slope' ? 'white' : '#ccc';
  
  if (sc === 'dam') {
    document.getElementById('scenario-tag').innerText = 'Earth Embankment Dam (Dunnicliff Ch. 21)';
  } else if (sc === 'excavation') {
    document.getElementById('scenario-tag').innerText = 'Braced Deep Excavation & Wall (Dunnicliff Ch. 19)';
  } else {
    document.getElementById('scenario-tag').innerText = 'Slope Stability & Shear Plane Profiling (Dunnicliff Ch. 22)';
  }
  renderScene();
}

function updateSimulation() {
  const head = parseFloat(document.getElementById('slider-head').value);
  const disp = parseFloat(document.getElementById('slider-disp').value);
  document.getElementById('val-head').innerText = head.toFixed(1) + ' m';
  document.getElementById('val-disp').innerText = disp.toFixed(1) + ' mm/day';

  const badge = document.getElementById('tarp-badge');
  if (disp > 5.0 || head > 25.0) {
    badge.innerText = 'ACTION REQUIRED (Level 2 - Red)';
    badge.style.background = '#b71c1c';
    badge.style.color = '#ff8a80';
  } else if (disp > 2.5 || head > 20.0) {
    badge.innerText = 'ALERT (Level 1 - Amber)';
    badge.style.background = '#e65100';
    badge.style.color = '#ffd180';
  } else {
    badge.innerText = 'NORMAL (Level 0 - Green)';
    badge.style.background = '#004d40';
    badge.style.color = '#00e676';
  }

  const pKpa = (head * 9.81).toFixed(1);
  const readout = document.getElementById('sensor-readout-box');
  readout.innerHTML = `P_pore: ${pKpa} kPa<br>Disp_rate: ${disp.toFixed(1)} mm/d<br>Sweep: 2145 Hz (Linear)`;
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
  } else {
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
  }
}

switchScenario('dam');
</script>

---

## 🏗️ Kiến trúc viễn đo ADAS từ đầu đến cuối

Sơ đồ dưới đây minh họa cách các cảm biến hiện trường kết nối vào kiến trúc trí tuệ đám mây không dây:

```mermaid
graph TD
    subgraph Subsurface_Sensors["1. Subsurface Instruments"]
        VWP["Vibrating Wire Piezometers<br/>(VW2100 / VMP)"]
        IPI["In-Place Inclinometers<br/>(MEMS / Digital Bus)"]
        MPBX["Multi-Point Extensometers<br/>(Rod / Magnetic)"]
        LC["Load Cells & Strain Gauges<br/>(VW Load Cells / VWSG)"]
        SAA["Shape array<br/>(SAA3D deformations)"]
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

    DT -->|Low-Power RF| L900
    L900 -->|Wireless Mesh| HUB
    CR6 -->|Modbus / SDI-12| HUB
    
    HUB -->|MQTT / HTTPS TLS| GEO
    GEO --> CALC
    GEO --> TARP
    GEO --> GTI
```
