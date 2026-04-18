<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Madhyanagar Mediator — by Anoushka Arun | PRN: 22010126227</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=VT323:wght@400&display=swap');

  * { margin: 0; padding: 0; box-sizing: border-box; image-rendering: pixelated; }

  body {
    background: #0a0a0a;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    min-height: 100vh;
    font-family: 'Press Start 2P', monospace;
    overflow-x: hidden;
  }

  /* ── INSTRUCTION PANEL ── */
  #instructions {
    width: 100%;
    max-width: 800px;
    background: #1a1a2e;
    border: 3px solid #4a9eff;
    padding: 16px 20px;
    margin: 12px auto 6px;
    color: #a0d4ff;
    font-family: 'VT323', monospace;
    font-size: 15px;
    line-height: 1.7;
    border-radius: 4px;
  }
  #instructions h2 { color: #ffdd57; font-size: 13px; margin-bottom: 8px; letter-spacing: 2px; }
  #instructions .cols { display: flex; gap: 20px; flex-wrap: wrap; }
  #instructions .col { flex: 1; min-width: 180px; }
  #instructions .col h3 { color: #ff7eb3; font-size: 11px; margin-bottom: 6px; }
  #instructions kbd {
    background: #2a2a4e; border: 1px solid #4a9eff;
    padding: 2px 6px; border-radius: 3px;
    color: #fff; font-size: 13px;
  }
  #instructions .tip { color: #7dffb3; margin-top: 8px; font-size: 14px; }

  /* ── GAME WRAPPER ── */
  #game-wrapper {
    position: relative;
    width: 480px;
    background: #2d4a1e;
    border: 6px solid #1a1a1a;
    border-radius: 16px 16px 40px 40px;
    padding: 10px 10px 30px;
    box-shadow: 0 0 40px #00ff4433, 0 20px 60px #000;
    margin-bottom: 10px;
  }

  /* Nokia brand bar */
  #nokia-bar {
    text-align: center;
    color: #9ab87a;
    font-size: 8px;
    letter-spacing: 6px;
    padding: 4px 0 8px;
    text-transform: uppercase;
  }

  /* Screen bezel */
  #screen-bezel {
    background: #1a2a0e;
    border: 4px solid #111;
    border-radius: 8px;
    padding: 6px;
    box-shadow: inset 0 0 20px #000a;
  }

  /* The actual game canvas area */
  #screen {
    position: relative;
    width: 460px;
    height: 320px;
    background: #9bbc0f;
    overflow: hidden;
    border-radius: 4px;
  }

  /* Scanline overlay */
  #screen::after {
    content: '';
    position: absolute;
    inset: 0;
    background: repeating-linear-gradient(
      to bottom,
      transparent 0px, transparent 2px,
      rgba(0,0,0,0.12) 2px, rgba(0,0,0,0.12) 4px
    );
    pointer-events: none;
    z-index: 100;
  }

  /* Status bar */
  #status-bar {
    background: #0f380f;
    color: #9bbc0f;
    font-size: 7px;
    padding: 3px 8px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-radius: 4px 4px 0 0;
    letter-spacing: 1px;
  }

  canvas {
    display: block;
    width: 460px;
    height: 296px;
    image-rendering: pixelated;
  }

  /* ── DIALOGUE BOX ── */
  #dialogue-box {
    display: none;
    position: absolute;
    bottom: 0; left: 0; right: 0;
    background: #0f380f;
    border-top: 3px solid #306230;
    padding: 8px 10px 6px;
    z-index: 50;
    min-height: 90px;
  }
  #dialogue-speaker {
    color: #ffdd57;
    font-size: 9px;
    margin-bottom: 5px;
    letter-spacing: 1px;
  }
  #dialogue-text {
    color: #e8f8b0;
    font-size: 8px;
    line-height: 2;
    min-height: 36px;
    font-family: 'Press Start 2P', monospace;
  }
  #dialogue-choices {
    margin-top: 6px;
    display: none;
    flex-direction: column;
    gap: 3px;
  }
  .choice-btn {
    background: #1a4a1a;
    border: 2px solid #8bac0f;
    color: #e8f8b0;
    font-family: 'Press Start 2P', monospace;
    font-size: 7px;
    padding: 6px 8px;
    cursor: pointer;
    text-align: left;
    transition: background 0.1s;
    line-height: 1.6;
  }
  .choice-btn:hover, .choice-btn.selected {
    background: #306230;
    color: #ffdd57;
  }
  #dialogue-continue {
    color: #7dffb3;
    font-size: 7px;
    text-align: right;
    margin-top: 4px;
    animation: blink 1s infinite;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  /* ── INFO POPUP (Fun Facts / Law) ── */
  #info-popup {
    display: none;
    position: absolute;
    top: 10px; left: 10px; right: 10px;
    background: #0f380f;
    border: 2px solid #8bac0f;
    padding: 10px;
    z-index: 60;
    border-radius: 4px;
  }
  #info-popup h3 { color: #ffdd57; font-size: 8px; margin-bottom: 8px; }
  #info-popup p  { color: #e8f8b0; font-size: 7px; line-height: 2.2; }
  #info-popup button {
    margin-top: 10px; background: #306230; border: 2px solid #8bac0f;
    color: #e8f8b0; font-family: 'Press Start 2P', monospace;
    font-size: 7px; padding: 6px 12px; cursor: pointer;
  }

  /* ── TRUST METERS ── */
  #trust-panel {
    display: none;
    position: absolute;
    top: 4px; right: 4px;
    background: #0f380f99;
    border: 1px solid #306230;
    padding: 5px 7px;
    z-index: 40;
    border-radius: 3px;
  }
  .trust-label { color: #8bac0f; font-size: 5px; margin-bottom: 2px; }
  .trust-bar-outer { background: #0a200a; width: 70px; height: 6px; border: 1px solid #306230; }
  .trust-bar-inner { height: 100%; background: #9bbc0f; transition: width 0.4s; }
  .trust-entry { margin-bottom: 4px; }

  /* ── D-PAD & BUTTONS ── */
  #controls {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 18px;
    padding: 0 20px;
  }
  #dpad {
    display: grid;
    grid-template-columns: repeat(3, 28px);
    grid-template-rows: repeat(3, 28px);
    gap: 2px;
  }
  .dpad-btn {
    background: #1a2a0e;
    border: 2px solid #0d1a08;
    color: #6a8a4e;
    display: flex; align-items: center; justify-content: center;
    cursor: pointer; border-radius: 3px; font-size: 10px;
    user-select: none;
    transition: background 0.1s;
  }
  .dpad-btn:active, .dpad-btn.pressed { background: #0a1206; color: #9bbc0f; }
  .dpad-center { background: #111; cursor: default; }

  #action-buttons {
    display: flex; flex-direction: column; gap: 8px; align-items: flex-end;
  }
  #action-buttons .btn-row { display: flex; gap: 8px; }
  .action-btn {
    width: 36px; height: 36px; border-radius: 50%;
    border: 3px solid #0d1a08;
    font-family: 'Press Start 2P', monospace;
    font-size: 8px; cursor: pointer;
    display: flex; align-items: center; justify-content: center;
    user-select: none; transition: transform 0.1s;
    color: #fff;
  }
  .action-btn:active { transform: scale(0.9); }
  .btn-a { background: #8b0000; }
  .btn-b { background: #00408b; }

  #small-buttons {
    display: flex; gap: 10px; justify-content: center; margin-top: 10px;
  }
  .small-btn {
    background: #1a2a0e; border: 2px solid #0d1a08;
    color: #6a8a4e; font-family: 'Press Start 2P', monospace;
    font-size: 5px; padding: 4px 10px; cursor: pointer;
    border-radius: 10px; letter-spacing: 1px;
  }

  /* ── SCORE PANEL ── */
  #score-display {
    text-align: center;
    margin-top: 4px;
    color: #4a7a2e;
    font-size: 6px;
    letter-spacing: 2px;
  }

  /* ── INFO CARDS BELOW GAME ── */
  #info-cards {
    width: 100%;
    max-width: 800px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 12px;
    margin: 8px auto 20px;
    padding: 0 10px;
  }
  .info-card {
    background: #0f1a0a;
    border: 2px solid #306230;
    border-radius: 6px;
    padding: 14px;
    font-family: 'VT323', monospace;
  }
  .info-card h3 {
    font-family: 'Press Start 2P', monospace;
    font-size: 8px;
    color: #ffdd57;
    margin-bottom: 8px;
    letter-spacing: 1px;
  }
  .info-card p, .info-card li {
    color: #9bbc0f;
    font-size: 14px;
    line-height: 1.6;
  }
  .info-card ul { padding-left: 16px; }
  .info-card .tag {
    display: inline-block;
    background: #1a4a1a;
    color: #7dffb3;
    font-size: 11px;
    padding: 2px 6px;
    border-radius: 3px;
    margin: 2px 2px 0 0;
  }

  /* Title screen overlay */
  #title-screen {
    position: absolute;
    inset: 0;
    background: #9bbc0f;
    z-index: 200;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    cursor: pointer;
  }

  /* End screen */
  #end-screen {
    display: none;
    position: absolute;
    inset: 0;
    background: #0f380f;
    z-index: 200;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 20px;
    text-align: center;
  }

  @media (max-width: 520px) {
    #game-wrapper { width: 100vw; border-radius: 0; }
    #screen { width: 100%; }
    canvas { width: 100%; }
    #instructions .cols { flex-direction: column; }
  }
