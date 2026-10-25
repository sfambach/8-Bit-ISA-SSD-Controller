# isa8_sd_ide

8-bit ISA card for XT and AT class PCs that presents **microSD card images as IDE drives** (hard disk and CD-ROM) and shows itself as an **XT-IDE compatible controller**, so the XT-IDE Universal BIOS boots from it. A second, real IDE port takes hard disks, CF/SATA adapters or a CD-ROM drive. Up to four devices in two channels.

**Status: concept.** Nothing has been built or tested yet.

## Features (planned)

- Channel 1: real IDE port (40-pin or 44-pin), XT-IDE compatible logic
- Channel 2: emulated by a Raspberry Pi Pico 2 (RP2350), two microSD slots, image files (`.img`, `.iso`, `.cue/.bin`)
- CD-ROM via own DOS driver (8088 compatible) + MSCDEX
- Option ROM socket (28C256) for XT-IDE Universal BIOS
- Addresses by DIP switch, IRQ by jumper, through-hole parts, glue logic in a GAL
- Later: plug-on module for [isa8_multi_io](https://github.com/sfambach/isa8_multi_io)

Details: [docs/concept.md](docs/concept.md)

## License

- Hardware: [CERN-OHL-S-2.0](LICENSE)
- Own firmware and DOS tools: PolyForm Noncommercial 1.0.0 (planned)
- Documentation: CC BY-SA 4.0
- XT-IDE Universal BIOS (GPL-2) – not included

## AI disclosure

This project is developed with the help of AI (Claude by Anthropic). Design decisions and testing are done by Stefan Fambach.

## Author

Stefan Fambach (SteFam) – https://www.fambach.net
