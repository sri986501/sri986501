<?xml version="1.0" encoding="utf-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 300" width="1000" height="300" role="img" aria-label="Profile intro">
  <defs>
    <linearGradient id="bgGrad" x1="0" x2="1">
      <stop offset="0%" stop-color="#0f1724"/>
      <stop offset="100%" stop-color="#071233"/>
    </linearGradient>

    <linearGradient id="avatarGrad" x1="0" x2="1">
      <stop offset="0%" stop-color="#4F46E5"/>
      <stop offset="100%" stop-color="#06B6D4"/>
    </linearGradient>

    <filter id="soft" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="18" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="100%" height="100%" fill="url(#bgGrad)"/>

  <!-- Subtle floating shapes -->
  <g opacity="0.12" filter="url(#soft)">
    <circle cx="150" cy="50" r="60" fill="#06B6D4">
      <animateTransform attributeName="transform" type="translate" values="0 0; 20 -10; 0 0" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="880" cy="200" r="80" fill="#4F46E5">
      <animateTransform attributeName="transform" type="translate" values="0 0; -25 10; 0 0" dur="10s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Avatar badge -->
  <g transform="translate(70,150)">
    <circle cx="0" cy="0" r="70" fill="url(#avatarGrad)">
      <animateTransform attributeName="transform" type="scale" values="0.98;1.03;0.98" dur="6s" repeatCount="indefinite"/>
    </circle>
    <text x="0" y="9" text-anchor="middle" font-family="Segoe UI, Roboto, Helvetica, Arial, sans-serif" font-size="48" font-weight="700" fill="#fff" letter-spacing="1">
      S
    </text>
    <circle cx="-40" cy="50" r="6" fill="#fff" opacity="0.06"/>
  </g>

  <!-- Text block -->
  <g transform="translate(220,95)" font-family="Segoe UI, Roboto, Helvetica, Arial, sans-serif">
    <!-- Name -->
    <text class="title" x="0" y="40" fill="#ffffff" font-size="40" font-weight="700" opacity="0">
      sri986501
      <animate attributeName="opacity" from="0" to="1" begin="0.6s" dur="0.6s" fill="freeze"/>
      <animateTransform attributeName="transform" type="translate" from="-8 0" to="0 0" begin="0.6s" dur="0.6s" fill="freeze"/>
    </text>

    <!-- Role -->
    <text x="0" y="80" fill="#a8b3c7" font-size="18" font-weight="500" opacity="0">
      Creative & Professional Frontend / Full‑stack Developer
      <animate attributeName="opacity" from="0" to="1" begin="1.2s" dur="0.6s" fill="freeze"/>
      <animateTransform attributeName="transform" type="translate" from="-6 0" to="0 0" begin="1.2s" dur="0.6s" fill="freeze"/>
    </text>

    <!-- Rotating skills (three items cycling) -->
    <g id="skills" transform="translate(0,130)" fill="#cbd5e1" font-size="20" font-weight="600">
      <text x="0" y="0" opacity="0">
        JavaScript • React • Node.js
        <animate attributeName="opacity" begin="2.1s" dur="4.5s" values="0;1;0" repeatCount="indefinite"/>
      </text>
      <text x="0" y="0" opacity="0">
        TypeScript • Next.js • Tailwind
        <animate attributeName="opacity" begin="3.6s" dur="4.5s" values="0;1;0" repeatCount="indefinite"/>
      </text>
      <text x="0" y="0" opacity="0">
        Design Systems • Accessibility • Testing
        <animate attributeName="opacity" begin="5.1s" dur="4.5s" values="0;1;0" repeatCount="indefinite"/>
      </text>
    </g>
  </g>

  <!-- Subtle underline animation -->
  <line x1="220" x2="600" y1="160" y2="160" stroke="#334155" stroke-width="1" opacity="0.6">
    <animate attributeName="x2" from="220" to="600" begin="1s" dur="0.8s" fill="freeze"/>
  </line>

  <!-- small call-to-action or social icons placeholders -->
  <g transform="translate(220,200)" fill="#94A3B8" font-size="14">
    <text x="0" y="0">GitHub:</text>
    <text x="62" y="0" fill="#fff" font-weight="600">@sri986501</text>
  </g>

  <!-- Accessibility: title & desc -->
  <title>Profile intro for sri986501</title>
  <desc>Animated profile banner: avatar badge, name, role, and cycling skills.</desc>
</svg><!--
**sri986501/sri986501** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