</style>
</head>
<body>

<!-- ═══════════════════════════════════════════════════════
     INSTRUCTIONS PANEL (for teachers / non-tech players)
═══════════════════════════════════════════════════════ -->
<div id="instructions">
  <h2>📋 HOW TO PLAY — MADHYANAGAR MEDIATOR &nbsp;|&nbsp; <span style="color:#7dffb3;">Anoushka Arun · PRN 22010126227</span></h2>
  <div class="cols">
    <div class="col">
      <h3>⌨️ KEYBOARD</h3>
      <kbd>↑ ↓ ← →</kbd> Move Arjun around<br>
      <kbd>Enter</kbd> or <kbd>A</kbd> — Talk / Confirm<br>
      <kbd>↑ ↓</kbd> — Pick dialogue choices<br>
      <kbd>B</kbd> or <kbd>Esc</kbd> — Back / Skip
    </div>
    <div class="col">
      <h3>🖱️ MOUSE / TOUCH</h3>
      Use the <b>D-PAD buttons</b> on screen to walk.<br>
      Press the red <b>A button</b> to interact.<br>
      Click any <b>dialogue choice</b> to pick it.<br>
      Works on phones too!
    </div>
    <div class="col">
      <h3>🎯 GOAL</h3>
      Walk to each character and press <b>ENTER</b> to talk.<br>
      Choose any response — all choices are positive!<br>
      Complete all conversations to reach the agreement.<br>
      <span class="tip">✦ Look for ★ signs for fun facts!</span>
    </div>
  </div>
  <div class="tip">💡 TEACHER TIP: Just open this file in Chrome, Firefox, or Edge. No install needed. Click the screen to start!</div>
</div>

<!-- ═══════════════════════════════════════════════════════
     THE NOKIA-STYLE GAME DEVICE
═══════════════════════════════════════════════════════ -->
<div id="game-wrapper">
  <div id="nokia-bar">NOKIA &nbsp;·&nbsp; ANOUSHKA ARUN &nbsp;·&nbsp; PRN: 22010126227</div>
  <div id="screen-bezel">
    <div id="status-bar">
      <span id="scene-name">MADHYANAGAR CITY</span>
      <span id="time-display">10:24</span>
      <span>♦♦♦</span>
    </div>

    <!-- THE GAME SCREEN -->
    <div id="screen">
      <canvas id="gameCanvas" width="460" height="296"></canvas>

      <!-- TITLE SCREEN -->
      <div id="title-screen" onclick="startGame()">
        <div style="font-size:9px;color:#0f380f;letter-spacing:2px;margin-bottom:5px;">PRESS START</div>
        <div style="font-size:11px;color:#0f380f;font-weight:bold;text-align:center;line-height:2;margin-bottom:6px;">
          MADHYANAGAR<br>MEDIATOR
        </div>
        <div style="font-size:6px;color:#306230;text-align:center;line-height:2.4;">
          A PIXEL JUSTICE GAME<br>
          ─────────────────<br>
          <span style="color:#ffdd57;font-size:7px;">✦ Anoushka Arun ✦</span><br>
          <span style="color:#8bac0f;">PRN: 22010126227</span><br>
          ─────────────────<br>
          Walk: ARROW KEYS<br>
          Talk: ENTER or A<br>
          ─────────────────<br>
          <span style="animation:blink 1s infinite;display:inline-block;color:#ffdd57;">▶ TAP TO BEGIN ◀</span>
        </div>
      </div>

      <!-- TRUST METERS -->
      <div id="trust-panel">
        <div class="trust-entry">
          <div class="trust-label">RAMESH ♥</div>
          <div class="trust-bar-outer"><div class="trust-bar-inner" id="trust-ramesh" style="width:80%"></div></div>
        </div>
        <div class="trust-entry">
          <div class="trust-label">SUNIL ♥</div>
          <div class="trust-bar-outer"><div class="trust-bar-inner" id="trust-sunil" style="width:80%"></div></div>
        </div>
      </div>

      <!-- DIALOGUE BOX -->
      <div id="dialogue-box">
        <div id="dialogue-speaker"></div>
        <div id="dialogue-text"></div>
        <div id="dialogue-choices"></div>
        <div id="dialogue-continue">▼ ENTER to continue</div>
      </div>

      <!-- INFO POPUP -->
      <div id="info-popup">
        <h3 id="info-title">★ FUN FACT</h3>
        <p id="info-body"></p>
        <button onclick="closeInfo()">OK, GOT IT →</button>
      </div>

      <!-- END SCREEN -->
      <div id="end-screen">
        <div id="end-title" style="font-size:9px;color:#ffdd57;margin-bottom:12px;"></div>
        <div id="end-body" style="font-size:6px;color:#9bbc0f;line-height:2.4;margin-bottom:14px;white-space:pre-line;"></div>
        <div style="font-size:8px;color:#ffdd57;margin-bottom:10px;letter-spacing:1px;">✦ ANOUSHKA ARUN ✦<br><span style="font-size:6px;color:#8bac0f;">PRN: 22010126227</span></div>
        <button onclick="restartGame()" style="background:#306230;border:none;color:#9bbc0f;font-family:'Press Start 2P',monospace;font-size:6px;padding:8px 14px;cursor:pointer;">▶ PLAY AGAIN</button>
      </div>
    </div><!-- /screen -->
  </div><!-- /bezel -->

  <!-- CONTROLS -->
  <div id="controls">
    <!-- D-PAD -->
    <div id="dpad">
      <div></div>
      <div class="dpad-btn" id="btn-up"   onmousedown="pressDir('up')"   onmouseup="releaseDir()" ontouchstart="pressDir('up')"   ontouchend="releaseDir()">▲</div>
      <div></div>
      <div class="dpad-btn" id="btn-left"  onmousedown="pressDir('left')"  onmouseup="releaseDir()" ontouchstart="pressDir('left')"  ontouchend="releaseDir()">◀</div>
      <div class="dpad-btn dpad-center"></div>
      <div class="dpad-btn" id="btn-right" onmousedown="pressDir('right')" onmouseup="releaseDir()" ontouchstart="pressDir('right')" ontouchend="releaseDir()">▶</div>
      <div></div>
      <div class="dpad-btn" id="btn-down"  onmousedown="pressDir('down')"  onmouseup="releaseDir()" ontouchstart="pressDir('down')"  ontouchend="releaseDir()">▼</div>
      <div></div>
    </div>

    <!-- SELECT / START -->
    <div style="display:flex;flex-direction:column;gap:6px;align-items:center;">
      <div id="small-buttons">
        <button class="small-btn" onclick="handleB()">SELECT</button>
        <button class="small-btn" onclick="handleStart()">START</button>
      </div>
      <div id="score-display">SCORE: <span id="score-val">0</span></div>
    </div>

    <!-- A / B BUTTONS -->
    <div id="action-buttons">
      <div class="btn-row">
        <button class="action-btn btn-b" onclick="handleB()">B</button>
        <button class="action-btn btn-a" onclick="handleA()">A</button>
      </div>
    </div>
  </div><!-- /controls -->
</div><!-- /game-wrapper -->

<!-- ═══════════════════════════════════════════════════════
     INFO CARDS — MEDIATION KNOWLEDGE BASE
