# Exploring Your First Network

Networking is usually invisible — until you look. This project is a hands-on tour of the Linux networking stack: interfaces, addresses, routes, name resolution, neighbors and sockets, observed through the system's own utilities.

## Task 0 — List Network Interfaces

`list_interfaces.sh` prints a concise, brief table of every network interface in the current environment: interface name, operational state, and assigned IPv4/IPv6 addresses. It uses the native output of `ip -brief address` — no reformatting, no hardcoded values.

### Usage

```bash
./list_interfaces.sh
```

### Example output

```text
lo               UNKNOWN        127.0.0.1/8 ::1/128
eth0@if5         UP             169.254.172.2/22 fe60::f003:dcaf:fe31:3e72/64
eth1             UP             10.42.125.74/16 fe80::46b:71ff:fafd:a2a5/64
```

*Values vary per environment — the script always reads the live state.*
