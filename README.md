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

## License

- Hardware: [CERN-OHL-S-2.0](LICENSE)
- Documentation: CC BY-SA 4.0
- XT-IDE Universal BIOS (GPL-2) – not included

## AI disclosure

This project is developed with the help of AI (Claude by Anthropic). Design decisions and testing are done by Stefan Fambach.

## Author

Stefan Fambach (SteFam) – https://www.fambach.net