═══════════════════════════════════════════════════════ -->
<div id="info-cards">
  <div class="info-card">
    <h3>⚖️ WHAT IS MEDIATION?</h3>
    <p>Mediation is a <b>voluntary, confidential</b> process where a neutral third party (the mediator) helps two or more parties reach their own agreement — without a judge deciding for them.</p>
    <br>
    <p>The mediator does <b>not</b> impose a solution. They ask questions, help parties understand each other, and guide them toward a settlement they both choose freely.</p>
    <br>
    <span class="tag">Voluntary</span><span class="tag">Confidential</span><span class="tag">Party-led</span><span class="tag">Flexible</span>
  </div>

  <div class="info-card">
    <h3>🇮🇳 INDIAN LAW &amp; MEDIATION</h3>
    <ul>
      <li><b>Mediation Act, 2023</b> — India's first dedicated mediation law, making pre-litigation mediation compulsory for commercial disputes.</li>
      <li><b>Section 89, CPC</b> — Courts can refer cases to mediation, arbitration, or Lok Adalat.</li>
      <li><b>Commercial Courts Act</b> — Mandates pre-institution mediation for commercial disputes.</li>
      <li><b>Lok Adalat</b> — Free, fast people's courts that settle millions of cases yearly.</li>
      <li>Settlements in mediation are <b>final and binding</b>, equivalent to court decrees.</li>
    </ul>
  </div>

  <div class="info-card">
    <h3>💡 5 CORE PRINCIPLES</h3>
    <ul>
      <li><b>Voluntariness</b> — No one is forced to stay or agree.</li>
      <li><b>Confidentiality</b> — Nothing said in mediation is used in court.</li>
      <li><b>Impartiality</b> — The mediator favours neither side.</li>
      <li><b>Self-determination</b> — Parties decide their own outcome.</li>
      <li><b>Neutrality</b> — Mediator has no stake in the result.</li>
    </ul>
    <br>
    <p style="color:#ffdd57;font-size:12px;">Remember: A mediator is a guide, not a judge!</p>
  </div>

  <div class="info-card">
    <h3>📊 WHY MEDIATION WINS</h3>
    <ul>
      <li>⏱️ Average court case: <b>3–15 years</b> in India</li>
      <li>⚡ Average mediation: <b>1–3 sessions</b></li>
      <li>💰 Court costs: Lawyer fees + court fees + lost time</li>
      <li>🤝 Mediation: Often <b>free or low-cost</b></li>
      <li>📋 India has <b>4.7 crore</b> pending court cases</li>
      <li>✅ Mediation success rate: <b>70–80%</b> globally</li>
      <li>🔒 Relationships preserved — parties stay in control</li>
    </ul>
  </div>

  <div class="info-card">
    <h3>🌍 FUN FACTS</h3>
    <ul>
      <li>The word "mediation" comes from Latin <i>mediare</i> — "to be in the middle."</li>
      <li>Ancient India used <b>panchayats</b> — village councils — as mediators for 3,000+ years.</li>
      <li>Singapore Convention (2019): mediation settlements are now enforceable in 55+ countries — India is a signatory!</li>
      <li>Lok Adalats settled <b>1.5 crore cases</b> in a single day (National Lok Adalat, 2022).</li>
      <li>The United Nations uses mediation to resolve international conflicts.</li>
    </ul>
  </div>

  <div class="info-card">
    <h3>🎭 THE STORY SO FAR</h3>
    <p><b>Ramesh Gupta</b> runs a small tailor shop in Madhyanagar. He ordered ₹40,000 of fabric from <b>Sunil Mehta's</b> supplier depot. Ramesh claims some of the fabric was defective. Sunil says it was fine when it left his warehouse.</p>
    <br>
    <p>The case is about to become <b>#48,422</b> in a court with a 12-year backlog. <b>You</b> — Arjun Varma, certified mediator — have one chance to help them talk it out and reach a voluntary agreement.</p>
    <br>
    <p style="color:#ffdd57;font-size:12px;">Can you find the truth — and the peace?</p>
    <br>
    <p style="color:#7dffb3;font-size:13px;border-top:1px solid #306230;padding-top:8px;">Made by: <b>Anoushka Arun</b><br>PRN: 22010126227</p>
  </div>
</div>

<!-- ═══════════════════════════════════════════════════════
     JAVASCRIPT — THE GAME ENGINE
═══════════════════════════════════════════════════════ -->
<script>
// ─────────────────────────────────────
// CANVAS SETUP
// ─────────────────────────────────────
const canvas = document.getElementById('gameCanvas');
const ctx = canvas.getContext('2d');
const W = 460, H = 296;

// ─────────────────────────────────────
// PALETTE (Game Boy Green)
// ─────────────────────────────────────
const C = {
  darkest:  '#0f380f',
  dark:     '#306230',
  mid:      '#8bac0f',
  light:    '#9bbc0f',
  lightest: '#e8f8b0',
  sky:      '#8bac0f',
  white:    '#e8f8b0',
  black:    '#0f380f',
};

// ─────────────────────────────────────
// GAME STATE
// ─────────────────────────────────────
let gameStarted = false;
let scene = 'city'; // city | tailor | office | caucus | final
let frameCount = 0;
let score = 0;

let trust = { ramesh: 80, sunil: 80 };
let storyFlags = {
  metRamesh: false,
  metSunil: false,
  metMentor: false,
  rameshOpened: false,
  sunilOpened: false,
  caucusDone: false,
  agreementReached: false,
};

// ─────────────────────────────────────
// PLAYER
// ─────────────────────────────────────
let player = {
  x: 100, y: 160,
  w: 12, h: 18,
  dir: 'down',
  frame: 0,
  moving: false,
  speed: 2,
};
let keys = {};
let moveInterval = null;
let currentDir = null;

// ─────────────────────────────────────
// DIALOGUE ENGINE
// ─────────────────────────────────────
let dialogue = {
  active: false,
  speaker: '',
  lines: [],
  lineIdx: 0,
  choices: null,
  onChoice: null,
  typing: false,
  displayedText: '',
  fullText: '',
  typeTimer: null,
};

// ─────────────────────────────────────
// NPC DEFINITIONS
// ─────────────────────────────────────
const npcs = {
  city: [
    {
      id: 'mentor', label: 'Justice Devi', x: 340, y: 100,
      color: C.darkest, accentColor: '#ffdd57',
      talk: talkMentor
    },
    {
      id: 'signboard', label: '★ INFO', x: 50, y: 80,
      color: C.dark, accentColor: C.light,
      isSign: true,
      info: {
        title: '★ DID YOU KNOW?',
        body: 'India has over 4.7 crore (47 million) pending court cases. At current rates, it would take 324 years to clear the backlog! Mediation can help solve this crisis — one case at a time.'
      }
    },
  ],
  tailor: [
    {
      id: 'ramesh', label: 'Ramesh Gupta', x: 100, y: 130,
      color: C.dark, accentColor: C.lightest,
      talk: talkRamesh
    },
    {
      id: 'sign2', label: '★ LAW', x: 380, y: 80,
      color: C.dark, accentColor: C.light,
      isSign: true,
      info: {
        title: '★ MEDIATION ACT 2023',
        body: 'India\'s Mediation Act 2023 makes pre-litigation mediation mandatory for commercial disputes before filing a civil suit. Agreements reached in mediation are enforceable like court decrees!'
      }
    },
  ],
  office: [
    {
      id: 'sunil', label: 'Sunil Mehta', x: 320, y: 140,
      color: C.dark, accentColor: C.mid,
      talk: talkSunil
    },
    {
      id: 'sign3', label: '★ FACT', x: 60, y: 70,
      color: C.dark, accentColor: C.light,
      isSign: true,
      info: {
        title: '★ VOLUNTARY PROCESS',
        body: 'Mediation is 100% voluntary. Either party can walk away at any time without penalty. This is what makes it powerful — both parties CHOOSE to stay and find a solution. The mediator NEVER forces an outcome.'
      }
    },
  ],
  caucus: [
    {
      id: 'ramesh-c', label: 'Ramesh (Private)', x: 130, y: 150,
      color: C.dark, accentColor: C.lightest,
      talk: talkCaucusRamesh
    },
    {
      id: 'sunil-c', label: 'Sunil (Private)', x: 310, y: 150,
      color: C.dark, accentColor: C.mid,
      talk: talkCaucusSunil
    },
  ],
  final: [
    {
      id: 'agreement', label: 'Sign Agreement', x: 220, y: 160,
      color: C.dark, accentColor: '#ffdd57',
      talk: talkFinal
    },
  ],
};

