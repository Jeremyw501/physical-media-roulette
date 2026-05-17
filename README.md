# 📽️ Media Roulette Project

A museum-quality physical media library featuring automated, genre-reactive lighting and a voice-activated "Roulette Picker" search engine.

## 🌟 Project Vision
- **Furniture:** Modified IKEA Billy Bookcases with custom valances and back-bumpers.
- **Lighting:** SK6812 12V RGBW LED strips (60 LEDs/m) for dedicated warm/cool white spine highlighting.
- **Brain:** Home Assistant (HA) running on a local NUC in Arlington, TX.
- **Control:** WLED via the Gladopto 4D Elite controller.

## 🛠️ Technical Stack
- **Remote Access:** Cloudflare Tunnel (`ha.mediaroulette.com`) & Tailscale.
- **Automation:** Jinja2-powered "Braking Logic" for realistic roulette deceleration.
- **Metadata:** iCollect database mapping physical spine locations to LED indices.

## 📏 Shelf Layout (Blu-ray Unit)
- **Tiers:** 9 rows total (including height extension).
- **Spacing:** 7-hole pin spacing for optimal case clearance.
- **Capacity:** ~540 standard cases.

---
*Follow the build on [mediaroulette.com](http://www.mediaroulette.com)*
