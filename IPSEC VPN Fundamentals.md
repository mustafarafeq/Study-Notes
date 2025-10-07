# IPSEC
IP SEC = Internet protocol security. A suite of software protocols used to secure IP communications by authenticating and encrypting each IP address.

- Widely used to secure VPN Tunnels (Virtual Private Network), remote access connections (RDP), and other types of network traffic.

- IPSEC sets up secure tunnels across insecure networks between peers. Also provides authentication and encryption.

Inside of these peer-to-peer tunnels, there is what is known as "Interesting traffic", which is traffic that follows certain rules.

- The traffic could be based on network prefixes, or other rules.
- If data is contained that matches any of the rules, then a VPN tunnel is created to get it to its destination.
- Any data that is in transit within the tunnel is encrypted even in an insecure network.

***Remember Asymmetric/Symmetric Encryption***

# IPSEC Phases

## Phase 1: IKE Phase
- Internet key exchange (slow and heavy)
- Authenticate - Pre shared key (password/certificate)
- Asymmetric Encryption to agree on and create Symmetric key.
- The end of IKE Phase 1 results in a tunnel or "Security Association"

## Phase 2 : IKE Phase 2

- Uses the keys agreed in phase 1
- agree on an encryption method and keys used for bulk data transfer.
- Create IPSEC SA (security association)
- This runs over phase 1

## Diffie Hellman Key Exchange

After authentication in IKE Phase 1, each side creates a DH private key that is used to decrypt data and sign things.
Each side uses this private key to derive a corresponding public key.

- Private Key: Decrypt Data
- Public Key: Encrypt Data

The final step in the whole process is each side generates a symmetrical key and the Phase 1 tunnel is created.
