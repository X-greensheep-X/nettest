# nettest
runs a variety of tests to assist in diagnosis of network issues:<br />
 1.) check for a NIC in UP state<br />
 2.) check for a NIC with an IP address<br />
 3.) check if there is a default gateway in the routing table<br />
 4.) ping default gateway<br />
 5.) ping Google's DNS (8.8.8.8)<br />
 6.) check if nslookup can resolve google.com, if it cant, it will ping the current DNS server to determine if it can be reached<br />
 8.) confirm internet connectivity and test for captive portal or filter by grabbing a webpage (https://pastebin.com/raw/MURsYtKx)<br />
 9.) measures packet loss by sending out several pings and measuring how many return within 500ms of transmission<br />
 
# syntax
nettest [-e] [--nocolor] <br />
 -e : exit on failure of any test<br />
 --nocolor : don't use ANSI escape codes in output, suitable for use with <code>watch</code>
# prerequisites
 dnsutils: <code>sudo apt install dnsutils</code><br />
 bc : <code>sudo apt install bc</code><br />
