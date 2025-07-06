<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>System Breach</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      background-color: black;
      font-family: 'Courier New', monospace;
      overflow: hidden;
      color: #00ff00;
    }

    canvas {
      position: fixed;
      top: 0;
      left: 0;
      z-index: -10;
    }

    #terminal {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      max-width: 90%;
    }

    .centered-line {
      margin: 10px 0;
    }

    .red {
      color: red;
    }

    .loading-bar {
      width: 80%;
      max-width: 300px;
      height: 12px;
      border: 1px solid red;
      margin: 10px auto;
      background: rgba(255, 0, 0, 0.1);
    }

    .bar-fill {
      width: 0%;
      height: 100%;
      background-color: red;
    }

    pre {
      white-space: pre-wrap;
    }
  </style>
</head>
<body>

<canvas id="matrix"></canvas>
<div id="terminal"></div>

<audio id="typeSound" src="https://cdn.pixabay.com/download/audio/2022/10/20/audio_6cd82ba69a.mp3?filename=spooky-typewriter-echo-122744.mp3"></audio>
<audio id="beep" src="https://actions.google.com/sounds/v1/alarms/beep_short.ogg"></audio>
<audio id="granted" src="https://www.soundjay.com/buttons/sounds/button-3.mp3"></audio>
<audio id="alarm" src="https://assets.mixkit.co/sfx/preview/mixkit-alarm-tone-996.mp3"></audio>
<audio id="glitch" src="https://cdn.pixabay.com/download/audio/2022/10/31/audio_fdf2be6355.mp3?filename=glitch-2-109723.mp3"></audio>
<audio id="evilLaugh" src="https://cdn.pixabay.com/download/audio/2023/01/31/audio_41d57de4f3.mp3?filename=evil-laugh-139873.mp3"></audio>

<script>
  // ✅ BINARY RAIN EFFECT
  const canvas = document.getElementById("matrix");
  const ctx = canvas.getContext("2d");
  canvas.height = window.innerHeight;
  canvas.width = window.innerWidth;

  const binary = "01";
  const columns = Math.floor(canvas.width / 10);
  const drops = Array(columns).fill(1);

  function drawRain() {
    ctx.fillStyle = "rgba(0, 0, 0, 0.05)";
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = "#0f0";
    ctx.font = "14px monospace";

    for (let i = 0; i < drops.length; i++) {
      const text = binary.charAt(Math.floor(Math.random() * binary.length));
      ctx.fillText(text, i * 10, drops[i] * 10);
      if (drops[i] * 10 > canvas.height && Math.random() > 0.975) {
        drops[i] = 0;
      }
      drops[i]++;
    }
  }

  setInterval(drawRain, 35);

  // ✅ TERMINAL SIMULATION
  const terminal = document.getElementById("terminal");
  const typeSound = document.getElementById("typeSound");
  const beep = document.getElementById("beep");
  const granted = document.getElementById("granted");
  const alarm = document.getElementById("alarm");
  const glitch = document.getElementById("glitch");
  const evilLaugh = document.getElementById("evilLaugh");

  const lines = [
    "> boot --secure",
    "> connect -root mainframe",
    "> inject_payload -bypass",
    "> access --override admin",
    "[ACCESS GRANTED]",
    "> sending_payload --size 2.6GB",
    "LOADING_BAR",
    "[FIREWALL] 🔥 BREACH DETECTED 🔥",
    "[ALERT] FBI tracing signal...",
    "[WARNING] Location ping received...",
    "[EXEC] Remote self-destruct triggered",
    "HTML:<div class='centered-line red'><pre>\
        ______\n\
     .-'      '-.\n\
    /            \\\n\
   |              |\n\
   |,  .-.  .-.  ,|\n\
   | )(_o/  \\o_)( |\n\
   |/     /\\     \\|\n\
   (_     ^^     _)\n\
    \\__|IIIIII|__/\n\
     | \\IIIIII/ |\n\
     \\          /\n\
      \`--------\`\
</pre></div>",
    "HTML:<div class='centered-line red'>💀 SYSTEM BREACHED 💀</div>",
    "HTML:<div class='centered-line red'>This device is now compromised.</div>",
    "Shutting down in 3...",
    "2...",
    "1...",
    "Goodbye 👁️"
  ];

  let i = 0;

  function typeLine(text, index = 0) {
    if (text === "LOADING_BAR") {
      showLoadingBar(() => {
        terminal.innerHTML += "<div class='centered-line red'>Data sent successfully ✅</div>";
        beep.play();
        i++;
        setTimeout(() => typeLine(lines[i]), 1000);
      });
      return;
    }

    if (text.startsWith("HTML:")) {
      terminal.innerHTML += text.replace("HTML:", "");
      beep.play();
      triggerSounds(text);
      i++;
      if (i < lines.length) setTimeout(() => typeLine(lines[i]), 1200);
      return;
    }

    if (index === 0) {
      terminal.innerHTML += `<div class="centered-line" id="line-${i}"></div>`;
    }

    const lineElement = document.getElementById(`line-${i}`);
    lineElement.innerHTML += text[index];

    if (text[index] !== " ") {
      typeSound.currentTime = 0;
      typeSound.play();
    }

    if (index + 1 < text.length) {
      setTimeout(() => typeLine(text, index + 1), 25);
    } else {
      beep.play();
      triggerSounds(text);
      i++;
      if (i < lines.length) setTimeout(() => typeLine(lines[i]), 800);
    }
  }

  function showLoadingBar(callback) {
    const container = document.createElement('div');
    container.className = 'centered-line';
    container.innerHTML = `
      <span class='red'>[SENDING DATA]</span>
      <div class='loading-bar'>
        <div class='bar-fill' id='bar'></div>
      </div>
    `;
    terminal.appendChild(container);

    const bar = container.querySelector("#bar");
    let percent = 0;
    const interval = setInterval(() => {
      percent++;
      bar.style.width = percent + "%";
      if (percent >= 100) {
        clearInterval(interval);
        setTimeout(callback, 600);
      }
    }, 40);
  }

  function triggerSounds(text) {
    if (text.includes("GRANTED")) granted.play();
    if (text.includes("BREACH")) alarm.play();
    if (text.includes("FBI") || text.includes("ping")) glitch.play();
    if (text.includes("Goodbye")) {
      evilLaugh.play();
      setTimeout(() => {
        window.open('', '_self')?.close();
      }, 5000);
    }
  }

  typeLine(lines[i]);
</script>
</body>
</html>
