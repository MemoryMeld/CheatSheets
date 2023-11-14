# Tshark
```bash
-r = read in the pcap 
-n = don't perform hostname resolution 
-q = suppress packet information output 
-z = display statistics of a pcap 
-e = include the specified field in the output 
-T = set the format of output 
-w = write to a file 
-Y = specify display filter
-z io,phs[,filter] - Create Protocol Hierarchy Statistics listing both number of packets and bytes.

TShark -r input.pcap -n -Y 'tcp.dstport==80' -w output.pcap 

TShark -r input.pcap -n -q -z io,phs 

TShark -r input.pcap -n -Y 'http' -T fields -e http.user_agent 

TShark -r input.pcap -n -Y 'http.user_agent' -T fields -e http.user_agent 

TShark -r input.pcap -n -Y 'http.user_agent' -T fields -e http.user_agent | sort | uniq -c | sort -n 
```