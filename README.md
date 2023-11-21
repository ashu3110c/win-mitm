# Win-MITM

`Win-MITM` project has been developed to make Network Intrusion and Penetration Testing easy in Windows environment

## Installation

Pre-Requisites

```bash
Download and install 'nmap' from https://nmap.org/dist/nmap-7.94-setup.exe
Download and install 'npcap' from https://npcap.com/dist/npcap-1.78.exe
```

## Modules

```shell
# ARP Poisoning [To get placed as MITM]
arp-poison #target=192.168.0.101

# Network Packet Sniffing [When placed as MITM]
sniffer #target=192.168.0.101

# Device Discovery [To discover devices on Network]
discover #iprange=192.168.0.1/24

# Get MAC [A helper tool to get MAC for any IP in network]
get-mac #ip=192.168.0.3

# Upcoming
* DNS Spoofer [To serve fake website to the target]
* Protocol Downgrader [HTTPS to HTTP - To sniff packets on https sites]
```

## A simple guideline for MITM attack
```bash
# Note: You can use 'help' command to see detailed doc of each module 
General Steps
1. Discover devices on network using 'discover' module
2. Identify your target IP
3. Start ARP poisoning using 'arp-poison' module
4. Start network packet capturing using 'sniffer' module
```

## Who do I talk to

#### Priyanshu [ashu3110c@gmail.com]

## Future Plans
`Source code will be made public`

## License

[MIT](https://choosealicense.com/licenses/mit/)