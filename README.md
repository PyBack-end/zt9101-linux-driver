# ZT9101 Linux USB Wi-Fi Driver

An open-source Linux driver project for USB wireless adapters based on the ZT9101 chipset.

The project focuses on bringing ZT9101-based wireless hardware into the Linux networking stack, including USB device management, wireless interface registration, cfg80211 integration, and Wi-Fi Direct (P2P) functionality.

## What it does

- **USB device support:** Detects and initializes compatible ZT9101 USB wireless adapters.
- **Wireless networking:** Integrates the adapter with Linux network interfaces.
- **cfg80211 integration:** Provides wireless configuration and interface management through the Linux wireless subsystem.
- **Wi-Fi Direct / P2P:** Includes infrastructure for P2P Client and P2P Group Owner interface roles.
- **Device lifecycle management:** Handles initialization, resource allocation, shutdown, and USB disconnection.
- **Hardware communication:** Implements the host interface and USB endpoint management required to communicate with the adapter.

## Current development

The project is undergoing a source-level audit and reliability improvement process.

Current areas of investigation include:

- USB probe and disconnect handling.
- Initialization failure recovery and resource cleanup.
- P2P and Wi-Fi Display resource management.
- cfg80211 interface configuration.
- Net-device registration and teardown.
- Kernel compatibility and build reliability.

## Development status

<details>
<summary>Current status</summary>

| Area | Status |
|---|---|
| USB device identification | Confirmed |
| Driver compilation | Previously successful |
| cfg80211 integration | Present in source |
| P2P Client role | Present in source |
| P2P Group Owner role | Present in source |
| Resource lifecycle audit | In progress |
| Initialization rollback | Requires improvement |
| Real hardware connectivity testing | Not yet verified |
| Android Wi-Fi Direct interoperability | Not yet verified |

</details>

**Important:** The presence of P2P functionality in the source does not establish that Wi-Fi Direct connections work on real hardware. Hardware interoperability testing is still required.

## Building

Build instructions and supported kernel versions will be documented as compatibility testing progresses.

Do not assume that successful compilation guarantees safe operation or complete hardware functionality.

## License

See the repository's `LICENSE` file for the applicable license and redistribution terms.

## Disclaimer

This project is under active investigation. Hardware support, kernel compatibility, and wireless functionality may vary. Use caution when testing experimental kernel drivers.
