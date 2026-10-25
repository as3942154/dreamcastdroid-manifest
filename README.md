
# DreamcastDroid ICS

An experimental Android 4.0 porting project targeting the Sega Dreamcast
(SH-4 architecture).

## Project status

**Stage:** Repository planning

This project is not yet a bootable Android system.

## Target platform

- Hardware: Sega Dreamcast
- CPU: Hitachi SH-4
- Android base: Ice Cream Sandwich (4.0)
- Build host: Ubuntu in VMware
- Initial testing: Dreamcast emulator

## Planned components

- [ ] Historical Android ICS source reference
- [ ] SH-4 cross-compilation toolchain
- [ ] Dreamcast-compatible Linux kernel
- [ ] Android device configuration
- [ ] SH-4-compatible native libraries and utilities
- [ ] BusyBox userspace
- [ ] Recovery environment
- [ ] Ethernet networking
- [ ] AICA audio integration
- [ ] Controller-based navigation
- [ ] Persistent storage and vold integration

## Development principles

1. Record upstream URLs and revisions before adding projects.
2. Keep experimental changes separate from upstream source.
3. Verify architecture compatibility for every native binary.
4. Test the kernel and minimal userspace before Android services.
5. Document memory constraints and emulator limitations.

## Important limitation

The Dreamcast has 16 MB of main RAM. A successful Linux boot does not
guarantee that the Android framework can run within the available memory.