// ─────────────────────────────────────
// SCENE DOORS / TRANSITIONS
// ─────────────────────────────────────
const doors = {
  city: [
    { x: 150, y: 200, w: 30, h: 10, label: 'Tailor Shop', to: 'tailor', playerX: 220, playerY: 240 },
    { x: 300, y: 200, w: 30, h: 10, label: 'Office', to: 'office', playerX: 220, playerY: 240 },
  ],
  tailor: [
    { x: 20, y: 240, w: 30, h: 10, label: 'Exit', to: 'city', playerX: 160, playerY: 210 },
    { x: 380, y: 240, w: 30, h: 10, label: 'Mediation Room', to: 'caucus', playerX: 220, playerY: 50, cond: ()=>storyFlags.metRamesh },
  ],
  office: [
    { x: 20, y: 240, w: 30, h: 10, label: 'Exit', to: 'city', playerX: 310, playerY: 210 },
    { x: 380, y: 240, w: 30, h: 10, label: 'Mediation Room', to: 'caucus', playerX: 220, playerY: 50, cond: ()=>storyFlags.metSunil },
  ],
  caucus: [
    { x: 20, y: 240, w: 30, h: 10, label: 'Final Room', to: 'final', playerX: 220, playerY: 50, cond: ()=>storyFlags.caucusDone },
  ],
  final: [],
};

// ─────────────────────────────────────────────────────────
// ★ DIALOGUE TREES
// ─────────────────────────────────────────────────────────

function talkMentor() {
  if (storyFlags.metMentor) {
    showDialogue('Justice Devi', [
      'Remember Arjun — listen first. Understand both sides.',
      'Visit Ramesh at the Tailor Shop, then Sunil at the Office.',
      'Once both have spoken, bring them to the Mediation Chamber.',
    ]);
    return;
  }
  storyFlags.metMentor = true;
  addScore(10);
  showDialogue('Justice Devi', [
    'Arjun! Finally. Case #48,421 just settled — a miracle.',
    'But case #48,422 is already here — Ramesh vs Sunil.',
    'Ramesh is a tailor. He says 30% of the fabric Sunil sold him was defective.',
    'Sunil says the fabric was perfect when it left his depot.',
    '₹40,000 is at stake. But more than money — both families depend on this.',
    'YOUR ROLE: You are NOT a judge. You do not decide who is right.',
    'You help them TALK. You help them UNDERSTAND each other.',
    'Then — if they choose — you help them write their own agreement.',
    'Go to the Tailor Shop. Meet Ramesh. Then visit Sunil at the Office.',
    'Remember: LISTEN. REFLECT. NEVER IMPOSE.',
  ]);
  showInfoAfterDialogue({
    title: '★ THE MEDIATOR\'S ROLE',
    body: 'A mediator is like a skilled bridge-builder. They do not walk across the bridge for you — they help YOU build it and walk across together. The mediator asks open questions, reflects feelings, and creates a safe space for honest conversation.'
  });
}

function talkRamesh() {
  if (storyFlags.rameshOpened) {
    showDialogue('Ramesh Gupta', [
      'Thank you for listening, Arjun.',
      'I feel much calmer now. Head to the Mediation Room when ready.',
    ]);
    return;
  }
  storyFlags.metRamesh = true;
  showDialogue('Ramesh Gupta', [
    '(nervously fidgeting with fabric samples)',
    'You\'re the mediator? I was told you\'d come.',
    'Look — I ordered 500 metres of cotton from Sunil\'s depot. ₹40,000.',
    'When I started cutting, some rolls had weak threads. Customer shirts were tearing!',
    'I lost three big orders. My reputation — badly hurt.',
    'I asked Sunil to refund ₹12,000 for the defective portion. He said no.',
    'He thinks I\'m lying. But I have the torn samples right here!',
    '(pauses) Honestly... I just want acknowledgment. And the money I lost back.',
    'Do you think this can really be resolved without going to court?',
  ], [
    { text: '✦ I hear you, Ramesh. It sounds like you felt financially hurt AND personally accused. Both feelings are valid.', good: true, who: 'ramesh', delta: 10 },
    { text: '✦ Can you tell me more about what a fair outcome would look like for you?', good: true, who: 'ramesh', delta: 10 },
  ], (choice) => {
    storyFlags.rameshOpened = true;
    addScore(20);
    trust.ramesh = Math.min(100, trust.ramesh + 10);
    updateTrustBars();
    showDialogue('Ramesh Gupta', [
      '(visibly relaxing)',
      'Yes... exactly. Not just the money. He made me feel like a LIAR.',
      'If he just acknowledges that something went wrong — I\'d even take less.',
      'Thank you for actually listening to me. Nobody does that anymore.',
      'The Mediation Room is through that door on the right. I\'ll be there.',
    ]);
    showInfoAfterDialogue({
      title: '★ ACTIVE LISTENING',
      body: 'A mediator\'s most powerful tool is ACTIVE LISTENING — reflecting back what someone says without judgment. "I hear that you felt accused" is more powerful than "I\'ll fix this." It validates the person\'s experience and builds trust instantly.'
    });
  });
}

function talkSunil() {
  if (storyFlags.sunilOpened) {
    showDialogue('Sunil Mehta', [
      'I appreciate you coming here, Arjun.',
      'I hope Ramesh is ready to talk reasonably. Meet us in the Mediation Room.',
    ]);
    return;
  }
  storyFlags.metSunil = true;
  showDialogue('Sunil Mehta', [
    '(standing with arms crossed)',
    'So you\'re the mediator. I don\'t know if this will work.',
    'My depot has been running for 15 years. FIFTEEN YEARS. No complaints.',
    'Ramesh orders fabric, pays, takes it. Two months later — suddenly defective?',
    'I think it may have been stored wrong. Humidity, pests, improper folding.',
    'AND he wants ₹12,000 back? That\'s a quarter of the order value!',
    '(voice softens slightly)',
    'Look... Ramesh and I used to be friends. Our families know each other.',
    'If I\'m somehow wrong... I need to know HOW. Proof. Not just accusations.',
    'I just want fairness. And to keep my reputation intact.',
  ], [
    { text: '✦ Sunil, it sounds like your reputation and your friendship both matter here — not just the money.', good: true, who: 'sunil', delta: 10 },
    { text: '✦ What would a fair outcome look like for you, if we find the truth together?', good: true, who: 'sunil', delta: 10 },
  ], (choice) => {
    storyFlags.sunilOpened = true;
    addScore(20);
    trust.sunil = Math.min(100, trust.sunil + 10);
    updateTrustBars();
    showDialogue('Sunil Mehta', [
      '(uncrossing arms slowly)',
      'Reputation... yes. And Ramesh. We grew up in the same mohalla.',
      'I don\'t want to DESTROY him. I just don\'t want to be wrongly blamed.',
      'If there\'s a way to figure out what actually happened...',
      'Maybe a joint inspection. Maybe I give him some credit on the next order.',
      'I\'m willing to try. Where is the mediation room?',
    ]);
    showInfoAfterDialogue({
      title: '★ INTERESTS VS POSITIONS',
      body: 'POSITION: "I want ₹12,000 back." INTEREST: "I want to feel respected and recover my loss." Great mediators dig past positions to find underlying interests. Sunil\'s real interest is reputation and fairness — not just money. When you find shared interests, solutions appear!'
    });
  });
}

function talkCaucusRamesh() {
  showDialogue('Ramesh (Private Caucus)', [
    'Good — this is just between us. That\'s how caucus works in mediation.',
    'Okay. Honestly? I may have overstated it a little. I was very angry.',
    'It was probably 15-20% defective, not 30%.',
    'What I really want: ₹8,000 credit and to keep buying from Sunil.',
    'His fabric is actually the best in the city.',
    'I don\'t want to lose him as a supplier. Can you help me say that?',
    'Thank you for making this a safe space, Arjun.',
  ]);
  addScore(15);
  trust.ramesh = Math.min(100, trust.ramesh + 8);
  updateTrustBars();
  showInfoAfterDialogue({
    title: '★ THE PRIVATE CAUCUS',
    body: 'A caucus is a private meeting between the mediator and one party. What\'s said in caucus stays confidential UNLESS the party gives permission to share. This allows parties to speak honestly — revealing real interests they\'d never share in front of the other side.'
  });
}

