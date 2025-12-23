# Notes on Meetings:

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
John Hauser via humboldt.edu 
	
Fri, Dec 19, 8:16 AM (4 days ago)
	
	
to humlug
In deference to most members sensibilities, the photos of my "machine stacks & racks" cabling have not been included!
 
What’s the purpose of a 10” server rack?
Portability
Organization 
Clean look
Good for multiples of 1U items

Pros
Enforces discipline & planning
Concentrates compute
Tiny/Mini/Micro 1L PCs

Cons
Stuff that doesn’t fit - Various MiniPCs - Cheaper Chinese > 1U High
Also High Intel NUCs, external hard drives
No solution to power or power brick issues
 When 10” isn’t? Inside rails = 8.75”
Ventilation 

Mini ITX Examples
NAS board
Where’s the power supply?
Where’s SATA storage gonna go?

Minisforum BD795i SE example
16 cores, 32 threads, 128GB RAM
Where’s the GPU gonna go?
Where’s the power supply going to go?

Current Favorite Value MiniPC - Peladn WO4
But it doesn’t fit in 1U!
Heard about it from this YT video:
https://youtu.be/tp_iQpjSctM?si=Z9NkQtaPiEiAFa6z

Make sure you get the right configuration, they sell multiple ones:
https://peladn.us/products/peladn-ha-4-mini-pc-amd-ryzen-5-7640hs?variant=50551604576573
AMD Ryzen5 7640HS
6 core, 12 thread CPU, 32GB DDR5 RAM, 1TB NVME
2 NICs - 1x2.5Gb, 1x1Gb
2 NVME slots
$384 w 10% discount code Geek1201
ships from US warehouse

Worth it for the RAM alone
Good for Proxmox node w Ceph storage due to 2nd NIC and 2nd NVME

VirtualizationHowto YT channel and blog
https://www.youtube.com/@VirtualizationHowto/videos
https://www.virtualizationhowto.com
