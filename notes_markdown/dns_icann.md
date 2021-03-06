# Domain Names, DNS, and ICANN

## Domain Names 
The Domain Name System (DNS) provides a service to map human-readable names to IP addresses. 
For example. www.google.com to 172.217.165.142. DNS operates in a client-server model where a 
computer is a client when it requests the IP of a given name and as a client when it serves the IP of 
such name. Each name consists of a sequence of alpha-numeric segments separated by periods. 
Domain names are hierarchical with every part separated by a period representing a part of 
that hierarchy. For example:

![Domain name parts](https://rebrand.ly/o86fhpo)

-----------------------------------------

## ICANN
The Domain Name System does not specify the value for the Top Level Domain. TLDs are controlled by 
an organization called Internet Corporation for Assigned Names and Numbers (ICANN). ICANN is an 
American nonprofit organization responsible for the maintenance and procedures of several 
databases related to the namespaces and numerical spaces of the Internet, ensuring the network's 
stable and secure operation. Much of its work has concerned the Internet's global Domain Name 
System (DNS), including policy development for internationalization of the DNS system, 
introduction of new generic top-level domains (TLDs), and the operation of root name servers.  
ICANN's creation was announced publicly on September 17, 1998, and it formally came into 
being on September 30, 1998, incorporated in the U.S. state of California. Originally 
headquartered in Marina del Rey in the same building as the University of Southern California's 
Information Sciences Institute (ISI), its offices are now in the Playa Vista neighborhood of Los A
ngeles in Facebook's old office.

-----------------------------------------

## Top Level Domains
When a company applies for a name under one of the existing top-level domains and the name 
is awarded, the domain name gets registered with the company and other companies cannot register 
the same domain (unless the registration expires). For example, company A registered the domain 
the3rdproject.com, other companies cannot register the same .com domain but they can register .org or .xyz if available. 

| Top Level Domain | Assigned To |
| ---------------- | ----------- |
| COM              | Commercial organizations |
| ORG              | Non-commercial organizations |
| BIZ              | Businesses |
| EDU              | Educational Institutions |
| GOV              | United States government |
| INFO             | Information |
| COUNTRY CODE (US)| A sovereign nation |

Many organizations assign domain names that reflect the role a computer in a given network performs.
For example, a file server in the3rdproject organization may be named: ftp.the3rdproject.com. FTP 
indicates that that computer is running the file transfer protocol. However, using the first label 
in a domain name to denote a service is merely a convention to help humans.

-----------------------------------------

## How does DNS really work?

### The DNS hierarchy
DNS is an autonomous system which means that each organization is free to assign names to computers
 or change them without notifying any authority. This is possible because each organization is 
 allowed to have DNS servers as part of its hierarchy. In the case of the3rdproject, their DNS 
 handles domains ending in the3rdproject.com. This means that their DNS knows the location (ip 
 address) of mail.the3rdproject.com, ftp.the3rdproject.com, server.the3rdproject.com, etc.  
 Another ability of the DNS system is that administrators can replicate DNS servers to provide 
 fault tolerance in environments where DNS servers are heavily used.  

### Name resolution
Name resolution is the conversion of a domain name to an IP address. The software that performs 
this conversion is the name resolver. Each resolver is configured with the address of one or more 
local domain name servers. The resolver forms a DNS request message, sends the message to the 
local server, and waits for the server to send a DNS reply message that contains the answer.
![DNS resolver in action](../assets/dnsresolver.gif)