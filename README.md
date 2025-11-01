# matrix.svg
<svg width="800" height="200" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg" style="background:#0a0a0a; font-family: monospace;">
  <defs>
    <linearGradient id="matrixGradient" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#00ff88" stop-opacity="1"/>
      <stop offset="100%" stop-color="#003300" stop-opacity="0"/>
    </linearGradient>

    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- animação de queda -->
    <style>
      @keyframes drop1 {
        0%   { transform: translateY(-200px); opacity: 0; }
        10%  { opacity: 1; }
        90%  { opacity: 1; }
        100% { transform: translateY(220px); opacity: 0; }
      }
      @keyframes drop2 {
        0%   { transform: translateY(-250px); opacity: 0; }
        10%  { opacity: 1; }
        90%  { opacity: 1; }
        100% { transform: translateY(240px); opacity: 0; }
      }
      @keyframes drop3 {
        0%   { transform: translateY(-220px); opacity: 0; }
        10%  { opacity: 1; }
        90%  { opacity: 1; }
        100% { transform: translateY(240px); opacity: 0; }
      }
      .col {
        fill: #00ff88;
        font-size: 16px;
        filter: url(#glow);
      }
      .fade {
        fill: url(#matrixGradient);
      }
      text {
        white-space: pre;
      }
    </style>
  </defs>

  <!-- coluna 1 -->
  <g style="animation: drop1 3s linear infinite;">
    <text x="100" y="0" class="col">F</text>
    <text x="100" y="20" class="col">R</text>
    <text x="100" y="40" class="col">E</text>
    <text x="100" y="60" class="col">D</text>
    <text x="100" y="80" class="col">Y</text>
    <text x="100" y="100" class="col">1</text>
    <text x="100" y="120" class="col">0</text>
    <text x="100" y="140" class="col">1</text>
    <text x="100" y="160" class="col">0</text>
    <rect x="96" y="0" width="16" height="200" class="fade"/>
  </g>

  <!-- coluna 2 -->
  <g style="animation: drop2 3.5s linear infinite; animation-delay: .4s;">
    <text x="200" y="0" class="col">0</text>
    <text x="200" y="20" class="col">1</text>
    <text x="200" y="40" class="col">F</text>
    <text x="200" y="60" class="col">R</text>
    <text x="200" y="80" class="col">E</text>
    <text x="200" y="100" class="col">D</text>
    <text x="200" y="120" class="col">Y</text>
    <text x="200" y="140" class="col">1</text>
    <text x="200" y="160" class="col">0</text>
    <rect x="196" y="0" width="16" height="200" class="fade"/>
  </g>

  <!-- coluna 3 -->
  <g style="animation: drop3 4s linear infinite; animation-delay: .8s;">
    <text x="300" y="0" class="col">F</text>
    <text x="300" y="20" class="col">R</text>
    <text x="300" y="40" class="col">E</text>
    <text x="300" y="60" class="col">D</text>
    <text x="300" y="80" class="col">Y</text>
    <text x="300" y="100" class="col">0</text>
    <text x="300" y="120" class="col">1</text>
    <text x="300" y="140" class="col">0</text>
    <text x="300" y="160" class="col">1</text>
    <rect x="296" y="0" width="16" height="200" class="fade"/>
  </g>

  <!-- título central -->
  <text x="440" y="100" fill="#00ff88" font-size="18" text-anchor="middle" filter="url(#glow)">
    FREDY // RED TEAM // ACTIVE
  </text>

  <text x="440" y="125" fill="#007744" font-size="12" text-anchor="middle">
    scanning network . . .
  </text>

</svg>
