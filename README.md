# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output :

```
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\SANTH> ping google.com

Pinging google.com [2404:6800:4007:836::200e] with 32 bytes of data:
Reply from 2404:6800:4007:836::200e: time=245ms
Reply from 2404:6800:4007:836::200e: time=59ms
Reply from 2404:6800:4007:836::200e: time=14ms
Reply from 2404:6800:4007:836::200e: time=16ms

Ping statistics for 2404:6800:4007:836::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 14ms, Maximum = 245ms, Average = 83ms
PS C:\Users\SANTH> ipconfig

Windows IP Configuration


Ethernet adapter Ethernet 2:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::d7b0:413b:e13:8d1d%18
   IPv4 Address. . . . . . . . . . . : 192.168.56.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . : saveetha.in
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:42:0:4e4:e00c:913a
   Link-local IPv6 Address . . . . . : fe80::4618:770:9f9e:c075%6
   Autoconfiguration IPv4 Address. . : 169.254.167.167
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%6
PS C:\Users\SANTH> tracert google.com

Tracing route to google.com [2404:6800:4007:836::200e]
over a maximum of 30 hops:

  1    14 ms     3 ms     6 ms  2403:8600:c090:42::1
  2     *
PS C:\Users\SANTH> nslookup google.com
Server:  UnKnown
Address:  2403:8600:c090:42:a000::200

Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4007:836::200e
          142.251.221.110

PS C:\Users\SANTH> netstat -an

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49670          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:8884         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:58214        127.0.0.1:58215        ESTABLISHED
  TCP    127.0.0.1:58215        127.0.0.1:58214        ESTABLISHED
  TCP    169.254.167.167:139    0.0.0.0:0              LISTENING
  TCP    192.168.56.1:139       0.0.0.0:0              LISTENING
  TCP    [::]:135               [::]:0                 LISTENING
  TCP    [::]:445               [::]:0                 LISTENING
  TCP    [::]:49664             [::]:0                 LISTENING
  TCP    [::]:49665             [::]:0                 LISTENING
  TCP    [::]:49666             [::]:0                 LISTENING
  TCP    [::]:49667             [::]:0                 LISTENING
  TCP    [::]:49668             [::]:0                 LISTENING
  TCP    [::]:49670             [::]:0                 LISTENING
  TCP    [::1]:42050            [::]:0                 LISTENING
  TCP    [::1]:49669            [::]:0                 LISTENING
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:49409  [2603:1040:a06:6::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:49671  [2600:140f:6::17c7:4593]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:49987  [2a06:98c1:3100::6812:202f]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:50096  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:52099  [2606:50c0:8002::215]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:52677  [64:ff9b::8c52:7016]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:52826  [2600:140f:5e00:14::17d3:3c0f]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:52964  [64:ff9b::8c52:7019]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:53091  [2600:140f:5e00:14::17d3:3c09]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:53258  [64:ff9b::14f7:a89e]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:53584  [64:ff9b::1487:60b]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:54199  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:54414  [64:ff9b::12a1:d817]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:54852  [2a03:2880:f36a:120:face:b00c:0:167]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:54881  [2a06:98c1:3100::6812:202f]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:55521  [64:ff9b::d6b:69e]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:55969  [2603:1061:14:150::1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:56098  [2620:1ec:33::12]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:56575  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:56611  [2620:1ec:33:1::11]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57180  [64:ff9b::14be:918e]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57344  [2603:1040:a06:8::1f1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57454  [2620:1ec:33:1::11]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57510  [2620:1ec:33:1::10]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57596  [2603:1063:2001:190b::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57597  [2603:1063:2001:190b::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:57652  [2620:1ec:33::11]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58212  [64:ff9b::cc4f:c5de]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58216  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58308  [2600:1901:0:47fc::]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58523  [2606:50c0:8002::154]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58641  [2620:2d:4000:1::26]:443  CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58642  [2606:4700::6812:14d5]:80  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:58986  [2620:1ec:33:1::10]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:59561  [64:ff9b::1487:60b]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:59618  [64:ff9b::8fa6:1c64]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:59653  [2603:1061:14:155::1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:59758  [2620:1ec:33:1::10]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:60057  [2a03:2880:f36a:120:face:b00c:0:167]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:60269  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:60548  [64:ff9b::284a:62c1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:61426  [64:ff9b::d4e:6da2]:8883  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:61473  [2603:1040:a06:8::1f1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:61991  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:62043  [2404:6800:4003:c04::bc]:5228  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:62532  [64:ff9b::284a:62c1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:62849  [64:ff9b::36f:f1e0]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:63424  [2600:140f:6::17c7:4593]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:63913  [2a06:98c1:3100::6812:202f]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:64203  [64:ff9b::acbc:9b19]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:64516  [64:ff9b::14cf:4955]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4e4:e00c:913a]:65490  [2600:140f:6::17c7:4549]:443  ESTABLISHED
  UDP    0.0.0.0:123            *:*
  UDP    0.0.0.0:5050           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5355           *:*
  UDP    0.0.0.0:51869          23.211.60.35:443
  UDP    0.0.0.0:57438          *:*
  UDP    0.0.0.0:61399          23.211.60.47:443
  UDP    0.0.0.0:63825          *:*
  UDP    0.0.0.0:63879          104.18.32.47:443
  UDP    127.0.0.1:1900         *:*
  UDP    127.0.0.1:49950        *:*
  UDP    127.0.0.1:52835        127.0.0.1:52835
  UDP    169.254.167.167:137    *:*
  UDP    169.254.167.167:138    *:*
  UDP    169.254.167.167:1900   *:*
  UDP    169.254.167.167:49949  *:*
  UDP    192.168.56.1:137       *:*
  UDP    192.168.56.1:138       *:*
  UDP    192.168.56.1:1900      *:*
  UDP    192.168.56.1:49948     *:*
  UDP    [::]:123               *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5355              *:*
  UDP    [::]:51869             [2600:140f:5e00:14::17d3:3c23]:443
  UDP    [::]:51952             *:*
  UDP    [::]:57438             [2600:1901:0:47fc::]:443
  UDP    [::]:59712             *:*
  UDP    [::]:61399             [2600:140f:5e00:14::17d3:3c2f]:443
  UDP    [::]:63825             *:*
  UDP    [::]:63879             [2a06:98c1:3100::6812:202f]:443
  UDP    [::1]:1900             *:*
  UDP    [::1]:49947            *:*
  UDP    [fe80::4618:770:9f9e:c075%6]:1900  *:*
  UDP    [fe80::4618:770:9f9e:c075%6]:49946  *:*
  UDP    [fe80::d7b0:413b:e13:8d1d%18]:1900  *:*
  UDP    [fe80::d7b0:413b:e13:8d1d%18]:49945  *:*
PS C:\Users\SANTH> hostname
SANTHOSH
PS C:\Users\SANTH> getmac

Physical Address    Transport Name
=================== ==========================================================
D8-B3-2F-BD-03-4B   \Device\Tcpip_{2A7F7D56-2979-401A-81FB-C4582F97EFF7}
0A-00-27-00-00-12   \Device\Tcpip_{F4C2CB11-998D-42CA-B051-1FA4B74C8AAB}
PS C:\Users\SANTH> route print
===========================================================================
Interface List
 18...0a 00 27 00 00 12 ......VirtualBox Host-Only Ethernet Adapter
 11...da b3 2f bd 03 4b ......Microsoft Wi-Fi Direct Virtual Adapter
  6...d8 b3 2f bd 03 4b ......Realtek RTL8852BE WiFi 6 802.11ax PCIe Adapter
  1...........................Software Loopback Interface 1
===========================================================================

IPv4 Route Table
===========================================================================
Active Routes:
Network Destination        Netmask          Gateway       Interface  Metric
        127.0.0.0        255.0.0.0         On-link         127.0.0.1    331
        127.0.0.1  255.255.255.255         On-link         127.0.0.1    331
  127.255.255.255  255.255.255.255         On-link         127.0.0.1    331
      169.254.0.0      255.255.0.0         On-link   169.254.167.167    286
  169.254.167.167  255.255.255.255         On-link   169.254.167.167    286
  169.254.255.255  255.255.255.255         On-link   169.254.167.167    286
     192.168.56.0    255.255.255.0         On-link      192.168.56.1    281
     192.168.56.1  255.255.255.255         On-link      192.168.56.1    281
   192.168.56.255  255.255.255.255         On-link      192.168.56.1    281
        224.0.0.0        240.0.0.0         On-link         127.0.0.1    331
        224.0.0.0        240.0.0.0         On-link      192.168.56.1    281
        224.0.0.0        240.0.0.0         On-link   169.254.167.167    286
  255.255.255.255  255.255.255.255         On-link         127.0.0.1    331
  255.255.255.255  255.255.255.255         On-link      192.168.56.1    281
  255.255.255.255  255.255.255.255         On-link   169.254.167.167    286
===========================================================================
Persistent Routes:
  None

IPv6 Route Table
===========================================================================
Active Routes:
 If Metric Network Destination      Gateway
  6    286 ::/0                     fe80::eedd:24ff:fe3d:ced5
  1    331 ::1/128                  On-link
  6    286 2403:8600:c090:42::/84   On-link
  6    286 2403:8600:c090:42:0:4e4:e00c:913a/128
                                    On-link
 18    281 fe80::/64                On-link
  6    286 fe80::/64                On-link
  6    286 fe80::4618:770:9f9e:c075/128
                                    On-link
 18    281 fe80::d7b0:413b:e13:8d1d/128
                                    On-link
  1    331 ff00::/8                 On-link
 18    281 ff00::/8                 On-link
  6    286 ff00::/8                 On-link
===========================================================================
Persistent Routes:
  None
PS C:\Users\SANTH> netsh wlan show profiles

Profiles on interface Wi-Fi:

Group policy profiles (read only)
---------------------------------
    <None>

User profiles
-------------
    All User Profile     : CIT-Campus
    All User Profile     : moto g96 5G_4529
    All User Profile     : Doctor Doom
    All User Profile     : Mithun Sai
    All User Profile     : iQOO Z5
    All User Profile     : SEC_LAB
    All User Profile     : CODING TEST 3
    All User Profile     : CODING TEST 1
    All User Profile     : CODING TEST 2
    All User Profile     : CODING TEST 11
    All User Profile     : CODING TEST 9
    All User Profile     : CODING TEST 10
    All User Profile     : CODING TEST 4
    All User Profile     : CODING TEST 5
    All User Profile     : Sakthi's A16
    All User Profile     : SEC-WiFi
    All User Profile     : iQOO Z10 5G
    All User Profile     : SEC_WIFI
    All User Profile     : CODING TEST 7
    All User Profile     : CODING TEST 6
    All User Profile     : SEC WIFI
    All User Profile     : administrator-MS-7A38
    All User Profile     : ohh net illa ya 😂🥱
    All User Profile     : Redmi Note 14 5G
    All User Profile     : Darknight
    All User Profile     : Nothing Phone (2a) Plus_2494
    All User Profile     : Galaxy F121EC1
    All User Profile     : Redmi Note 13 5G
    All User Profile     : RON IN THE HOOD
    All User Profile     : POCO C65
    All User Profile     : Airtel_Computer store

PS C:\Users\SANTH> arp -a

Interface: 169.254.167.167 --- 0x6
  Internet Address      Physical Address      Type
  169.254.112.209       e0-2e-0b-7a-bc-e6     dynamic
  169.254.163.40        78-0c-b8-80-e9-81     dynamic
  224.0.0.2             01-00-5e-00-00-02     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  224.77.77.77          01-00-5e-4d-4d-4d     static
  225.16.8.68           01-00-5e-10-08-44     static
  230.0.0.1             01-00-5e-00-00-01     static
  239.192.152.143       01-00-5e-40-98-8f     static
  239.255.102.18        01-00-5e-7f-66-12     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static

Interface: 192.168.56.1 --- 0x12
  Internet Address      Physical Address      Type
  192.168.56.255        ff-ff-ff-ff-ff-ff     static
  224.0.0.2             01-00-5e-00-00-02     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  224.77.77.77          01-00-5e-4d-4d-4d     static
  225.16.8.68           01-00-5e-10-08-44     static
  230.0.0.1             01-00-5e-00-00-01     static
  239.192.152.143       01-00-5e-40-98-8f     static
  239.255.102.18        01-00-5e-7f-66-12     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
PS C:\Users\SANTH> pathping google.com

Tracing route to google.com [2404:6800:4007:836::200e]
over a maximum of 30 hops:
  0  SANTHOSH.saveetha.in [2403:8600:c090:42:0:4e4:e00c:913a]
  1  2403:8600:c090:42::1
  2     *        *        *
Computing statistics for 25 seconds...
            Source to Here   This Node/Link
Hop  RTT    Lost/Sent = Pct  Lost/Sent = Pct  Address
  0                                           SANTHOSH.saveetha.in [2403:8600:c090:42:0:4e4:e00c:913a]
                                0/ 100 =  0%   |
  1   26ms     0/ 100 =  0%     0/ 100 =  0%  2403:8600:c090:42::1

Trace complete.
PS C:\Users\SANTH> netsh wlan show interfaces

There is 1 interface on the system:
Network shell commands need location permission to access WLAN information. Turn on Location services on the Location page in Privacy & security settings.

Here is the URI for the Location page in the Settings app:
ms-settings:privacy-location
To open the Location page in the Settings app, hold down the Ctrl key and select the link, or run the following command:
start ms-settings:privacy-location

Or, to open the Location page from the Run dialog box, press Windows logo key + R, and then copy and paste the URI above.

Function WlanQueryInterface returns error 5:
The requested operation requires elevation (Run as administrator).

PS C:\Users\SANTH> ipconfig /flushdns

Windows IP Configuration

Successfully flushed the DNS Resolver Cache.
PS C:\Users\SANTH> netsh interface ipv4 show subinterfaces^C
PS C:\Users\SANTH>
```

## Result
Thus Execution of Network commands Performed 
