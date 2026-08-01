<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 868 880" font-family="'Segoe UI', Helvetica, Arial, sans-serif">
  <defs>
    <pattern id="hatch" width="8" height="8" patternUnits="userSpaceOnUse" patternTransform="rotate(45)">
      <rect width="8" height="8" fill="#ECEEF1"/>
      <line x1="0" y1="0" x2="0" y2="8" stroke="#B6BCC4" stroke-width="1.3"/>
    </pattern>
    <marker id="ar" markerWidth="11" markerHeight="11" refX="7" refY="3" orient="auto-start-reverse">
      <path d="M0,0 L7,3 L0,6 Z" fill="#2A6470"/>
    </marker>
    <marker id="arrow" markerWidth="10" markerHeight="10" refX="7" refY="3" orient="auto">
      <path d="M0,0 L7,3 L0,6 Z" fill="#1F2933"/>
    </marker>
  </defs>

  <rect x="0" y="0" width="760" height="880" fill="#FBFAF7"/>
  <text x="40" y="44" font-size="23" font-weight="700" fill="#1F2933">Joystick Variant — Unit on a ball-and-socket pivot</text>
  <text x="40" y="70" font-size="14" fill="#5A6470">Tilt the mouthpiece to move the cursor; sip / puff through the same mouthpiece for clicks. One sealed Unit, two input modes.</text>

  <!-- tilt arc -->
  <path d="M268,150 Q380,108 492,150" fill="none" stroke="#2A6470" stroke-width="2" marker-start="url(#ar)" marker-end="url(#ar)"/>
  <text x="380" y="100" font-size="13" fill="#2A6470" text-anchor="middle" font-weight="600">tilt = cursor (2-axis: ±X, ±Y)</text>

  <!-- ghost tilted position -->
  <g opacity="0.35">
    <line x1="380" y1="540" x2="470" y2="300" stroke="#9AA0A6" stroke-width="2" stroke-dasharray="5 4"/>
    <rect x="430" y="170" width="120" height="92" rx="14" transform="rotate(20 490 216)" fill="none" stroke="#9AA0A6" stroke-width="1.6" stroke-dasharray="5 4"/>
  </g>

  <!-- ===== mouthpiece Unit ===== -->
  <rect x="315" y="135" width="130" height="115" rx="16" fill="#FFFFFF" stroke="#6B7280" stroke-width="1.5"/>
  <path d="M338,178 C360,170 392,172 408,192" fill="none" stroke="#0E7C86" stroke-width="3"/>
  <text x="380" y="206" font-size="12.5" fill="#1F2933" text-anchor="middle" font-weight="600">Mouthpiece Unit</text>
  <text x="380" y="222" font-size="11" fill="#5A6470" text-anchor="middle">(sealed; sip/puff = clicks)</text>
  <!-- spigot -->
  <rect x="362" y="250" width="36" height="22" fill="url(#hatch)" stroke="#6B7280" stroke-width="1"/>

  <!-- ===== stem ===== -->
  <rect x="360" y="272" width="8" height="200" fill="url(#hatch)" stroke="#6B7280" stroke-width="1"/>
  <rect x="392" y="272" width="8" height="200" fill="url(#hatch)" stroke="#6B7280" stroke-width="1"/>

  <!-- ===== ball ===== -->
  <circle cx="380" cy="540" r="72" fill="url(#hatch)" stroke="#6B7280" stroke-width="1.6"/>
  <text x="380" y="528" font-size="12" fill="#5A6470" text-anchor="middle">ball</text>
  <line x1="380" y1="468" x2="380" y2="612" stroke="#C9CDD3" stroke-width="1" stroke-dasharray="3 3"/>

  <!-- ===== socket / housing ===== -->
  <path d="M130,700 L130,624 Q130,612 150,610 L300,610 Q318,560 335,548 A72,72 0 0 0 425,548 Q442,560 460,610 L610,610 Q630,612 630,624 L630,700 Z" fill="url(#hatch)" stroke="#6B7280" stroke-width="1.6"/>
  <text x="200" y="592" font-size="12" fill="#1F2933" font-weight="600">socket (housing) — ball pivots here</text>

  <!-- centering boot -->
  <polyline points="332,548 344,528 334,512 350,494 342,476 362,462" fill="none" stroke="#7E8794" stroke-width="2"/>
  <polyline points="428,548 416,528 426,512 410,494 418,476 398,462" fill="none" stroke="#7E8794" stroke-width="2"/>
  <text x="150" y="500" font-size="11.5" fill="#1F2933">centering boot</text>
  <text x="150" y="515" font-size="11" fill="#5A6470">(recenters + spit/dust seal)</text>
  <line x1="232" y1="503" x2="330" y2="510" stroke="#5A6470" stroke-width="1"/>

  <!-- magnet at ball bottom pole -->
  <rect x="364" y="586" width="32" height="13" fill="#C0392B"/>
  <rect x="364" y="599" width="32" height="13" fill="#2D6A8A"/>
  <text x="380" y="596" font-size="9" fill="#FFFFFF" text-anchor="middle" font-weight="700">N</text>
  <text x="380" y="610" font-size="9" fill="#FFFFFF" text-anchor="middle" font-weight="700">S</text>

  <!-- ===== PCB ===== -->
  <rect x="150" y="700" width="460" height="22" fill="#21402C" rx="2"/>
  <text x="595" y="715" font-size="10.5" fill="#CFE3D5" text-anchor="end">PCB · RP2350 — reads both over I²C (Seesaw)</text>
  <!-- Hall sensor -->
  <rect x="362" y="686" width="36" height="14" fill="#2A3340" rx="2"/>
  <!-- pressure sensor -->
  <rect x="228" y="686" width="44" height="14" fill="#2A3340" rx="2"/>

  <!-- sense gap -->
  <line x1="420" y1="612" x2="420" y2="686" stroke="#9AA0A6" stroke-width="1" stroke-dasharray="3 3"/>
  <text x="428" y="652" font-size="10.5" fill="#5A6470">sense gap</text>

  <!-- ===== flexible air tube ===== -->
  <path d="M380,250 L372,300 L372,470 C370,505 358,548 344,580 C328,614 288,668 250,693" fill="none" stroke="#4C97A8" stroke-width="11" stroke-linecap="round"/>
  <path d="M380,250 L372,300 L372,470 C370,505 358,548 344,580 C328,614 288,668 250,693" fill="none" stroke="#D8EAEF" stroke-width="6" stroke-linecap="round"/>

  <!-- ===== labels ===== -->
  <line x1="560" y1="252" x2="445" y2="200" stroke="#5A6470" stroke-width="1"/>
  <text x="566" y="250" font-size="12" fill="#1F2933">same disposable Unit —</text>
  <text x="566" y="266" font-size="12" fill="#1F2933">push-fits onto stem + tube</text>

  <line x1="470" y1="360" x2="397" y2="370" stroke="#5A6470" stroke-width="1"/>
  <text x="478" y="356" font-size="12" fill="#1F2933">stem (rigid) —</text>
  <text x="478" y="372" font-size="12" fill="#1F2933">transmits tilt to ball</text>

  <line x1="150" y1="640" x2="300" y2="630" stroke="#5A6470" stroke-width="1"/>
  <text x="40" y="636" font-size="12" fill="#1F2933" font-weight="600">flexible air tube</text>
  <text x="40" y="652" font-size="11" fill="#5A6470">flexes with tilt;</text>
  <text x="40" y="666" font-size="11" fill="#5A6470">off-axis through ball</text>

  <line x1="408" y1="592" x2="398" y2="592" stroke="#5A6470" stroke-width="1"/>
  <text x="414" y="582" font-size="11.5" fill="#1F2933" font-weight="600">magnet (on pivot axis)</text>

  <line x1="380" y1="740" x2="380" y2="700" stroke="#5A6470" stroke-width="1"/>
  <text x="386" y="752" font-size="11.5" fill="#1F2933">3-axis Hall — contactless tilt → X/Y</text>

  <line x1="250" y1="740" x2="250" y2="700" stroke="#5A6470" stroke-width="1"/>
  <text x="40" y="752" font-size="11.5" fill="#1F2933">pressure sensor — sip/puff → buttons</text>

  <!-- ===== notes ===== -->
  <line x1="40" y1="778" x2="720" y2="778" stroke="#E3DFD6"/>
  <text x="40" y="802" font-size="12" fill="#5A6470">Control map: tilt the mouthpiece = move cursor (2 axes); sip / puff through the same mouthpiece = left / right click</text>
  <text x="40" y="820" font-size="12" fill="#5A6470">(add soft / hard thresholds for more buttons). The Unit push-fits onto the stem and into the air tube, so hygiene swaps never touch the mechanism.</text>
  <text x="40" y="842" font-size="12" fill="#5A6470">Hall sensing (magnet on ball + 3-axis Hall below) is contactless — no wear, sealed, low power — and fits the RP2350 / Seesaw path.</text>
  <text x="40" y="860" font-size="12" fill="#5A6470">Alternatives: gimbal + potentiometers (wear, bulkier) or a COTS analog thumbstick under the stem.</text>
</svg>
