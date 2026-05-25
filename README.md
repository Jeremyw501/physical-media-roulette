# 📽️ Media Roulette Project

A museum-quality physical media library featuring automated, genre-reactive lighting and a voice-activated "Roulette Picker" search engine.

## 🌟 Project Vision
- **Furniture:** Modified IKEA Billy Bookcases with custom valances and back-bumpers.
- **Lighting:** SK6812 12V RGBW LED strips (60 LEDs/m) for dedicated warm/cool white spine highlighting.
- **Brain:** Home Assistant (HA) running on a local NUC in Arlington, TX.
- **Control:** WLED via the Gladopto 4D Elite controller.

## 🛠️ Technical Stack
- **Remote Access:** Cloudflare Tunnel & Tailscale.
- **Automation:** Jinja2-powered "Braking Logic" for realistic roulette deceleration.
- **Metadata:** iCollect database mapping physical spine locations to LED indices.

## 📏 Shelf Layout (Blu-ray Unit)
- **Tiers:** 9 rows total (including height extension).
- **Spacing:** 7-hole pin spacing for optimal case clearance.
- **Capacity:** ~540 standard cases.

---
## 🛒 Bill of Materials (Shopping List)

This section outlines the components used to build the physical structure and smart-home integration layer.

<details>
<summary>📦 Click to expand full Hardware & Tools breakdown</summary>

### 🖼️ Structural & Aesthetic Foundation
- [ ] **2x IKEA BILLY Bookcases** (Black Oak Effect)
- [ ] **2x IKEA BILLY Height Extension Units** (Black Oak Effect)
- [ ] **1x IKEA KALLAX 4x4 Frame** (Center hub for TV & electronics)
- [ ] **Muzata 45-Degree Aluminum LED Channels** (Model: V-Shape / LN1) - *Angled down/back to eliminate glare hotspots.*
- [ ] **1/2-inch 3M 9448A Double-Sided Tape** (0.15mm ultra-thin industrial acrylic adhesive for a gap-free flush mount)

### ⚡ Electronics & Wiring Stack
- [ ] **SK6812 12V Addressable RGBW LED Strips** (60 LEDs/meter, features a dedicated true-white channel)
- [ ] **Gladopto 4D Elite Controller** (Pre-flashed with WLED firmware)
- [ ] **12V 12.5A (150W) Ultra-Slim Terminal Block Power Supply**
- [ ] **18AWG 3-Conductor Black Silicone Ribbon Wire** (Flexible for layout jumps)
- [ ] **1/2" 3:1 Ratio Dual-Wall Heat Shrink Tubing** (Adhesive-lined)

### 🛠️ Prep & Build Tools
- [ ] **91% Isopropyl Alcohol** (For deep chemical cleaning prior to paint and tape application)
- [ ] **Self-Etching Spray Primer** (Chemically bites into raw aluminum channels to prevent peeling)
- [ ] **Matte or Satin Black Spray Paint** (To match channels perfectly to the IKEA Black Oak finish)
- [ ] **YIHUA 926III-v2 Soldering Station** (Set to 350°C for fast pad wetting)
- [ ] **MG Chemicals No-Clean Flux Pen**
- [ ] **Small Hand File or Dremel Tool** (For side-shelf wire routing notches)

</details>

---

## 🏗️ Step-by-Step Build Plan

The construction is broken into distinct mechanical, aesthetic, and electrical phases to ensure a clean, hidden layout.

### Phase 1: Aluminum Channel Preparation (The Stealth Look)
To prevent regular spray paint from scratching or flaking off the slick raw aluminum, follow this mechanical/chemical bonding progression:
1. **Disassembly:** Remove the frosted plastic diffuser lenses from the aluminum tracks completely. Set them aside.
2. **Mechanical Scuffing:** Lightly sand all visible exterior surfaces of the aluminum using a 320–400 grit scuff pad to create micro-abrasions ("teeth") for the paint to grip.
3. **Chemical Wipe:** Wipe down the tracks thoroughly with **91% Isopropyl Alcohol** to remove all manufacturing oils and aluminum dust.
4. **Etching Primer:** Apply 1-2 thin coats of **Self-Etching Spray Primer**. Let cure for 20 minutes until a dull gray color forms.
5. **Top Coat:** Apply 2 mist coats of **Matte or Satin Black Spray Paint** for a seamless match with the bookcase finish. Allow to cure completely for **24 hours**.

> ⚠️ **Tolerance Pro-Tip:** Do not spray a heavy layer of paint inside the tracking grooves where the diffuser lens clips in. If the paint layer is too thick, the lens will fail to snap in securely.

### Phase 2: Structural Modifications & Mounting
1. **Wire Path Routing:** To snake wires down the inside frame walls without drilling giant pass-through holes through the shelves, use a hand file or Dremel to grind a small U-shaped notch ($1/8\text{ inch}$ deep by $1/2\text{ inch}$ wide) into the side edge of each adjustable shelf.
2. **Channel Mounting:** Clean the underside front edge of the shelves with alcohol. Apply **3M 9448A tape** to the painted aluminum channel. Press firmly onto the shelf with high physical pressure for 15–20 seconds to fully activate the adhesive. 

> 🕒 **Adhesive Cure Window:** 3M 9448A reaches 90% strength at 24 hours and 100% at 72 hours. Avoid hanging heavy wire clusters or snapping in tight diffusers until the adhesive has set.

### Phase 3: Solder and Electrical Matrix
1. **LED Placement:** Cut individual LED strips to fit your channels, making sure the interior strip is cut roughly $0.75\text{ inches}$ shorter than the track to leave an open wire pocket at the edge.
2. **Soldering:** Tin the 3 copper pads (`+12V`, `Data`, `GND`) using a flux pen and your iron at 350°C. Solder your 18AWG silicone ribbon wire to the pads inside the channel housing.
3. **Wire Protection:** Protect the side wall transition bending points by sliding a $1.5\text{-inch}$ section of adhesive-lined black heat shrink over the ribbon cable where it passes through your filed shelf notch. This acts as a protective protective bushing against raw wood edges.
4. **S-Chain Snake:** Loop the ribbon wire through the gap between the shelf edge and outer frame down to the next shelf level, keeping a minor relaxed S-curve loop to avoid tension on the solder joints.
*Follow the build on [mediaroulette.com](http://www.mediaroulette.com)*
