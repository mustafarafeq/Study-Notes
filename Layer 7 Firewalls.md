# Layer 7 Firewall - Application Layer Firewall

Layer 7 Firewalls function at Layer 7 of the OSI model which means they have all the functionality of previous layer firewalls such as stateless firewalls plus a bit more functionality.

Also called Application Layer Firewalls
- Provides advances security features by detecting and filtering data at the application layer of the OSI model.
- Inspects and controls traffic based on the specific content and behavior of applications, not just the source and destination IP like layer 3/4 firewalls do.
- Performs deep inspection of packets like looking at HTTP headers, cookies, URL, and the actual payload of data being sent, in order to detect and block sophicaticated threats such as SQL injection, DDos Attacks, etc.

Application Layer Firewalls are typically located between the client and server or "in front" of the server meaning before the request or data reaches the server.

In AWS, the primary application layer firewall is AWS Web Application Firewall or WAF.

A layer 7 firewall keeps all the features of the L3 and L4, and L5 firewalls and can react to the below L7 elements.
    
    - DNS Names
    - Rate of Flow (how many connections per second)
    - Content and Headers.