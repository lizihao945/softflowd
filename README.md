#How to run
softflowd -D -r data/1MB.dump -v 5 -n 127.0.0.1:41300 > csv.file

##Output Format
Source IPaddr, Source Port, Destination IPaddr, Destination Port, TCP flags, Layer 4 Protocol, Packet Count, Byte Count    

* TCP flags: Protocol state (URG=32, ACK=16, PSH=8, RST=4, SYN=2, FIN=1). For example, a value of 27 indicates the flow had a SYN, ACK, PUSH, and FIN (2+16+8+1=27).
* Layer 4 Protocol: Type of layer 4 protocol. For example, ICMP=1, TCP=6, Telnet=14, UDP=1
