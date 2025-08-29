🌌 AstraFocus
<svg width="100%" height="220" viewBox="0 0 1200 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="g" cx="50%" cy="50%" r="65%">
      <stop offset="0%" stop-color="#00e5ff" stop-opacity=".95"/>
      <stop offset="60%" stop-color="#7c4dff" stop-opacity=".55"/>
      <stop offset="100%" stop-color="#0d1117" stop-opacity="0"/>
    </radialGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3.5" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- background haze -->
  <rect width="1200" height="220" fill="#0d1117"/>
  <ellipse cx="600" cy="110" rx="500" ry="120" fill="url(#g)"/>

  <!-- orbits -->
  <g fill="none" stroke="#00e5ff" stroke-opacity=".6" filter="url(#glow)">
    <ellipse cx="600" cy="110" rx="520" ry="120" stroke-width="1.2"/>
    <ellipse cx="600" cy="110" rx="420" ry="95"  stroke="#7c4dff" stroke-width="1.1"/>
    <ellipse cx="600" cy="110" rx="320" ry="70"  stroke="#14f195" stroke-width="1.0"/>
  </g>

  <!-- moving nodes -->
  <g>
    <circle r="4" fill="#00e5ff">
      <animateMotion dur="12s" repeatCount="indefinite" path="M80,110 A520,120 0 1,1 1120,110 A520,120 0 1,1 80,110"/>
    </circle>
    <circle r="4" fill="#7c4dff">
      <animateMotion dur="9s"  repeatCount="indefinite" path="M180,110 A420,95 0 1,1 1020,110 A420,95 0 1,1 180,110"/>
    </circle>
    <circle r="4" fill="#14f195">
      <animateMotion dur="7s"  repeatCount="indefinite" path="M280,110 A320,70 0 1,1 920,110 A320,70 0 1,1 280,110"/>
    </circle>
  </g>

  <!-- title -->
  <g transform="translate(0,6)">
    <text x="50%" y="110" text-anchor="middle" font-size="34" font-family="Inter,Segoe UI,Arial" fill="#e6f6ff">
      Eskinder Kassahun • AstraFocus
      <animate attributeName="opacity" values="0.8;1;0.8" dur="4s" repeatCount="indefinite"/>
    </text>
    <text x="50%" y="140" text-anchor="middle" font-size="14" fill="#9fb3c8">Cloud • DevOps • Security • AI</text>
  </g>
</svg>

Define • Do • Done

AstraFocus is my take on making productivity fun. It’s a task tracker combined with a Pomodoro timer, wrapped in a glowing cyber-theme with a live particle background. I built it to sharpen my React + TypeScript skills while creating something I’d actually use to stay focused.


What it does

Task Tracker → add, complete, and clear tasks with optional due dates

Reminders → browser notifications for deadlines

Pomodoro Timer → Focus / Short break / Long break cycles that log against active tasks

Neon UI → Animated particle background + glowing buttons that make it feel alive

Try it locally
# Clone this repo
git clone https://github.com/Eskinder185/tasktracker.git
cd tasktracker

# Install dependencies
npm install

# Start the dev server
npm start


The app will open at http://localhost:3000

 Why I built this

I didn’t just want another plain to-do app. AstraFocus is my sandbox for learning, but also something I rely on. The Pomodoro sessions help me code longer without burning out, and the neon aesthetic keeps me motivated — because if I’m staring at a screen for hours, it might as well look cool 😅.

This is a personal learning project, but if you’ve got cool ideas, feel free to fork it, tweak it, or open an issue.

📜 License

MIT © 2025 Eskinder Kassahun
