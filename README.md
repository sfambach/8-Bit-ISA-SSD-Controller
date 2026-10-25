# 8-Bit-ISA-SSD-Controller

**8-Bit ISA SSD-Controller**

8-bit ISA card for XT and AT class PCs with **SATA ports for SSDs**. Technically it is an **XT-IDE compatible IDE controller**, so the XT-IDE Universal BIOS boots from it. Up to four SSDs in two channels.

**Status: concept.** Nothing has been built or tested yet.

## Features (planned)

- XT-IDE compatible logic (GAL + latches), two channels (master + slave each)
- Up to four SATA ports via plug-on IDE-to-SATA converter boards (JM20330 class)
- Option ROM socket (28C256) for XT-IDE Universal BIOS
- Addresses by DIP switch, through-hole parts
- Later: plug-on module for [isa8_multi_io](https://github.com/sfambach/isa8_multi_io), own DOS CD-ROM driver

Details: [docs/concept.md](docs/concept.md)

## History

- 2026-10-25: Idea from the [isa8_multi_io](https://github.com/sfambach/isa8_multi_io) work. First concept emulated drives from microSD with a Raspberry Pi Pico 2; dropped because "SSD" meant SATA SSDs. Now XT-IDE logic with plug-on IDE-to-SATA converters, two channels, up to four SSDs. The 16-bit sibling [16-Bit-ISA-SSD-Controller](https://github.com/sfambach/16-Bit-ISA-SSD-Controller) was split off the same day.

## License

- Hardware: [CERN-OHL-S-2.0](LICENSE)
- Documentation: CC BY-SA 4.0
- XT-IDE Universal BIOS (GPL-2) – not included

## Authors

- **Stefan Fambach** (SteFam) – idea and concept, review and testing – https://www.fambach.net
- **Claude** (Anthropic AI) – implementation, via Claude Code

## AI disclosure

This project is built with AI assistance. Stefan Fambach had the idea, wrote the concept and reviews and tests every change; the implementation (schematics, PCB and logic design files, firmware and documentation) is written largely by Claude (Anthropic) via Claude Code.