function talkCaucusSunil() {
  if (!storyFlags.caucusDone) {
    showDialogue('Sunil (Private Caucus)', [
      'Alright. Just between us.',
      'I had a new warehouse worker that month. Some mistakes may have happened.',
      'I can\'t say that publicly — but I\'m not 100% certain the fabric was perfect.',
      'Here is what I can offer: ₹8,000 credit on his next order.',
      'AND a joint quality inspection going forward — so we both know the standard.',
      'No blame. Just solutions. That\'s what I want.',
      'I\'m glad you came to us before we ended up in court.',
    ]);
    storyFlags.caucusDone = true;
    addScore(20);
    trust.sunil = Math.min(100, trust.sunil + 8);
    updateTrustBars();
    showInfoAfterDialogue({
      title: '★ ZONE OF POSSIBLE AGREEMENT',
      body: 'The ZOPA (Zone of Possible Agreement) is the overlap between what each party is willing to accept. Ramesh wants ₹8,000 credit. Sunil is willing to give ₹8,000 credit. The ZOPA exists! A skilled mediator finds this overlap and helps both parties walk into it together.'
    });
  } else {
    showDialogue('Sunil (Private Caucus)', [
      'I\'ve said what I can say.',
      'I trust you to bridge us — I\'m ready if Ramesh is.',
    ]);
  }
}

function talkFinal() {
  storyFlags.agreementReached = true;
  showDialogue('MEDIATION CHAMBER', [
    'You bring Ramesh and Sunil to the table for the joint session.',
    'You summarise what both shared — with their permission.',
    '"Sunil will credit ₹8,000 on the next fabric order."',
    '"Ramesh withdraws the complaint and continues the business relationship."',
    '"Both agree to a joint quality inspection protocol going forward."',
    '(A long pause. Both men look at each other across the table.)',
    'Ramesh: "I may have overstated things. I was frustrated. I\'m sorry."',
    'Sunil: "I may have had a warehouse issue that month. I\'m sorry too."',
    '(They shake hands. You slide the agreement across the table.)',
    'Both men sign. Case #48,422 — RESOLVED.',
    'Ramesh: "Thank you, Arjun — and thank Anoushka Arun for training you!"',
    'Sunil: "Yes — tell your mentor Anoushka she taught you well. PRN 22010126227!"',
    'Justice Devi appears in the doorway, nodding slowly with a smile.',
    '"This is why we mediate, Arjun. Not to win. To heal."',
    '"Congratulations. You have done Madhyanagar proud."',
  ]);
  setTimeout(() => {
    showEndScreen(true);
  }, 26000);
}

// ─────────────────────────────────────
// DIALOGUE ENGINE FUNCTIONS
// ─────────────────────────────────────
let pendingInfo = null;

function showInfoAfterDialogue(info) {
  pendingInfo = info;
}

function showDialogue(speaker, lines, choices, onChoice) {
  dialogue.active = true;
  dialogue.speaker = speaker;
  dialogue.lines = lines;
  dialogue.lineIdx = 0;
  dialogue.choices = choices || null;
  dialogue.onChoice = onChoice || null;
  dialogue.typing = false;

  const box = document.getElementById('dialogue-box');
  box.style.display = 'block';
  document.getElementById('trust-panel').style.display = 'block';
  document.getElementById('dialogue-speaker').textContent = '▶ ' + speaker;
  document.getElementById('dialogue-choices').style.display = 'none';
  document.getElementById('dialogue-continue').style.display = 'block';

  showLine(lines[0]);
}

function showLine(text) {
  const el = document.getElementById('dialogue-text');
  const cont = document.getElementById('dialogue-continue');
  el.textContent = '';
  cont.style.display = 'none';

  let i = 0;
  dialogue.typing = true;
  if (dialogue.typeTimer) clearInterval(dialogue.typeTimer);
  dialogue.typeTimer = setInterval(() => {
    if (i < text.length) {
      el.textContent += text[i++];
    } else {
      clearInterval(dialogue.typeTimer);
      dialogue.typing = false;
      // Last line — show choices or continue
      const isLast = dialogue.lineIdx === dialogue.lines.length - 1;
      if (isLast && dialogue.choices) {
        showChoices();
      } else {
        cont.style.display = 'block';
        cont.textContent = isLast ? '▼ ENTER to close' : '▼ ENTER to continue';
      }
    }
  }, 28);
}

function showChoices() {
  const cont = document.getElementById('dialogue-continue');
  const choiceDiv = document.getElementById('dialogue-choices');
  cont.style.display = 'none';
  choiceDiv.style.display = 'flex';
  choiceDiv.innerHTML = '';

  dialogue.choices.forEach((c, i) => {
    const btn = document.createElement('button');
    btn.className = 'choice-btn';
    btn.textContent = (i+1) + '. ' + c.text;
    btn.onclick = () => selectChoice(c);
    choiceDiv.appendChild(btn);
  });
}

function selectChoice(choice) {
  // Apply trust change
  if (choice.who && choice.delta) {
    trust[choice.who] = Math.max(0, Math.min(100, trust[choice.who] + choice.delta));
    updateTrustBars();
  }
  document.getElementById('dialogue-choices').style.display = 'none';
  if (dialogue.onChoice) dialogue.onChoice(choice);
}

function advanceDialogue() {
  if (dialogue.typing) {
    // Skip typing
    if (dialogue.typeTimer) clearInterval(dialogue.typeTimer);
    const isLast = dialogue.lineIdx === dialogue.lines.length - 1;
    const text = dialogue.lines[dialogue.lineIdx];
    document.getElementById('dialogue-text').textContent = text;
    dialogue.typing = false;
    if (isLast && dialogue.choices) {
      showChoices();
    } else {
      const cont = document.getElementById('dialogue-continue');
      cont.style.display = 'block';
      cont.textContent = isLast ? '▼ ENTER to close' : '▼ ENTER to continue';
    }
    return;
  }

  dialogue.lineIdx++;
  if (dialogue.lineIdx < dialogue.lines.length) {
    showLine(dialogue.lines[dialogue.lineIdx]);
  } else {
    closeDialogue();
  }
}

function closeDialogue() {
  dialogue.active = false;
  document.getElementById('dialogue-box').style.display = 'none';
  document.getElementById('dialogue-choices').style.display = 'none';

  if (pendingInfo) {
    setTimeout(() => {
      showInfo(pendingInfo.title, pendingInfo.body);
      pendingInfo = null;
    }, 400);
  }
}

function showInfo(title, body) {
  document.getElementById('info-title').textContent = title;
  document.getElementById('info-body').textContent = body;
  document.getElementById('info-popup').style.display = 'block';
}

function closeInfo() {
  document.getElementById('info-popup').style.display = 'none';
}

function updateTrustBars() {
  document.getElementById('trust-ramesh').style.width = trust.ramesh + '%';
  document.getElementById('trust-sunil').style.width = trust.sunil + '%';
}

// ─────────────────────────────────────
// SCORE
// ─────────────────────────────────────
function addScore(n) {
  score = Math.max(0, score + n);
  document.getElementById('score-val').textContent = score;
}

// ─────────────────────────────────────
// INTERACTION — proximity check
// ─────────────────────────────────────
function tryInteract() {
  if (dialogue.active) { advanceDialogue(); return; }

  const sceneNpcs = npcs[scene] || [];
  for (const npc of sceneNpcs) {
    const dx = Math.abs(player.x - npc.x);
    const dy = Math.abs(player.y - npc.y);
    if (dx < 40 && dy < 40) {
      if (npc.isSign) {
        showInfo(npc.info.title, npc.info.body);
      } else if (npc.talk) {
        npc.talk();
      }
      return;
    }
  }

  // Check doors
  const sceneDoors = doors[scene] || [];
  for (const door of sceneDoors) {
    const dx = Math.abs(player.x - (door.x + door.w/2));
    const dy = Math.abs(player.y - door.y);
    if (dx < 40 && dy < 40) {
      if (door.cond && !door.cond()) {
        showInfo('🚪 DOOR LOCKED', 'You need to meet with the parties first before proceeding. Complete the conversations!');
        return;
      }
      transitionScene(door.to, door.playerX, door.playerY);
      return;
    }
  }
}

