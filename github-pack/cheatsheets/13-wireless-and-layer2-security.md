# Wireless and Layer 2 Security

Purpose: understand common local-network risks and the controls that reduce them.

Concepts
- Wireless networks rely on secure authentication, encryption, and access-point configuration.
- Weak shared passphrases and outdated protocols increase exposure.
- Layer 2 attacks may abuse trust in address resolution, switching, or local broadcast behavior.
- Network segmentation limits the impact of compromised devices.

Useful defensive checks
- `netsh wlan show interfaces` — inspect the wireless interface on a Windows device.
- `ip neigh` or `arp -a` — review the local neighbor cache for troubleshooting; entries are transient and not proof of compromise.
- Review switch security settings, DHCP snooping, dynamic ARP inspection, and port-security capabilities where supported.

Defensive notes
Use current supported wireless security modes, unique credentials, guest isolation, firmware updates, network access control, and monitoring for unexpected address changes. Protect management interfaces and disable unused switch ports.

Only inspect networks you own or are authorized to administer. Standard reference knowledge added because the supplied Layer 2 lab files were held for private infrastructure indicators.
