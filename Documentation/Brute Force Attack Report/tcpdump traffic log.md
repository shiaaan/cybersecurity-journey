[tcpdump traffic log.docx](https://github.com/user-attachments/files/20489235/tcpdump.traffic.log.docx)

This capture illustrates two separate sequences of DNS and HTTP traffic originating from a local host (your.machine) to two distinct domains: yummyrecipesforme.com and greatrecipesforme.com. The observed activity is as follows:

DNS Resolution:

The local machine queries Google DNS (dns.google) to resolve the A records for:

yummyrecipesforme.com, which resolves to 203.0.113.22

greatrecipesforme.com, which resolves to 192.0.2.17

HTTP Communication:

Shortly after DNS resolution, the machine initiates TCP connections (three-way handshake) on port 80 (HTTP) with both domains.

HTTP GET requests for the root (/) resource are sent to each server.

Both servers respond with standard ACKs and proceed to transmit content, indicated by subsequent traffic on port 80.

Connection Characteristics:

All communications occur over unencrypted HTTP (port 80).

The presence of full handshakes and HTTP GET requests confirms successful establishment of sessions with both domains.

Timestamps and sequence numbers indicate the requests were made manually or via automated browsing within short time spans.