function transitionScene(to, px, py) {
  scene = to;
  player.x = px || 220;
  player.y = py || 150;
  document.getElementById('scene-name').textContent = sceneNames[to] || to.toUpperCase();
  dialogue.active = false;
  document.getElementById('dialogue-box').style.display = 'none';
}

const sceneNames = {
  city: 'MADHYANAGAR CITY',
  tailor: 'RAMESH\'S TAILOR SHOP',
  office: 'SUNIL\'S DEPOT OFFICE',
  caucus: 'PRIVATE CAUCUS ROOM',
  final: 'MEDIATION CHAMBER',
};

// ─────────────────────────────────────
// END SCREEN
// ─────────────────────────────────────
function showEndScreen(success) {
  const el = document.getElementById('end-screen');
  el.style.display = 'flex';
  document.getElementById('end-title').textContent = '🎉 CASE RESOLVED!';
  document.getElementById('end-body').innerHTML =
    'FINAL SCORE: ' + score + '\n\n' +
    'Ramesh & Sunil signed a voluntary agreement.\n' +
    'Case #48,422 never reached court.\n\n' +
    '✦ ₹8,000 credit issued\n' +
    '✦ Business relationship preserved\n' +
    '✦ Joint quality protocol established\n' +
    '✦ Friendship renewed\n\n' +
    '─────────────────────\n' +
    'Created by:\n' +
    'ANOUSHKA ARUN\n' +
    'PRN: 22010126227\n' +
    '─────────────────────\n' +
    '"Justice doesn\'t always wear a robe.\n Sometimes it wears patience."\n' +
    '— Justice Devi';
}

function restartGame() {
  score = 0;
  trust = { ramesh: 80, sunil: 80 };
  storyFlags = { metRamesh:false, metSunil:false, metMentor:false, rameshOpened:false, sunilOpened:false, caucusDone:false, agreementReached:false };
  player = { x:100, y:160, w:12, h:18, dir:'down', frame:0, moving:false, speed:2 };
  scene = 'city';
  document.getElementById('end-screen').style.display = 'none';
  document.getElementById('trust-panel').style.display = 'none';
  document.getElementById('dialogue-box').style.display = 'none';
  document.getElementById('info-popup').style.display = 'none';
  document.getElementById('score-val').textContent = '0';
  updateTrustBars();
}

// ─────────────────────────────────────
// DRAWING — PIXEL ART SCENES
// ─────────────────────────────────────
function drawScene() {
  ctx.clearRect(0, 0, W, H);
  if (scene === 'city') drawCity();
  else if (scene === 'tailor') drawTailor();
  else if (scene === 'office') drawOffice();
  else if (scene === 'caucus') drawCaucus();
  else if (scene === 'final') drawFinal();

  drawDoorLabels();
  drawNPCs();
  drawPlayer();
  drawProximityHints();
}

// ── pixel helpers ──
function pxRect(x, y, w, h, fill, stroke) {
  ctx.fillStyle = fill;
  ctx.fillRect(Math.round(x), Math.round(y), w, h);
  if (stroke) { ctx.strokeStyle = stroke; ctx.lineWidth = 2; ctx.strokeRect(Math.round(x)+1, Math.round(y)+1, w-2, h-2); }
}
function pxText(text, x, y, color, size) {
  ctx.fillStyle = color || C.dark;
  ctx.font = `${size||7}px 'Press Start 2P'`;
  ctx.fillText(text, Math.round(x), Math.round(y));
}
function pxWindow(x, y, w, h) {
  pxRect(x, y, w, h, C.mid);
  pxRect(x+2, y+2, w-4, h/2-2, C.lightest);
  pxRect(x+2, y+h/2, w-4, h/2-2, C.light);
}

// ── CITY SCENE ──
function drawCity() {
  // Sky
  pxRect(0, 0, W, 80, C.mid);
  // Ground
  pxRect(0, 80, W, H-80, C.light);
  // Road
  pxRect(0, 180, W, 40, C.dark);
  // Road dashes
  for (let x = 0; x < W; x += 40) {
    pxRect(x, 198, 20, 4, C.mid);
  }

  // --- Courthouse Building ---
  pxRect(20, 50, 100, 130, '#8bac0f');
  pxRect(30, 50, 80, 15, C.darkest); // roof
  for (let c = 0; c < 4; c++) { pxRect(32+c*18, 65, 8, 60, C.mid); } // columns
  pxRect(20, 125, 100, 55, '#8bac0f');
  pxRect(50, 140, 20, 38, C.darkest); // door
  pxWindow(28, 100, 20, 18);
  pxWindow(72, 100, 20, 18);
  // Big readable label
  pxRect(14, 46, 112, 14, C.darkest);
  pxText('⚖ COURTHOUSE', 16, 57, C.lightest, 6);

  // --- Tailor Shop ---
  pxRect(150, 80, 90, 100, C.light);
  pxRect(150, 80, 90, 18, C.dark); // awning
  pxRect(150, 178, 90, 2, C.darkest);
  pxRect(185, 120, 24, 58, C.darkest); // door
  pxWindow(158, 90, 18, 18);
  pxWindow(204, 90, 18, 18);
  pxRect(148, 62, 96, 16, C.darkest);
  pxRect(149, 63, 94, 14, '#e8f8b0');
  pxText('TAILOR SHOP', 153, 74, C.darkest, 7);

  // --- Office/Depot ---
  pxRect(300, 60, 130, 120, '#8bac0f');
  pxRect(300, 60, 130, 20, C.darkest);
  pxRect(301, 61, 128, 18, '#e8f8b0');
  pxText('SUNIL\'S DEPOT', 305, 74, C.darkest, 7);
  pxRect(355, 120, 28, 58, C.darkest);
  pxWindow(308, 88, 22, 20);
  pxWindow(338, 88, 22, 20);
  pxWindow(370, 88, 22, 20);

  // --- Justice Devi's spot ---
  pxRect(325, 85, 12, 2, '#ffdd57'); // star indicator
  pxText('★', 337, 102, '#ffdd57', 8);

  // Trees
  drawTree(260, 130); drawTree(440, 90); drawTree(85, 135);

  // Cloud
  drawCloud(frm(160, 200, 40), 20);
  drawCloud(frm(300, 350, 30), 10);

  // Signboard ★
  pxRect(40, 60, 16, 24, C.dark);
  pxRect(38, 58, 20, 10, C.darkest);
  pxText('★', 42, 67, '#ffdd57', 7);
}

// ── TAILOR SHOP SCENE ──
function drawTailor() {
  // Floor
  for (let x = 0; x < W; x += 20) {
    for (let y = 0; y < H; y += 20) {
      pxRect(x, y, 19, 19, (x+y)%40===0 ? C.light : C.mid);
    }
  }
  // Walls
  pxRect(0, 0, W, 34, C.darkest);
  pxRect(1, 1, W-2, 32, C.dark);
  pxText("RAMESH'S TAILOR SHOP", 30, 22, C.lightest, 8);

  // Sewing machines
  for (let i = 0; i < 3; i++) {
    drawSewingMachine(40 + i*90, 80);
  }

  // Fabric rolls
  for (let i = 0; i < 5; i++) {
    pxRect(10, 150+i*12, 25, 10, i%2===0 ? C.lightest : C.mid);
  }

  // Exit door
  pxRect(20, 230, 30, 30, C.darkest);
  pxText('EXIT', 22, 248, C.light, 5);

  // Right door to caucus
  if (storyFlags.metRamesh) {
    pxRect(380, 230, 60, 30, C.dark);
    pxText('MEDIATION', 382, 245, C.light, 5);
    pxText('ROOM ▶', 390, 255, '#ffdd57', 5);
  }

  // Signboard
  pxRect(370, 60, 16, 24, C.dark);
  pxRect(368, 58, 20, 10, C.darkest);
  pxText('★', 372, 67, '#ffdd57', 7);
}

function drawSewingMachine(x, y) {
  pxRect(x, y, 50, 35, C.darkest);
  pxRect(x+2, y+2, 46, 20, C.dark);
  pxRect(x+20, y+5, 10, 15, C.mid); // needle area
  pxRect(x, y+35, 50, 8, C.mid); // base
  // Wheel
  ctx.beginPath(); ctx.arc(x+42, y+15, 8, 0, Math.PI*2);
  ctx.fillStyle = C.mid; ctx.fill();
  ctx.strokeStyle = C.darkest; ctx.lineWidth = 2; ctx.stroke();
}

