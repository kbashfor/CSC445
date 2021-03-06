# Assignment 2

Write a proxy server program, that relays files/pages. To demonstrate, you'll need a client and a server program:

 * The proxy server awaits connections.
 * A client connects, sends a URL.
 * The proxy server gets the corresponding page/file using HTTP.
 * The proxy sends the page/file to the client, that then uses (stores or displays) it.
 
The proxy server is allowed to, but not required to, cache pages.

Wherever applicable, use the commands and protocol for TFTP ([IETF RFC 1350](http://www.ietf.org/rfc/rfc1350.txt)), with the following modifications:

 * A client only downloads files from the proxy server, never uploads.
 * Support only binary (octet) transmission.
 * Support a command line argument specifiying whether packets are IPv4 vs IPv6 UDP datagrams
 * Support a command line argument specifying to use TCP-style sliding windows rather than the sequential acks used in TFTP. To implement this, you may need to design and use additional packet header information than that in TFTP.
 * Support a command line argument controlling whether to pretend to drop 1 percent of the packets;
Create a web page showing throughput across varying conditions (V4 vs V6; sequential vs windowed acks; drops vs no drops)
