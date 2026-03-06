# Desk and switching (Mac + PC)

Standalone guide to sharing one desk between a Mac and a gaming PC: KVM vs software (Barrier/Synergy), input-only switching, and cable management.

**Related:** [Monitors](monitors.md) (inputs, resolution/Hz) · [Peripherals](peripherals.md) (keyboard, mouse) · [Checklist](checklist.md)

---

## Options at a glance

| Approach | Display | Keyboard/mouse | Pros | Cons |
|----------|---------|----------------|------|------|
| **KVM switch** | Switches | Shared via KVM USB | One keypress; single set of peripherals | Cost; need KVM that supports your resolution/Hz |
| **Software (Barrier/Synergy)** | Manual input switch on monitor | Shared over network | No extra hardware; free (Barrier) | Display not switched; both machines on; network dependency |
| **Monitor input only** | You switch input (HDMI/DP) | Separate or unplug/swap | Simple; no KVM cost | Two keyboard/mouse or cable swapping |
| **Dedicated peripherals** | One set per machine | Each machine has its own | No switching logic | More gear and cables |

---

## KVM switches

A **KVM** switches **video + USB** (keyboard, mouse, sometimes webcam) between two (or more) computers. One button or hotkey switches everything.

### What to look for

- **Resolution and refresh:** Must support your monitor’s mode (e.g. 1440p @ 144 Hz, 4K @ 60 Hz). Check product specs for max resolution/Hz per port.
- **Ports:** HDMI 2.0/2.1 and/or DisplayPort; USB 3.0+ for peripherals.
- **Dual-monitor:** If you have two displays, you need a **dual-monitor KVM** (two inputs per computer, two outputs to monitors).
- **EDID emulation:** Helps monitors keep the same resolution when switching (avoids re-handshake).
- **Mac compatibility:** Not all KVMs play well with Mac (especially M-series). Prefer models that list Mac/Apple.

### Example product space (verify specs before buying)

- **Avico dual-monitor KVM** — HDMI 2.0, USB 3.0; 4K@60 Hz, 1440p@144 Hz, 1080p@240 Hz; EDID; Mac (M1/M2/M3) listed. (e.g. [Newegg](https://www.newegg.com/p/1DJ-01CJ-00001), [Avico](https://avicotech.com/products/avico-2x2-hdmi-2-0-kvm-dual-monitor-switch).)
- **AV Access 2×1 4K dual HDMI KVM** — USB 3.0 hub, hotkey switching; 1080p@240 Hz, 1440p@144 Hz. (e.g. [AV Access](https://www.avaccess.com/products/4ksw21-dm-c/).)
- **Cable Matters 14-in-1 USB-C KVM dock** — Dual 4K@60 Hz, USB-C, up to 100 W charging; good if both machines use USB-C/Thunderbolt.

Always confirm **exact** resolution and refresh rate for your setup (e.g. 1440p 165 Hz) on the manufacturer’s spec page.

---

## Software: Barrier and Synergy

**Barrier** and **Synergy** let you use **one keyboard and one mouse** across multiple computers. The mouse “moves” to the other machine when you drag to the edge of the screen. **Displays are not switched** — each computer still drives its own monitor(s); you switch the **monitor input** (HDMI/DP) yourself when you change machines.

### Barrier (free, open source)

- Fork of older Synergy; cross-platform (Windows, Mac, Linux).
- **Use case:** One keyboard/mouse for Mac + PC; you manually change monitor input when switching.
- **Setup:** Install on both machines, same LAN; configure which machine is “server” (has the physical keyboard/mouse) and which is “client.”
- **Links:**
  - [Barrier on GitHub](https://github.com/debauchee/barrier)
  - [Barrier — Flathub](https://flathub.org/en/apps/com.github.debauchee.barrier) (Linux)
  - [Control Mac & Windows with one keyboard/mouse (Barrier)](https://kevinsguides.com/guides/utilities/barrier-mac-windows/) — setup walkthrough

### Synergy (paid)

- [Synergy](https://synergy-foss.org/) — commercial; similar idea; paid license (~$29–39). Barrier is the common free alternative.

### Limitations

- **Display:** Does not switch video; only keyboard/mouse. You still need to change the monitor input (or use a KVM for video).
- **Network:** Both PCs on same LAN; can be flaky over VPN or unstable Wi-Fi.
- **Gaming:** Slight latency possible; usually fine for productivity; some prefer a hardware KVM for gaming.

---

## Monitor input only (no KVM)

- **Setup:** Mac and PC both connected to the same monitor(s). Use the monitor’s **input select** (HDMI 1/2, DP 1/2) to choose which computer is shown.
- **Keyboard/mouse:** Either:
  - **Two sets** — one for Mac, one for PC (no switching), or  
  - **One set** — unplug USB and move to the other machine (or use a small USB switch for one keyboard/mouse).
- **Pros:** Simple, no KVM cost, works with any resolution/Hz the monitor supports.
- **Cons:** Manual steps; two keyboards/mice or cable swapping if you want one set.

---

## Cable management

- **Length:** Run cables along the desk (under or behind) so both Mac and PC can reach the KVM or monitor without tension.
- **Labels:** Label HDMI/DP cables (e.g. “Mac,” “PC”) so you know which is which at the monitor or KVM.
- **One cable per machine to KVM:** If using a KVM, one video cable + one USB cable per computer to the KVM; then one set of cables from KVM to monitor(s) and peripherals.
- **Desk layout:** Place the KVM or a USB switch where you can reach the button or hotkey without moving the whole setup.

---

## References

- **KVM examples (check current models and specs):** [Avico dual-monitor KVM](https://avicotech.com/products/avico-2x2-hdmi-2-0-kvm-dual-monitor-switch), [AV Access 2×1 4K dual HDMI KVM](https://www.avaccess.com/products/4ksw21-dm-c/), [Cable Matters USB-C KVM dock](https://www.cablematters.com/pc-1538-178-14-in-1-dual-4k-60hz-usb-c-kvm-switch-dock-for-2-computers-up-to-100w-charging-displayport-hdmi.aspx).
- **Barrier:** [GitHub](https://github.com/debauchee/barrier), [Kevin’s Guides — Barrier Mac + Windows](https://kevinsguides.com/guides/utilities/barrier-mac-windows/).
- **Synergy:** [synergy-foss.org](https://synergy-foss.org/).

Use the [Checklist](checklist.md) to lock in your switching approach and cable plan.