// ── OFFICE SCENE ──
function drawOffice() {
  // Floor
  pxRect(0, 0, W, H, C.light);
  pxRect(0, 0, W, 36, C.darkest);
  pxRect(1, 1, W-2, 34, C.dark);
  pxText("SUNIL'S FABRIC DEPOT", 40, 24, C.lightest, 8);

  // Shelves with fabric bolts
  for (let shelf = 0; shelf < 3; shelf++) {
    pxRect(30, 50+shelf*55, 200, 10, C.dark); // shelf
    for (let bolt = 0; bolt < 6; bolt++) {
      const colors = [C.lightest, C.mid, C.dark, C.light, C.darkest, C.mid];
      pxRect(35+bolt*32, 32+shelf*55, 22, 20, colors[bolt]);
      pxRect(37+bolt*32, 34+shelf*55, 18, 16, colors[(bolt+2)%6]); // pattern
    }
  }

  // Desk
  pxRect(290, 100, 140, 70, C.darkest);
  pxRect(295, 105, 130, 60, C.dark);
  pxRect(320, 110, 40, 30, C.mid); // papers
  pxRect(380, 108, 25, 25, C.darkest); // computer monitor
  pxRect(383, 111, 19, 19, C.mid);

  // Exit
  pxRect(20, 230, 30, 30, C.darkest);
  pxText('EXIT', 22, 248, C.light, 5);

  // Right door
  if (storyFlags.metSunil) {
    pxRect(380, 230, 60, 30, C.dark);
    pxText('MEDIATION', 382, 245, C.light, 5);
    pxText('ROOM ▶', 390, 255, '#ffdd57', 5);
  }

  // Sign
  pxRect(50, 60, 16, 24, C.dark);
  pxRect(48, 58, 20, 10, C.darkest);
  pxText('★', 52, 67, '#ffdd57', 7);
}

// ── CAUCUS ROOM ──
function drawCaucus() {
  // Calm room
  pxRect(0, 0, W, H, C.mid);
  pxRect(0, 0, W, 34, C.darkest);
  pxRect(1, 1, W-2, 32, C.dark);
  pxText('PRIVATE CAUCUS ROOM', 55, 23, C.lightest, 8);

  // Two partitions
  pxRect(200, 30, 8, H-30, C.darkest);

  // Left side — Ramesh
  pxRect(10, 50, 180, 15, C.dark);
  pxText("RAMESH'S SIDE", 20, 61, C.light, 5);
  // Chair and table
  pxRect(60, 100, 80, 50, C.dark);
  pxRect(65, 105, 70, 40, C.light);

  // Right side — Sunil
  pxRect(210, 50, 230, 15, C.dark);
  pxText("SUNIL'S SIDE", 220, 61, C.light, 5);
  pxRect(270, 100, 80, 50, C.dark);
  pxRect(275, 105, 70, 40, C.light);

  // Door
  if (storyFlags.caucusDone) {
    pxRect(10, 230, 80, 30, C.dark);
    pxText('FINAL ROOM ▶', 14, 248, '#ffdd57', 5);
  }

  // Confidentiality sign
  pxRect(180, 50, 80, 30, C.darkest);
  pxText('CONFIDENTIAL', 185, 60, '#ffdd57', 4);
  pxText('ZONE', 200, 70, '#ffdd57', 4);
}

// ── FINAL MEDIATION CHAMBER ──
function drawFinal() {
  pxRect(0, 0, W, H, C.mid);
  pxRect(0, 0, W, 34, C.darkest);
  pxRect(1, 1, W-2, 32, '#1a4a1a');
  pxText('MEDIATION CHAMBER', 70, 23, '#ffdd57', 8);

  // Conference table (oval)
  ctx.beginPath();
  ctx.ellipse(230, 165, 130, 55, 0, 0, Math.PI*2);
  ctx.fillStyle = C.darkest; ctx.fill();
  ctx.beginPath();
  ctx.ellipse(230, 165, 126, 51, 0, 0, Math.PI*2);
  ctx.fillStyle = C.dark; ctx.fill();

  // Chairs around table
  const chairPos = [
    [100, 125], [160, 110], [230, 105], [300, 110], [355, 125],
    [100, 205], [160, 220], [230, 225], [300, 220], [355, 205],
  ];
  for (const [cx, cy] of chairPos) {
    pxRect(cx-8, cy-8, 16, 16, C.mid);
    pxRect(cx-6, cy-6, 12, 12, C.light);
  }

  // Document on table
  pxRect(205, 145, 50, 35, C.lightest);
  pxRect(208, 148, 44, 4, C.dark);
  pxRect(208, 155, 44, 2, C.mid);
  pxRect(208, 160, 44, 2, C.mid);
  pxRect(208, 165, 44, 2, C.mid);
  pxText('AGREEMENT', 208, 143, C.darkest, 4);

  // Pen
  pxRect(255, 155, 20, 3, C.darkest);
  pxRect(273, 153, 4, 7, C.mid);

  // ★ Sign
  pxRect(380, 50, 60, 40, C.darkest);
  pxText('SIGN TO', 385, 65, '#ffdd57', 5);
  pxText('RESOLVE', 385, 78, '#ffdd57', 5);

  // Trust meter visual - always positive
  const allGood = trust.ramesh >= 70 && trust.sunil >= 70;
  pxRect(10, 245, 440, 15, C.darkest);
  pxRect(12, 247, Math.round(436 * (trust.ramesh+trust.sunil)/200), 11, '#7dffb3');
  pxText('TRUST: READY TO SIGN THE AGREEMENT!', 14, 258, '#7dffb3', 5);
}

// ── HELPERS ──
function drawTree(x, y) {
  pxRect(x+4, y+20, 8, 20, C.darkest);
  ctx.beginPath(); ctx.arc(x+8, y+10, 14, 0, Math.PI*2);
  ctx.fillStyle = C.dark; ctx.fill();
  ctx.beginPath(); ctx.arc(x+8, y+4, 10, 0, Math.PI*2);
  ctx.fillStyle = C.darkest; ctx.fill();
}
function drawCloud(x, y) {
  ctx.beginPath(); ctx.arc(x, y+8, 12, 0, Math.PI*2);
  ctx.arc(x+14, y+4, 14, 0, Math.PI*2);
  ctx.arc(x+28, y+8, 12, 0, Math.PI*2);
  ctx.fillStyle = C.lightest; ctx.fill();
}
function frm(a, b, speed) { return a + (b-a)*(0.5 + 0.5*Math.sin(frameCount/speed)); }

function drawNPCs() {
  const sceneNpcs = npcs[scene] || [];
  for (const npc of sceneNpcs) {
    if (npc.isSign) {
      // Sign post — bigger, more visible
      pxRect(npc.x, npc.y, 6, 28, C.darkest);
      pxRect(npc.x-14, npc.y-18, 36, 18, C.darkest);
      pxRect(npc.x-12, npc.y-16, 32, 14, '#ffdd57');
      pxText('★ INFO', npc.x-10, npc.y-5, C.darkest, 6);
    } else {
      drawCharacter(npc.x, npc.y, npc.color, npc.accentColor, false, npc.label);
    }
  }
}

function drawCharacter(x, y, bodyColor, accentColor, isPlayer, label) {
  const bob = isPlayer ? 0 : Math.sin(frameCount/20 + x)*1.5;
  // Shadow
  ctx.beginPath(); ctx.ellipse(x, y+18, 7, 3, 0, 0, Math.PI*2);
  ctx.fillStyle = 'rgba(0,0,0,0.3)'; ctx.fill();
  // Legs
  pxRect(x-5, y+10+bob, 4, 9, bodyColor);
  pxRect(x+1, y+10+bob, 4, 9, bodyColor);
  // Body
  pxRect(x-6, y+bob, 12, 11, accentColor || bodyColor);
  // Head
  pxRect(x-5, y-10+bob, 10, 10, bodyColor);
  // Eyes
  pxRect(x-3, y-7+bob, 2, 2, C.lightest);
  pxRect(x+1, y-7+bob, 2, 2, C.lightest);
  // Label — big, high-contrast background pill
  if (label) {
    const lw = label.length * 7 + 8;
    pxRect(x - lw/2, y-30+bob, lw, 13, C.darkest);
    pxRect(x - lw/2 + 1, y-29+bob, lw-2, 11, accentColor === '#ffdd57' ? '#ffdd57' : C.lightest);
    pxText(label, x - lw/2 + 4, y-20+bob, C.darkest, 7);
  }
}

