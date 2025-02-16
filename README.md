# Window-Defender-Firewall
A firewall is a network security device that monitors incoming and outgoing network trafic and decide whether to allow or block specific traffic based.
This project involved validating the effectiveness of firewall on the microsoft window by linking another operating sysyem (kali) operating system through IP address. For this to occur a command called "ping" will be used.
For kali, the IP address was gotten using "ifconfig" at the terminal emulator. for base window, "ipcongfig" was used at the command prompt.
The IP address on the base window was 192.168.96.85 and that of kali was 10.0.2.15
Note: for two operating systems to communicate they must connect to the same network interface.
Since Kali and base window were operating on different network interface, the adjustment was done on Kali to match up that of the base window. From network setting of Kali it was cganged from "NAT" to "BRIDGE ADAPTER" 
After adjustment, the IP address of Kali OS changes to 192.168.96.8 as shown in screenshot-1. This shows that Kali OS and base window are now operating on the same network interface.
Using the command "ping" with the IP address on both operating systems, the result shows that tha base window could communicate the Kali OS because it has 0% packet loss but Kali couldn't communicate because it has 100% packet loss. This is shown in screenshot-2.
This gave room to setting of Inbound and Outbound Rules on the firewall. This is shown in screenshot-3.
Going back to the terminal emulator of the Kali OS, ping with the IP address of the base window (e.g. ping 192.168.96.85, pressing enter key) the packet loss became 0% as shown in screenshot-4. This shows that the OS (Kali and window) were communicating well by allowing traffic between the operating systems
In conclusion, this shows that firewall is an important security device in a system without it, it makes our system to be vulnerable to attacks. 
 
