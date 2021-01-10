# nettest
runs a variety of tests to assist in diagnosis of network issues:<br />
 1.) check for a NIC in UP state<br />
 2.) check for a NIC with an IP address<br />
 3.) check if there is a default gateway in the routing table<br />
 4.) ping default gateway<br />
 5.) ping Google's DNS (8.8.8.8)<br />
 6.) check if nslookup can resolve google.com, if it cant, it will ping the current DNS server<br />
 8.) confirm internet connectivity by grabbing a webpage (https://pastebin.com/raw/MURsYtKx)<br />
 
# syntax
nettest [-e] <br />
 -e exit on failure of any test
# prerequisites
 dnsutils: <code>sudo apt install dnsutils</code>
