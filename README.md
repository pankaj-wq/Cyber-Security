NetProbe: Network Probe
NetProbe is a tool you can use to scan for devices on your network. The program sends ARP requests to any IP address on your network and lists the IP addresses, MAC addresses, manufacturers, and device models of the responding devices.


Buy Me A Coffee
Features
Scan for devices on a specified IP address or subnet
Display the IP address, MAC address, manufacturer, and device model of discovered devices
Live tracking of devices (optional)
Save scan results to a file (optional)
Filter by manufacturer (e.g., 'Apple') (optional)
Filter by IP range (e.g., '192.168.1.0/24') (optional)
Scan rate in seconds (default: 5) (optional)
Download
You can download the program from the GitHub page.

$ git clone https://github.com/pankaj-wq/Cyber-Security.git
Installation
To install the required libraries, run the following command:

$ pip install -r requirements.txt
Usage
To run the program, use the following command:

$ python3 netprobe.py [-h] -t  [...] -i  [...] [-l] [-o] [-m] [-r] [-s]
-h,--help: show this help message and exit
-t,--target: Target IP address or subnet (default: 192.168.1.0/24)
-i,--interface: Interface to use (default: None)
-l,--live: Enable live tracking of devices
-o,--output: Output file to save the results
-m,--manufacturer: Filter by manufacturer (e.g., 'Apple')
-r,--ip-range: Filter by IP range (e.g., '192.168.1.0/24')
-s,--scan-rate: Scan rate in seconds (default: 5)
Example:
$ python3 netprobe.py -t 192.168.1.0/24 -i eth0 -o results.txt -l
Help Menu
$ python3 netprobe.py --help                      
usage: netprobe.py [-h] -t  [...] -i  [...] [-l] [-o] [-m] [-r] [-s]

NetProbe: Network Scanner Tool

options:
  -h, --help            show this help message and exit
  -t  [ ...], --target  [ ...]
                        Target IP address or subnet (default: 192.168.1.0/24)
  -i  [ ...], --interface  [ ...]
                        Interface to use (default: None)
  -l, --live            Enable live tracking of devices
  -o , --output         Output file to save the results
  -m , --manufacturer   Filter by manufacturer (e.g., 'Apple')
  -r , --ip-range       Filter by IP range (e.g., '192.168.1.0/24')
  -s , --scan-rate      Scan rate in seconds (default: 5)
Default Scan
$ python3 netprobe.py 
Live Tracking
You can enable live tracking of devices on your network by using the -l or --live flag. This will continuously update the device list every 5 seconds.

$ python3 netprobe.py -t 192.168.1.0/24 -i eth0 -l
Save Results
You can save the scan results to a file by using the -o or --output flag followed by the desired output file name.

$ python3 netprobe.py -t 192.168.1.0/24 -i eth0 -l -o results.txt
┏━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃ IP Address   ┃ MAC Address       ┃ Packet Size ┃ Manufacturer                 ┃
┡━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
│ 192.168.1.1  │ **:6e:**:97:**:28 │ 102         │ ASUSTek COMPUTER INC.        │
│ 192.168.1.3  │ 00:**:22:**:12:** │ 102         │ InPro Comm                   │
│ 192.168.1.2  │ **:32:**:bf:**:00 │ 102         │ Xiaomi Communications Co Ltd │
│ 192.168.1.98 │ d4:**:64:**:5c:** │ 102         │ ASUSTek COMPUTER INC.        │
│ 192.168.1.25 │ **:49:**:00:**:38 │ 102         │ Unknown                      │
└──────────────┴───────────────────┴─────────────┴──────────────────────────────┘
Contact
If you have any questions, suggestions, or feedback about the program, please feel free to reach out to me through any of the following platforms:

Mywebsite: Pankaj
LinkedIn: LinkedIn
TryHackMe: TryHackMe
Instagram: Instagram
YouTube: YouTube
Email: Pk9779817@gmail.com
License
This program is released under the MIT LICENSE. See LICENSE for more information.

Thank you for considering supporting me! Your support enables me to dedicate more time and effort to creating useful tools like DNSWatch and developing new projects. By contributing, you're not only helping me improve existing tools but also inspiring new ideas and innovations. Your support plays a vital role in the growth of this project and future endeavors. Together, let's continue building and learning. Thank you!" BuyMeACoffee Patreon
