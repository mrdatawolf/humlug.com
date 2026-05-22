# Meeting Notes

## May 2026

### Songs
- Yesterday
- She's So Heavy
- Helter Skelter
- Lady Madonna
- Here There and Everywhere
- Brain

### Topics & Links
- [copyparty](https://urldefense.com/v3/__https://github.com/9001/copyparty__;!!OzdlGbv3!6IRdEYdfHkzn0w4d-9emZwzMiWayIIczkcD7IZMiADJTuqFh5fjkeIivH_lfX5SXl2HbtqVXgeA-p11nKHc$)
- [project-brain](https://github.com/mrdatawolf/project-brain)
- [Spreadsheet](https://docs.google.com/spreadsheets/d/1lKvDxJ6aZJOhhJysCRVTpIJsobJRy3PZCO52i7S8I50/edit?gid=1952542002#gid=1952542002)
- [DM Helper](https://github.com/mrdatawolf/DM_Helper)

---

## April 2026

**Project NOMAD** — Knowledge that never goes offline

Release 1.32.0 is here: [announcement](https://urldefense.com/v3/__https://crosstalksolutions.us20.list-manage.com/track/click?u=48c0b53253f77061ffe21068b&id=5eecfc1b04&e=c498deec1e__;!!OzdlGbv3!6uUQ5UtJj4JvqyVNK0fd4a_SbbapUlvFzb1xKasH0agj4bdgT12liEPe2Ny2nYSjJo5_lH0etS3Fo-61t2M$)

---

## December 2025

### Notes on 10" Server Racks, MiniPCs, and Related Hardware

_In deference to most members' sensibilities, the photos of my "machine stacks & racks" cabling have not been included._

#### What's the Purpose of a 10" Server Rack?
- Portability
- Organization
- Clean look
- Good for multiples of 1U items

#### Pros
- Enforces discipline & planning
- Concentrates compute
- Works well with Tiny/Mini/Micro 1L PCs

#### Cons
- Stuff that doesn't fit:
  - Various MiniPCs
  - Cheaper Chinese units > 1U height
  - Taller Intel NUCs
  - External hard drives
- No solution to power or power‑brick issues
- When 10" isn't really 10": inside rails = **8.75"**
- Ventilation challenges

#### Mini‑ITX Examples
- NAS boards
- Questions to solve:
  - Where's the power supply going?
  - Where's SATA storage going to go?

#### Minisforum BD795i SE
- 16 cores, 32 threads, 128GB RAM
- Questions to solve:
  - Where's the GPU going to go?
  - Where's the power supply going to go?

#### Current Favorite Value MiniPC — Peladn WO4

**But it doesn't fit in 1U!**

Heard about it from this [YouTube video](https://youtu.be/tp_iQpjSctM?si=Z9NkQtaPiEiAFa6z).

Multiple variants available — make sure you get the right configuration:
[Peladn WO4 on peladn.us](https://peladn.us/products/peladn-ha-4-mini-pc-amd-ryzen-5-7640hs?variant=50551604576573)

**Specs:**
- AMD Ryzen 5 7640HS
- 6‑core / 12‑thread CPU
- 32GB DDR5 RAM
- 1TB NVMe
- 2 NICs: 1 × 2.5Gb, 1 × 1Gb
- 2 NVMe slots
- ~$384 with 10% discount code `Geek1201`
- Ships from US warehouse

**Why it's compelling:**
- Worth it for the RAM alone
- Great for a Proxmox node with Ceph storage due to 2nd NIC and 2nd NVMe slot

#### VirtualizationHowto
- [YouTube channel](https://www.youtube.com/@VirtualizationHowto/videos)
- [Blog](https://www.virtualizationhowto.com)

---

## May 2025

### Internet in a Box (IIAB)

- [CD3WD on Wikipedia](https://en.wikipedia.org/wiki/CD3WD)
- [CD3WD Project](https://www.cd3wdproject.org/)

It's been 2 years since my HumLUG presentation on "Internet in a Box". Here's a link to the slides.

I've found that IIAB works better from an x86 machine rather than a Raspberry Pi, especially if you're going to load up Open Street Maps and expect to be zooming around between the 10 levels of detail.

Today I got x86 IIAB resurrected in its April 2023 configuration and am now updating what content I can.

Questions about IIAB are welcome!

[Video of the presentation](https://drive.google.com/file/d/19XeHLMtnmnT88G4iZ0vgbz75rODm58Nk/view)

---

## March 2025

### MQTT

```sh
winget install mosquitto
winget install --id=thomasnordquist.MQTT-Explorer -e
```

- [mqtt_serve_tester](https://github.com/mrdatawolf/mqtt_serve_tester)
- [ps-mqtt-sqlite](https://github.com/mrdatawolf/ps-mqtt-sqlite)
- DB Browser for SQLite
