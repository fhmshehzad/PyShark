<h1 align="center">PyShark - A Python Based Packet Sniffer</h1>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.7-yellow?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/build-stable-green?style=for-the-badge&logo=build">
  <img src="https://img.shields.io/badge/version-1.0-red?style=for-the-badge&logo=version">

A Python3 scapy based Packet Sniffer that has the capabilities of sniffing raw HTTP, TCP, UDP, ICMP, ARP packets and writing the output to .pcap for inspection within tools such as Wireshark.

## Features
<ul>
  <li>Python 3 Support</li>
  <li>Raw Packet Capturing</li>
  <li>Pure Python</li>
  <li>Cross-Platform</li>
  <li>Supported Layers: HTTP, TCP, UDP, ICMP</li>
</ul>

## Installation:
Cloning:
```
$ git clone https://github.com/pyshark/pyshark.git
$ cd pyshark/
$ pip3 install -r requirements.txt
```

First Run:
```
$ python3 pyshark.py
```

## Usage
```
usage: pyshark.py [-h] [-c COUNT] [-f FILTER [FILTER ...]] [-H] [-o OUTFILE] [-i INTERFACE]

PyShark - HTTP Packet Sniffer.

optional arguments:
  -h, --help            show this help message and exit
  -c COUNT, --count COUNT
                        Numbers of packets that you need to capture (0 = Infinity)
  -f FILTER [FILTER ...], --filter FILTER [FILTER ...]
                        The Berkeley Packet Filter (BPF) that you need to set. (Default is: 'port 80 and tcp') NOTE: You need to Specify them as a string
  -H, --http-only       Limit the results to display only http/https packets
  -o OUTFILE, --outfile OUTFILE
                        Store all the sniffed packet to a .pcap file (You don't need Specify the extension, just the file name.)
  -i INTERFACE, --interface INTERFACE
                        Specify an interface to sniff traffic on
```
