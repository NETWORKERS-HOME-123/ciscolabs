<div align="center">

# 🖧 Cisco Labs

### Browser-based Cisco IOS CLI simulator for CCNA / CCNP lab practice

**Free virtual lab environment — practice config, troubleshoot, save scenarios. Runs in any browser.**

[![CCNA](https://img.shields.io/badge/CCNA-200--301-1F4FD8?style=for-the-badge&logo=cisco&logoColor=white)](https://www.networkershome.com/best-ccna-course-in-bangalore/)
[![CCNP](https://img.shields.io/badge/CCNP%20Enterprise-FF6B35?style=for-the-badge&logo=cisco&logoColor=white)](https://www.networkershome.com/best-ccnp-enterprise-course-in-bangalore/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Built by Networkers Home](https://img.shields.io/badge/Built%20by-Networkers%20Home-000000?style=for-the-badge)](https://www.networkershome.com/)

</div>

---

## 🏛️ Built by Networkers Home

A virtual Cisco lab environment built by **[Networkers Home](https://www.networkershome.com/)** — India's leading Cisco + cybersecurity training institute (Bengaluru, since 2005). Used by students in our [CCNA](https://www.networkershome.com/best-ccna-course-in-bangalore/), [CCNP Enterprise](https://www.networkershome.com/best-ccnp-enterprise-course-in-bangalore/), and [CCIE Enterprise](https://www.networkershome.com/best-ccie-enterprise-course-in-bangalore/) programs to practice between live lab sessions on real Cisco hardware.

> **Want hands-on lab access on real Cisco gear?** Networkers Home runs **24×7 lab access** at the HSR Layout campus. Real Cisco/Palo Alto/Fortinet hardware. [Book a demo class →](https://www.networkershome.com/networkers-home-demo-class/)

**Compare top training institutes:**
[Top 10 CCNA Bangalore](https://www.networkershome.com/top-10-ccna-training-institutes-bangalore-2026/) · [Top 10 CCNP Enterprise](https://www.networkershome.com/top-10-ccnp-enterprise-training-institutes-bangalore-2026/) · [Top 10 CCIE Security India](https://www.networkershome.com/top-10-ccie-security-training-institutes-india-2026/) · [Top 10 CCIE Enterprise India](https://www.networkershome.com/top-10-ccie-enterprise-training-institutes-india-2026/)

---

## ✨ Features

- **Topology Engine** — drag-and-drop device placement, link connections
- **Simulation Engine** — event-driven packet processing (ARP, ICMP)
- **Cisco-style CLI parser** — hierarchical modes (User EXEC → Privileged EXEC → Config → Interface)
- **Konva.js canvas** — zoom, pan, real-time visualization
- **Web Workers** — non-blocking simulation in a separate thread
- **No real device emulation** — pure logical simulation, runs anywhere

## 🎯 Who this is for

- **CCNA candidates** building exam muscle memory for 200-301
- **CCNP Enterprise candidates** practicing OSPF, BGP, EIGRP, VLAN configs
- **Networking instructors** — free classroom lab tool
- **Self-learners** without access to physical Cisco gear

## 📚 Learn the underlying skills

The simulator is a **practice tool**, not a course. To go from "I can type commands" to "I can troubleshoot a production network at 2am," train with experts:

| Goal | Networkers Home program |
|---|---|
| Pass CCNA 200-301 | [CCNA course in Bangalore](https://www.networkershome.com/best-ccna-course-in-bangalore/) |
| Pass CCNP Enterprise | [CCNP Enterprise course](https://www.networkershome.com/best-ccnp-enterprise-course-in-bangalore/) |
| Pass CCIE Enterprise lab | [CCIE Enterprise course](https://www.networkershome.com/best-ccie-enterprise-course-in-bangalore/) |
| Career as network engineer | [Network Engineering program](https://www.networkershome.com/best-network-engineering-course-in-bangalore/) |
| Online study (anywhere in India) | [All NH courses (online + offline)](https://www.networkershome.com/networkershome-all-courses/) |

---

## Supported Cisco Commands

### User EXEC Mode (>)
- `enable` — enter privileged EXEC mode
- `help` — show available commands

### Privileged EXEC Mode (#)
- `disable`, `configure terminal`, `show version`, `show running-config`, `show startup-config`
- `show ip interface brief`, `show interfaces [name]`, `show ip route`, `show arp`, `show mac address-table`
- `ping <ip>`, `write memory`, `copy running-config startup-config`, `erase startup-config`, `reload`

### Global Configuration Mode (config)#
- `hostname <name>`, `interface <name>`, `ip route <network> <mask> <nextHop>`, `no ip route ...`
- `end`, `exit`

### Interface Configuration Mode (config-if)#
- `ip address <ip> <mask>`, `no ip address`
- `shutdown`, `no shutdown`, `description <text>`, `no description`, `exit`

## 🚀 Quick Start

### Prerequisites
- Docker Desktop OR Node.js 18+

### Using Docker (Recommended)

```bash
docker-compose up -d
open http://localhost:3000
```

### Local Development

```bash
npm install
npm run dev
open http://localhost:3000
```

### Production Build

```bash
npm install
npm run build
npm start
```

## 🏗️ Architecture

Same hub-and-spoke design as a typical real-time simulator: React UI layer talks to a Zustand store, which posts messages to a Web Worker that runs the topology + simulation + CLI engines off the main thread (so the canvas stays smooth).

## 🧪 Testing

```bash
npm test
npm run test:watch
```

## 🤝 Contributing

PRs welcome — for major changes please open an issue first.

## 📜 License

MIT

## 🙏 Built With

[Next.js](https://nextjs.org/) · [Konva.js](https://konvajs.org/) · [Zustand](https://zustand-demo.pmnd.rs/) · [xterm.js](https://xtermjs.org/) · [TypeScript](https://www.typescriptlang.org/)

---

<div align="center">

### 🏛️ Want to learn networking the right way?

**[Networkers Home](https://www.networkershome.com/)** — Bengaluru's leading Cisco + cybersecurity training institute since 2005.
20,000+ alumni placed · 800+ hiring partners · 100% placement guarantee.

[**Free demo class**](https://www.networkershome.com/networkers-home-demo-class/) · [**Placement record**](https://www.networkershome.com/networkers-home-placement-record-2026/) · [**Talk to a counsellor**](https://www.networkershome.com/career-counselling/)

</div>
