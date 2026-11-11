# Home Automation CONOPS

## 1. Purpose

This is the overarching concept of operations for an open source home automation system, covering the full stack from hardware to the application layer.

## 2. Mission

Give users control of their data and homes — without the security-ownership and privacy risks of big tech. Maximum control for power users when wanted; easy defaults for everyone else.

## 3. Concept

"House as a supercharged LAN": easy, secure onboarding for new devices, everything internal, external access only through a VPN.

## 4. System of Systems

### Core Infrastructure
- All Linux/BSD machines: router, NAS, streaming device.
- No locked-down appliances — power users can root in.

### Security
- Forefront requirement.
- Strict external access control: VPN only, no inbound exposure.

### Network
- Routers, switches, firewalls, VLANs/segmentation, VPN (client + server).

### Storage
- NAS, local-first data, backups.

### Media
- Streaming devices, media servers.

### Manager Node
- A real computer (not a peripheral): home lab / self-hosting hub.
- Runs VMs/containers for services: email server, password manager, notes/files, media server, backups, git.
- Main/backup terminal and controller for the automation stack.
- Candidates: Proxmox or libvirt/KVM on a mini-PC or DIY x86 box; optional second node for HA/backup.

### Peripherals
- Cameras, garage/door openers, lights, sensors, locks.

### First-Party IoT Devices
- **Architecture:** SoM (MCU + support systems) + interchangeable carrier boards.
- **Dumb peripherals:** no complex OS on the SoM; configuration derived from carrier board type (SoM reads carrier ID via ID resistor or I2C EEPROM).
- **Identity:** devices self-identify on the network with a common protocol/IP scheme; flash storage holds user-assigned friendly names ("garage door", "downstairs light").
- **Rationale:** simpler PCB design; one certified brain reused across device types.

### Control Layer
- Mobile/web apps, voice (optional), dashboards.

### Automation Layer
- Rules/scenes/schedules, local-first execution, no cloud dependency.

## 5. User Experience Tiers

- **Simple mode:** sane defaults, guided setup.
- **Expert mode:** raw config, API, scripting, root access.

## 6. Notes

- Scope analysis of existing home automation systems done 2026-11-02 as first step.