function drawPlayer() {
  const dir = player.dir;
  const x = player.x, y = player.y;
  const walk = player.moving ? Math.sin(frameCount/6)*2 : 0;
  // Shadow
  ctx.beginPath(); ctx.ellipse(x, y+18, 8, 3, 0, 0, Math.PI*2);
  ctx.fillStyle = 'rgba(0,0,0,0.3)'; ctx.fill();
  // Legs (animated)
  pxRect(x-5, y+10, 4, 9+walk, C.dark);
  pxRect(x+1, y+10, 4, 9-walk, C.dark);
  // Body
  pxRect(x-7, y, 14, 11, C.lightest);
  // Jacket
  pxRect(x-6, y+1, 12, 9, C.mid);
  // Head
  pxRect(x-5, y-11, 10, 11, '#c8a870');
  // Hair
  pxRect(x-5, y-11, 10, 3, C.darkest);
  // Eyes
  if (dir !== 'up') {
    pxRect(x-3, y-6, 2, 2, C.darkest);
    pxRect(x+1, y-6, 2, 2, C.darkest);
  }
  // Clipboard
  pxRect(x+6, y+2, 6, 8, C.lightest);
  pxRect(x+7, y+3, 4, 6, C.light);
  // Player label — bright yellow pill
  const plabel = 'ARJUN (YOU)';
  const pw = plabel.length * 6 + 8;
  pxRect(x - pw/2, y-26, pw, 12, C.darkest);
  pxRect(x - pw/2 + 1, y-25, pw-2, 10, '#ffdd57');
  pxText(plabel, x - pw/2 + 3, y-17, C.darkest, 6);
}

function drawDoorLabels() {
  const sceneDoors = doors[scene] || [];
  for (const d of sceneDoors) {
    const active = !d.cond || d.cond();
    // Big bright door marker
    pxRect(d.x - 5, d.y - 4, d.w + 10, d.h + 8, active ? C.darkest : '#333');
    pxRect(d.x - 3, d.y - 2, d.w + 6, d.h + 4, active ? '#ffdd57' : '#555');
    // Label above door
    const lw = d.label.length * 7 + 10;
    pxRect(d.x + d.w/2 - lw/2, d.y - 20, lw, 14, C.darkest);
    pxRect(d.x + d.w/2 - lw/2 + 1, d.y - 19, lw-2, 12, active ? '#ffdd57' : '#555');
    pxText(d.label, d.x + d.w/2 - lw/2 + 4, d.y - 9, C.darkest, 7);
  }
}

function drawProximityHints() {
  const sceneNpcs = npcs[scene] || [];
  for (const npc of sceneNpcs) {
    const dx = Math.abs(player.x - npc.x);
    const dy = Math.abs(player.y - npc.y);
    if (dx < 50 && dy < 50) {
      // Big flashing PRESS ENTER hint
      const alpha = 0.7 + 0.3 * Math.sin(frameCount / 8);
      ctx.globalAlpha = alpha;
      pxRect(npc.x - 42, npc.y - 46, 84, 16, C.darkest);
      pxRect(npc.x - 41, npc.y - 45, 82, 14, '#00ff88');
      pxText('PRESS ENTER TO TALK', npc.x - 40, npc.y - 34, C.darkest, 6);
      ctx.globalAlpha = 1;
    }
  }
  for (const d of (doors[scene]||[])) {
    const dx = Math.abs(player.x - (d.x + d.w/2));
    const dy = Math.abs(player.y - d.y);
    if (dx < 50 && dy < 50) {
      const active = !d.cond || d.cond();
      const alpha = 0.7 + 0.3 * Math.sin(frameCount / 8);
      ctx.globalAlpha = alpha;
      pxRect(d.x - 20, d.y - 32, 90, 16, C.darkest);
      pxRect(d.x - 19, d.y - 31, 88, 14, active ? '#00ff88' : '#ff6666');
      pxText(active ? 'PRESS ENTER TO ENTER' : 'TALK TO NPC FIRST!', d.x - 18, d.y - 20, C.darkest, 6);
      ctx.globalAlpha = 1;
    }
  }

  // Persistent bottom navigation guide
  drawNavGuide();
}

function drawNavGuide() {
  // Semi-transparent strip at very bottom showing what to do next
  pxRect(0, 278, W, 18, C.darkest);
  let hint = '';
  if (!storyFlags.metMentor) hint = '★ GO TALK TO JUSTICE DEVI (top right of city)';
  else if (!storyFlags.rameshOpened) hint = '▶ ENTER TAILOR SHOP → TALK TO RAMESH';
  else if (!storyFlags.sunilOpened) hint = '▶ ENTER OFFICE → TALK TO SUNIL';
  else if (!storyFlags.caucusDone) hint = '▶ GO TO MEDIATION ROOM → TALK TO BOTH';
  else if (!storyFlags.agreementReached) hint = '▶ GO TO FINAL ROOM → SIGN THE AGREEMENT!';
  else hint = '✦ CASE RESOLVED — CONGRATULATIONS! ✦';
  pxText(hint, 8, 291, '#ffdd57', 6);
}

// ─────────────────────────────────────
// MOVEMENT
// ─────────────────────────────────────
function movePlayer() {
  if (dialogue.active) return;
  let moved = false;
  const spd = player.speed;
  if (keys['ArrowUp']    || keys['w']) { player.y -= spd; player.dir='up';    moved=true; }
  if (keys['ArrowDown']  || keys['s']) { player.y += spd; player.dir='down';  moved=true; }
  if (keys['ArrowLeft']  || keys['a']) { player.x -= spd; player.dir='left';  moved=true; }
  if (keys['ArrowRight'] || keys['d']) { player.x += spd; player.dir='right'; moved=true; }
  player.x = Math.max(10, Math.min(W-10, player.x));
  player.y = Math.max(30, Math.min(H-20, player.y));
  player.moving = moved;
}

function pressDir(dir) {
  const keyMap = { up:'ArrowUp', down:'ArrowDown', left:'ArrowLeft', right:'ArrowRight' };
  keys[keyMap[dir]] = true;
  document.getElementById('btn-'+dir)?.classList.add('pressed');
}
function releaseDir() {
  keys = {};
  document.querySelectorAll('.dpad-btn').forEach(b => b.classList.remove('pressed'));
}

// ─────────────────────────────────────
// KEYBOARD
// ─────────────────────────────────────
document.addEventListener('keydown', e => {
  keys[e.key] = true;
  if (e.key === 'Enter' || e.key === 'a' || e.key === 'A') handleA();
  if (e.key === 'b' || e.key === 'B' || e.key === 'Escape') handleB();
  if (['ArrowUp','ArrowDown','ArrowLeft','ArrowRight',' '].includes(e.key)) e.preventDefault();
});
document.addEventListener('keyup', e => { keys[e.key] = false; });

function handleA() {
  if (!gameStarted) { startGame(); return; }
  tryInteract();
}
function handleB() {
  if (dialogue.active) closeDialogue();
  if (document.getElementById('info-popup').style.display === 'block') closeInfo();
}
function handleStart() { if (!gameStarted) startGame(); }

// ─────────────────────────────────────
// GAME LOOP
// ─────────────────────────────────────
function startGame() {
  gameStarted = true;
  document.getElementById('title-screen').style.display = 'none';
  document.getElementById('trust-panel').style.display = 'none';
  loop();
  // Welcome message after short delay
  setTimeout(() => {
    showInfo('WELCOME, MEDIATOR!',
      'You are Arjun Varma, a certified mediator in Madhyanagar.\n\nUse arrow keys (or D-pad) to walk. Press A or Enter to talk to characters.\n\nFind Justice Devi (★) to begin your mission!\n\nLook for ★ signs for fun facts about mediation.');
  }, 500);
}

function loop() {
  frameCount++;
  movePlayer();
  drawScene();

  // Update time display
  const mins = Math.floor(frameCount / 60) % 60;
  const hrs = 10 + Math.floor(frameCount / 3600);
  document.getElementById('time-display').textContent =
    hrs + ':' + String(mins).padStart(2,'0');

  requestAnimationFrame(loop);
}

// Pre-draw title to canvas so it's not blank
(function initCanvas() {
  pxRect(0, 0, W, H, C.light);
})();
</script>
</body>
</html>
