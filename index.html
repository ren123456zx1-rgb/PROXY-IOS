<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PROXY IOS</title>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;600;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    background: #08090c;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    font-family: 'Rajdhani', sans-serif;
  }
  .panel {
    width: 320px;
    background: #0f1015;
    border: 1px solid #2a2d3a;
    border-radius: 12px;
    overflow: hidden;
    position: relative;
    user-select: none;
  }
  .panel-glow-top {
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, #c9a84c, transparent);
  }
  .corner { position: absolute; width: 10px; height: 10px; }
  .corner-tl { top: 8px; left: 8px; border-top: 1px solid #c9a84c55; border-left: 1px solid #c9a84c55; }
  .corner-tr { top: 8px; right: 8px; border-top: 1px solid #c9a84c55; border-right: 1px solid #c9a84c55; }
  .corner-bl { bottom: 8px; left: 8px; border-bottom: 1px solid #c9a84c33; border-left: 1px solid #c9a84c33; }
  .corner-br { bottom: 8px; right: 8px; border-bottom: 1px solid #c9a84c33; border-right: 1px solid #c9a84c33; }

  .panel-header {
    padding: 13px 18px 11px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #1a1c25;
    background: #13141a;
  }
  .panel-title {
    font-family: 'Share Tech Mono', monospace;
    font-size: 12px;
    letter-spacing: 3px;
    color: #c9a84c;
  }
  .header-btns { display: flex; gap: 7px; }
  .hbtn {
    width: 18px; height: 18px;
    border-radius: 50%; border: none;
    cursor: pointer;
    font-size: 9px; font-weight: 700;
    display: flex; align-items: center; justify-content: center;
    transition: opacity 0.2s;
  }
  .hbtn:hover { opacity: 0.7; }
  .hbtn-min { background: #252733; color: #666; }
  .hbtn-close { background: #3a1212; color: #d94444; }

  .panel-body { padding: 6px 0; }

  .row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 12px 20px;
    border-bottom: 1px solid #0c0d12;
    transition: background 0.2s;
  }
  .row:last-child { border-bottom: none; }
  .row:hover { background: #ffffff04; }
  .row-label {
    font-size: 13px;
    font-weight: 600;
    letter-spacing: 2px;
    color: #555a72;
    text-transform: uppercase;
    transition: color 0.3s;
  }
  .row.active .row-label { color: #c8cce0; }

  .toggle { position: relative; width: 44px; height: 22px; flex-shrink: 0; }
  .toggle input { opacity: 0; width: 0; height: 0; position: absolute; }
  .slider {
    position: absolute; inset: 0;
    background: #16182080;
    border: 1px solid #252836;
    border-radius: 11px;
    cursor: pointer;
    transition: 0.35s;
  }
  .slider::before {
    content: '';
    position: absolute;
    width: 15px; height: 15px;
    left: 3px; top: 3px;
    background: #2e3248;
    border-radius: 50%;
    transition: 0.35s;
  }
  .toggle input:checked + .slider {
    background: #18180a;
    border-color: #c9a84c;
    box-shadow: 0 0 10px #c9a84c33, inset 0 0 6px #c9a84c11;
  }
  .toggle input:checked + .slider::before {
    transform: translateX(22px);
    background: #c9a84c;
    box-shadow: 0 0 8px #c9a84c88;
  }

  .target-row { padding: 10px 20px; border-bottom: 1px solid #0c0d12; display: flex; align-items: center; justify-content: space-between; }
  .target-label { font-size: 13px; font-weight: 600; letter-spacing: 2px; color: #555a72; text-transform: uppercase; }
  .dropdown-wrap { position: relative; }
  .dropdown-sel {
    background: #0b0c10;
    border: 1px solid #c9a84c;
    border-radius: 6px;
    color: #c9a84c;
    font-family: 'Share Tech Mono', monospace;
    font-size: 11px;
    padding: 5px 26px 5px 10px;
    appearance: none;
    -webkit-appearance: none;
    cursor: pointer;
    letter-spacing: 1.5px;
    min-width: 90px;
    outline: none;
    transition: box-shadow 0.2s;
  }
  .dropdown-sel:focus { box-shadow: 0 0 0 2px #c9a84c33; }
  .dropdown-arrow {
    position: absolute; right: 8px; top: 50%;
    transform: translateY(-50%);
    color: #c9a84c; pointer-events: none;
    font-size: 9px; font-family: monospace;
  }

  .divider { margin: 2px 20px; height: 1px; background: linear-gradient(90deg, #c9a84c1a, transparent); }

  .status-bar {
    padding: 9px 20px 13px;
    border-top: 1px solid #1a1c25;
    display: flex; align-items: center; gap: 8px;
    background: #0d0e13;
  }
  .status-dot {
    width: 5px; height: 5px; border-radius: 50%;
    background: #c9a84c;
    animation: pulse 2.5s ease-in-out infinite;
    flex-shrink: 0;
  }
  @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:0.25} }
  .status-text {
    font-family: 'Share Tech Mono', monospace;
    font-size: 10px;
    color: #333;
    letter-spacing: 1px;
    transition: color 0.3s;
  }
  .status-text.active { color: #c9a84c; }
</style>
</head>
<body>

<div class="panel" id="panel">
  <div class="panel-glow-top"></div>
  <div class="corner corner-tl"></div>
  <div class="corner corner-tr"></div>
  <div class="corner corner-bl"></div>
  <div class="corner corner-br"></div>

  <div class="panel-header">
    <div class="panel-title">◈ PROXY IOS</div>
    <div class="header-btns">
      <button class="hbtn hbtn-min" title="Minimize">—</button>
      <button class="hbtn hbtn-close" title="Close" onclick="document.getElementById('panel').style.display='none'">✕</button>
    </div>
  </div>

  <div class="panel-body">
    <div class="row" id="r-auto_headshot">
      <span class="row-label">Auto Headshot</span>
      <label class="toggle">
        <input type="checkbox" onchange="toggle('auto_headshot', 'AUTO HEADSHOT', this)">
        <span class="slider"></span>
      </label>
    </div>

    <div class="target-row">
      <span class="target-label">Target</span>
      <div class="dropdown-wrap">
        <select class="dropdown-sel" onchange="setTarget(this.value)">
          <option value="Head">HEAD</option>
          <option value="Neck">NECK</option>
          <option value="Body">BODY</option>
          <option value="Legs">LEGS</option>
        </select>
        <span class="dropdown-arrow">▼</span>
      </div>
    </div>

    <div class="divider"></div>

    <div class="row" id="r-drag_headshot">
      <span class="row-label">Drag Headshot</span>
      <label class="toggle">
        <input type="checkbox" onchange="toggle('drag_headshot', 'DRAG HEADSHOT', this)">
        <span class="slider"></span>
      </label>
    </div>

    <div class="row" id="r-magic_bullet">
      <span class="row-label">Magic Bullet</span>
      <label class="toggle">
        <input type="checkbox" onchange="toggle('magic_bullet', 'MAGIC BULLET', this)">
        <span class="slider"></span>
      </label>
    </div>

    <div class="row" id="r-esp_line_hack">
      <span class="row-label">Esp Line Hack</span>
      <label class="toggle">
        <input type="checkbox" onchange="toggle('esp_line_hack', 'ESP LINE HACK', this)">
        <span class="slider"></span>
      </label>
    </div>
  </div>

  <div class="status-bar">
    <div class="status-dot"></div>
    <span class="status-text" id="status">by boom</span>
  </div>
</div>

<script>
  let statusTimer = null;

  function showStatus(msg) {
    const el = document.getElementById('status');
    el.textContent = msg;
    el.classList.add('active');
    clearTimeout(statusTimer);
    statusTimer = setTimeout(() => {
      el.textContent = 'SYSTEM READY';
      el.classList.remove('active');
    }, 2500);
  }

  function toggle(key, label, cb) {
    const row = document.getElementById('r-' + key);
    row.classList.toggle('active', cb.checked);
    showStatus(label + ' — ' + (cb.checked ? 'ENABLED' : 'DISABLED'));
  }

  function setTarget(val) {
    showStatus('TARGET SET: ' + val.toUpperCase());
  }
</script>
</body>
</html>
