# Notes on Meetings:

# May 2026 - 

https://urldefense.com/v3/__https://github.com/9001/copyparty__;!!OzdlGbv3!6IRdEYdfHkzn0w4d-9emZwzMiWayIIczkcD7IZMiADJTuqFh5fjkeIivH_lfX5SXl2HbtqVXgeA-p11nKHc$

https://github.com/mrdatawolf/project-brain

#April 2026 -
Project NOMAD
Knowledge that never goes offline
Release 1.32.0
v1.32.0 is here.
https://urldefense.com/v3/__https://crosstalksolutions.us20.list-manage.com/track/click?u=48c0b53253f77061ffe21068b&id=5eecfc1b04&e=c498deec1e__;!!OzdlGbv3!6uUQ5UtJj4JvqyVNK0fd4a_SbbapUlvFzb1xKasH0agj4bdgT12liEPe2Ny2nYSjJo5_lH0etS3Fo-61t2M$

# March 2025 -

MQTT notes:
  winget install mosquitto
  [mqtt_serve_tester](https://github.com/mrdatawolf/mqtt_serve_tester)
  [ps-mqtt-sqlite](https://github.com/mrdatawolf/ps-mqtt-sqlite)
  winget install --id=thomasnordquist.MQTT-Explorer -e
  DB Browser for SQLite
  
# May 2025 -

More detail on this project:

https://en.wikipedia.org/wiki/CD3WD

https://www.cd3wdproject.org/

It’s been 2 years since my HumLUG presentation on "Internet in a Box”. Here’s a link to the slides. 

I’ve found that IIAB works better from a x86 machine rather than a Raspberry Pi, especially if you’re going to load up Open Street Maps and expect to be zooming around between the 10 levels of detail.

Today I got x86 IIAB resurrected  in it's April 2023 configuration and am now updating what content I can.

Questions about IIAB are welcome!

Video of the presentation:
https://drive.google.com/file/d/19XeHLMtnmnT88G4iZ0vgbz75rODm58Nk/view

# June 2025

# Dec 2025
# Notes on 10" Server Racks, MiniPCs, and Related Hardware

_In deference to most members’ sensibilities, the photos of my "machine stacks & racks" cabling have not been included._

---

## What’s the Purpose of a 10” Server Rack?

- Portability  
- Organization  
- Clean look  
- Good for multiples of 1U items  

---

## Pros

- Enforces discipline & planning  
- Concentrates compute  
- Works well with Tiny/Mini/Micro 1L PCs  

---

## Cons

- Stuff that doesn’t fit:
  - Various MiniPCs  
  - Cheaper Chinese units > 1U height  
  - Taller Intel NUCs  
  - External hard drives  
- No solution to power or power‑brick issues  
- When 10” isn’t really 10”: inside rails = **8.75”**  
- Ventilation challenges  

---

## Mini‑ITX Examples

- NAS boards  
- Questions to solve:
  - Where’s the power supply going?  
  - Where’s SATA storage going to go?  

---

## Minisforum BD795i SE Example

- 16 cores, 32 threads, 128GB RAM  
- Questions to solve:
  - Where’s the GPU going to go?  
  - Where’s the power supply going to go?  

---

## Current Favorite Value MiniPC — **Peladn WO4**

**But it doesn’t fit in 1U!**

Heard about it from this YT video:  
https://youtu.be/tp_iQpjSctM?si=Z9NkQtaPiEiAFa6z

Make sure you get the right configuration — they sell multiple variants:  
https://peladn.us/products/peladn-ha-4-mini-pc-amd-ryzen-5-7640hs?variant=50551604576573

**Specs:**

- AMD Ryzen 5 7640HS  
- 6‑core / 12‑thread CPU  
- 32GB DDR5 RAM  
- 1TB NVMe  
- 2 NICs:
  - 1 × 2.5Gb  
  - 1 × 1Gb  
- 2 NVMe slots  
- ~$384 with 10% discount code `Geek1201`  
- Ships from US warehouse  

**Why it’s compelling:**

- Worth it for the RAM alone  
- Great for a Proxmox node with Ceph storage due to:
  - 2nd NIC  
  - 2nd NVMe slot  

---

## VirtualizationHowto (YouTube & Blog)

- https://www.youtube.com/@VirtualizationHowto/videos  
- https://www.virtualizationhowto.com  

---

