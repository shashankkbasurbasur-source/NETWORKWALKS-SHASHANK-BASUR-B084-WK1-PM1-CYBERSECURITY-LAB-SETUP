# Cybersecurity Lab Setup — Week 1

This project is part of my Networkwalks cybersecurity internship. The goal was to set up a Kali Linux lab using VirtualBox for cybersecurity practice.

## Lab Setup

- **Host OS:** Ubuntu
- **Virtualization:** Oracle VirtualBox 7.2
- **Virtual Machine:** Kali Linux 2026.3
- **Network:** NAT Network (`10.0.0.0/24`)
- **Kali IP:** `10.0.0.2/24`
- **Gateway:** `10.0.0.1`
- **DNS:** `8.8.8.8`

## Tasks Completed

- Configured the VirtualBox NAT Network.
- Set up Kali Linux with the required IP address.
- Verified internet and DNS connectivity.
- Enabled bidirectional clipboard and drag-and-drop.
- Shared the Ubuntu Downloads folder with Kali at `/mnt/downloads`.
- Created a VM snapshot named `Week1-Lab-Setup-Complete`.

## Connectivity Test

Commands used to verify connectivity:

ping -c 4 10.0.0.1
ping -c 4 google.com

Both tests completed successfully with no packet loss.

## Troubleshooting

During setup, Kali encountered IP address configuration conflicts. I applied the `ipv4.dad-timeout 0` setting recommended in the internship guide, configured the required IP address, and verified that the gateway and internet connection were working.

## Screenshots

Screenshots of the network configuration, connectivity tests, shared folder, VM settings, and snapshot are available in the `screenshots/` directory.

## Learning Outcomes

- VirtualBox networking and IPv4 configuration
- Basic network troubleshooting
- DNS and connectivity testing
- Shared folders and VM snapshots


