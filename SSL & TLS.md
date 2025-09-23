# SSL & TLS

## SSL - Secure Socket Layer
## TLS - Transport Layer Security

These are communication protocols used for privacy and data integrity between the client and server. These protocols are used to secure web traffic, email, instant messaging, and other types of internet traffic.

SSL/TLS = ENCRYPTION!

## TLS
- There is both asymmetric and symmetric encryption.
- Asymmetric encryption = server makes public key available to server (that server only) where transfer of keys is not needed.
- Symmetric encryption is better, used for ongoing encryption requirements.
- TLS also provides identity verification where the client usually verifies the server is actually the server it says it is but it can also be used for two way verification to verify the client as well.

## 3 Steps To TLS

1) Cipher Suites
    - Layer 4. Starts when TCP connection is already active between client and server. 
    - Client "Hello" <--> Server "Hello"
    - Server sends public key to client in a certificate.

2) Authentication
    - Client ensures the certificate is valid (public key, DNS name, etc). 
    - Client sends test data for server to decrypt using its private key.

3) Key Exchange
    - Here is where it moves from asymmetric to symmetric encryption.
    - Client generates some test data using the servers public key to encrypt it. This is called the "Pre-Master Key".
    - Once this is sent to the server, the server then decrypts this pre-master key using its private key. At this point, both sides have what is known as a "Master Secret" which keeps the session connection going.