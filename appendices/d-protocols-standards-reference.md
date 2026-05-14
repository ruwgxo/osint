# 20260131 | OSINT: Appendices (Chapter 31.4 Protocol and Standards Reference) by Raghav Dinesh  
#wrap #paper  
  
**Contents**  
|‣ Open Source Intelligence  
|‣‣ Appendices  
|‣‣‣ Protocol and Standards Reference  
1. Essential RFC documents for OSINT  
2. Internet protocol specifications  
3. Web technology standard references  
4. Cryptographic standard implementations  
5. Data format specifications  
6. API documentation standards  
7. Security protocol references  
  
  
**Protocol and Standards Reference**  
This appendix provides essential protocol specifications and technical standards reference materials for OSINT practitioners, including RFC documents, internet protocols, web technologies, cryptographic standards, and security protocols.  
  
  
1. **Essential RFC Documents for OSINT**  
  
**Core Internet Protocols**  
- RFC 791 - Internet Protocol (IPv4)  
- RFC 2460 - Internet Protocol Version 6 (IPv6)  
- RFC 793 - Transmission Control Protocol (TCP)  
- RFC 768 - User Datagram Protocol (UDP)  
  
**RFC 791 - Internet Protocol (IPv4)**  
Date: September 1981 Status: Internet Standard Summary: Defines the Internet Protocol version 4, including packet format, addressing, and routing.  
  
Key OSINT Applications:  
- IP address geolocation and attribution  
- Network topology mapping  
- Traffic flow analysis  
- Infrastructure reconnaissance  
  
Header Fields of Interest:  
- Source Address (32 bits): Origin of packet  
- Destination Address (32 bits): Target of packet  
- Time to Live (8 bits): Maximum hop count  
- Protocol (8 bits): Next level protocol identifier  
  
**RFC 2460 - Internet Protocol Version 6 (IPv6)**  
Date: December 1998 Status: Internet Standard Summary: Specification for IPv6, the next generation Internet Protocol.  
  
Key OSINT Applications:  
- Next-generation network analysis  
- Extended address space tracking  
- Enhanced security analysis  
- Mobile device tracking  
  
IPv6 Address Types:  
- Unicast: Single interface identifier  
- Multicast: Group communication  
- Anycast: Nearest of multiple interfaces  
  
**RFC 793 - Transmission Control Protocol (TCP)**  
Date: September 1981 Status: Internet Standard Summary: Defines TCP for reliable, ordered delivery of data streams.  
  
Key OSINT Applications:  
- Connection analysis and tracking  
- Service identification  
- Session reconstruction  
- Traffic pattern analysis  
  
TCP Flags for Analysis:  
- SYN: Connection initiation  
- ACK: Acknowledgment  
- FIN: Connection termination  
- RST: Connection reset  
- PSH: Push data immediately  
- URG: Urgent data pointer  
  
**RFC 768 - User Datagram Protocol (UDP)**  
Date: August 1980 Status: Internet Standard Summary: Simple, connectionless transport protocol.  
  
Key OSINT Applications:  
- DNS query analysis  
- Real-time communication tracking  
- Gaming and streaming analysis  
- IoT device communication  
  
**Domain Name System (DNS)**  
- RFC 1035 - Domain Names - Implementation and Specification  
- RFC 3596 - DNS Extensions to Support IPv6  
  
**RFC 1035 - Domain Names - Implementation and Specification**  
Date: November 1987 Status: Internet Standard Summary: Core DNS specification defining domain name structure and resolution.  
  
Key OSINT Applications:  
- Domain ownership research  
- Infrastructure mapping  
- Subdomain enumeration  
- DNS tunneling detection  
  
DNS Message Structure:  
```
Header (12 bytes)
Question Section (variable)
Answer Section (variable)
Authority Section (variable)
Additional Section (variable)

```
  
**RFC 3596 - DNS Extensions to Support IPv6**  
Date: October 2003 Status: Internet Standard Summary: Defines AAAA records for IPv6 address resolution.  
RFC 4034 - Resource Records for DNS Security Extensions  
Date: March 2005 Status: Proposed Standard Summary: Defines DNSSEC resource records for DNS security.  
  
DNSSEC Record Types:  
- DNSKEY: Public key for verification  
- RRSIG: Digital signature  
- DS: Delegation Signer  
- NSEC/NSEC3: Authenticated denial of existence  
  
**HTTP and Web Technologies**  
- RFC 7230 - Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing  
- RFC 7540 - Hypertext Transfer Protocol Version 2 (HTTP/2)  
- RFC 6455 - The WebSocket Protocol  
  
**RFC 7230 - Hypertext Transfer Protocol (HTTP/1.1): Message Syntax and Routing**  
Date: June 2014 Status: Proposed Standard Summary: Core HTTP/1.1 specification for web communication.  
Key OSINT Applications:  
- Web traffic analysis  
- User behavior tracking  
- Content analysis  
- Server identification  
HTTP Request Methods:  
- GET: Retrieve resource  
- POST: Submit data  
- PUT: Update resource  
- DELETE: Remove resource  
- HEAD: Get headers only  
- OPTIONS: Query supported methods  
  
**RFC 7540 - Hypertext Transfer Protocol Version 2 (HTTP/2)**  
Date: May 2015 Status: Proposed Standard Summary: Major revision of HTTP with performance improvements.  
Key Features for Analysis:  
- Binary protocol format  
- Request/response multiplexing  
- Server push capability  
- Header compression (HPACK)  
  
**RFC 6455 - The WebSocket Protocol**  
Date: December 2011 Status: Proposed Standard Summary: Full-duplex communication protocol over TCP.  
  
OSINT Applications:  
- Real-time communication monitoring  
- Chat and messaging analysis  
- Live data stream analysis  
- Interactive application tracking  
  
**Email Protocols**  
- RFC 5321 - Simple Mail Transfer Protocol (SMTP)  
- RFC 3501 - Internet Message Access Protocol (IMAP) Version 4rev1  
  
**RFC 5321 - Simple Mail Transfer Protocol (SMTP)**  
Date: October 2008 Status: Draft Standard Summary: Protocol for email transmission between servers.  
  
Key OSINT Applications:  
- Email routing analysis  
- Server identification  
- Spam source tracking  
- Email authentication  
  
SMTP Commands:  
- HELO/EHLO: Identify sending server  
- MAIL FROM: Specify sender  
- RCPT TO: Specify recipient  
- DATA: Begin message content  
- QUIT: End session  
  
**RFC 3501 - Internet Message Access Protocol (IMAP) Version 4rev1**  
Date: March 2003 Status: Proposed Standard Summary: Protocol for accessing and managing email on a server.  
RFC 1939 - Post Office Protocol - Version 3 (POP3)  
Date: May 1996 Status: Internet Standard Summary: Protocol for retrieving email from a server.  
  
**Security Protocols**  
- RFC 5246 - The Transport Layer Security (TLS) Protocol Version 1.2  
- RFC 8446 - The Transport Layer Security (TLS) Protocol Version 1.3  
  
**RFC 5246 - The Transport Layer Security (TLS) Protocol Version 1.2**  
Date: August 2008 Status: Proposed Standard Summary: Cryptographic protocol for secure communications.  
Key OSINT Applications:  
- Certificate analysis  
- Cipher suite identification  
- Security assessment  
- Encrypted traffic analysis  
  
TLS Handshake Process:  
- ClientHello  
- ServerHello  
- Certificate exchange  
- Key exchange  
- Certificate verification  
- Finished messages  
  
**RFC 8446 - The Transport Layer Security (TLS) Protocol Version 1.3**  
Date: August 2018 Status: Proposed Standard Summary: Latest version of TLS with improved security and performance.  
  
Key Improvements:  
- Reduced handshake latency  
- Improved forward secrecy  
- Simplified cipher suite negotiation  
- Enhanced privacy protection  
  
  
2. **Internet Protocol Specifications**  
  
**IPv4 Addressing and Subnetting**  
- Private Address Ranges (RFC 1918)  
- Special-Use IPv4 Addresses  
- Subnet Mask Calculations  
  
**Private Address Ranges (RFC 1918)**  
- Class A: 10.0.0.0/8 (10.0.0.0 - 10.255.255.255)  
- Class B: 172.16.0.0/12 (172.16.0.0 - 172.31.255.255)  
- Class C: 192.168.0.0/16 (192.168.0.0 - 192.168.255.255)  
  
**Special-Use IPv4 Addresses**  
- Loopback: 127.0.0.0/8  
- Link-Local: 169.254.0.0/16  
- Multicast: 224.0.0.0/4  
- Reserved: 240.0.0.0/4  
  
**Subnet Mask Calculations**  

| CIDR | Subnet Mask     | Network Bits | Host Bits | Max Hosts |
| ---- | --------------- | ------------ | --------- | --------- |
| /24  | 255.255.255.0   | 24           | 8         | 254       |
| /25  | 255.255.255.128 | 25           | 7         | 126       |
| /26  | 255.255.255.192 | 26           | 6         | 62        |
| /27  | 255.255.255.224 | 27           | 5         | 30        |
| /28  | 255.255.255.240 | 28           | 4         | 14        |
| /29  | 255.255.255.248 | 29           | 3         | 6         |
| /30  | 255.255.255.252 | 30           | 2         | 2         |
  
  
**IPv6 Addressing Structure**  
- IPv6 Address Format  
- IPv6 Address Types  
- IPv6 Special Addresses  
  
**IPv6 Address Format**  
- Length: 128 bits (16 bytes)  
- Notation: 8 groups of 4 hexadecimal digits  
- Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334  
- Compressed: 2001:db8:85a3::8a2e:370:7334  
  
**IPv6 Address Types**  
- Global Unicast: 2000::/3  
- Link-Local: FE80::/10  
- Unique Local: FC00::/7  
- Multicast: FF00::/8  
- Loopback: ::1/128  
- Unspecified: ::/128  
  
**IPv6 Special Addresses**  
- 6to4: 2002::/16 (IPv6 over IPv4 tunneling)  
- Teredo: 2001::/32 (NAT traversal)  
- Documentation: 2001:DB8::/32  
  
**Routing Protocol Specifications**  
- Border Gateway Protocol (BGP) - RFC 4271  
- IPv6 Special Addresses  
  
**Border Gateway Protocol (BGP) - RFC 4271**  
Key OSINT Applications:  
- Internet routing analysis  
- ASN (Autonomous System Number) research  
- Network path analysis  
- BGP hijacking detection  
  
BGP Message Types:  
- OPEN: Establish BGP session  
- UPDATE: Advertise/withdraw routes  
- NOTIFICATION: Error conditions  
- KEEPALIVE: Maintain session  
  
**Open Shortest Path First (OSPF) - RFC 2328**  
- Applications: Internal network topology discovery  
- Routing Information Protocol (RIP) - RFC 2453  
- Applications: Small network analysis  
  
  
3. **Web Technology Standard References**  
  
**HTML5 Specification**  
- Document Structure Elements  
- Metadata Elements for OSINT  
- Geolocation API  
  
Document Structure Elements  
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <!-- Content -->
</body>
</html>

```
  
Metadata Elements for OSINT  
- Author: <meta name="author" content="John Doe">  
- Description: <meta name="description" content="Page description">  
- Keywords: <meta name="keywords" content="keyword1, keyword2">  
- Generator: <meta name="generator" content="WordPress 5.8">  
- Date: <meta name="date" content="2023-01-15">  
  
Geolocation API  
```
navigator.geolocation.getCurrentPosition(success, error, options);

```
  
Accuracy Levels:  
- Desktop: ~1000-5000 meters  
- Mobile GPS: ~5-10 meters  
- Mobile Network: ~100-1000 meters  
  
**CSS Selectors for Data Extraction**  
- Basic Selectors  
- Advanced Selectors  
- Pseudo-Selectors  
  
Basic Selectors  
- Universal: * (all elements)  
- Type: div (all div elements)  
- Class: .classname (elements with specific class)  
- ID: #idname (element with specific ID)  
- Attribute: [attribute] (elements with attribute)  
  
Advanced Selectors  
- Descendant: div p (p inside div)  
- Child: div > p (direct p child of div)  
- Adjacent Sibling: div + p (p immediately after div)  
- General Sibling: div ~ p (p siblings after div)  
  
Pseudo-Selectors  
- First Child: :first-child  
- Last Child: :last-child  
- Nth Child: :nth-child(n)  
- Contains: :contains("text")  
  
**JavaScript APIs for OSINT**  
- Geolocation API  
- Canvas Fingerprinting  
- WebRTC IP Detection  
  
Geolocation API  
```
// Get current position
navigator.geolocation.getCurrentPosition(
    function(position) {
        const lat = position.coords.latitude;
        const lon = position.coords.longitude;
        const accuracy = position.coords.accuracy;
    }
);

```
  
Canvas Fingerprinting  
```
// Canvas fingerprinting detection
const canvas = document.createElement('canvas');
const ctx = canvas.getContext('2d');
ctx.textBaseline = 'top';
ctx.font = '14px Arial';
ctx.fillText('Browser fingerprint text', 2, 2);
const fingerprint = canvas.toDataURL();

```
  
WebRTC IP Detection  
```
// WebRTC local IP detection
const pc = new RTCPeerConnection({iceServers:[]});
pc.createDataChannel('');
pc.createOffer().then(offer => pc.setLocalDescription(offer));
pc.onicecandidate = function(ice) {
    if (ice.candidate) {
        const ip = /([0-9]{1,3}(\.[0-9]{1,3}){3})/.exec(ice.candidate.candidate)[1];
        console.log('Local IP:', ip);
    }
};

```
  
  
4. **Cryptographic Standard Implementations**  
  
**Symmetric Encryption Standards**  
- Advanced Encryption Standard (AES) - FIPS 197  
- Data Encryption Standard (DES) - FIPS 46  
- **Triple DES (3DES) - FIPS 46-3**  
  
**Advanced Encryption Standard (AES) - FIPS 197**  
Key Sizes: 128, 192, 256 bits  
Block Size: 128 bits   
Modes of Operation:  
- ECB: Electronic Codebook (not recommended)  
- CBC: Cipher Block Chaining  
- CFB: Cipher Feedback  
- OFB: Output Feedback  
- CTR: Counter Mode  
- GCM: Galois/Counter Mode (authenticated)  
  
AES-256-GCM Example Usage:  
```
# Python example using cryptography library
from cryptography.fernet import Fernet
from cryptography.hazmat.primitives.ciphers.aead import AESGCM

key = AESGCM.generate_key(bit_length=256)
aesgcm = AESGCM(key)
nonce = os.urandom(12)
ct = aesgcm.encrypt(nonce, data, aad)

```
  
**Data Encryption Standard (DES) - FIPS 46**  
- Status: Deprecated due to small key size  
- Key Size: 56 bits (64 bits with parity)  
- Block Size: 64 bits  
  
**Triple DES (3DES) - FIPS 46-3**  
- Status: Legacy, being phased out Key Size: 112 or 168 bits effective Block Size: 64 bits  
  
**Asymmetric Encryption Standards**  
- **RSA (Rivest-Shamir-Adleman)**  
- **Elliptic Curve Cryptography (ECC)**  
  
**RSA (Rivest-Shamir-Adleman)**  
Key Sizes: 1024, 2048, 3072, 4096 bits Security Level:  
- 1024-bit: Deprecated  
- 2048-bit: Minimum recommended  
- 3072-bit: Good security margin  
- 4096-bit: High security  
  
RSA Key Generation Process:  
- Choose two large prime numbers p and q  
- Compute n = p × q  
- Compute φ(n) = (p-1)(q-1)  
- Choose e such that gcd(e, φ(n)) = 1  
- Compute d such that d × e ≡ 1 (mod φ(n))  
- Public key: (n, e), Private key: (n, d)  
  
**Elliptic Curve Cryptography (ECC)**  
Common Curves:  
- P-256 (secp256r1): 256-bit prime field  
- P-384 (secp384r1): 384-bit prime field  
- P-521 (secp521r1): 521-bit prime field  
- Curve25519: High-security curve  
- Ed25519: Edwards curve for signatures  
  
ECC vs RSA Security Equivalence:  
- 256-bit ECC ≈ 3072-bit RSA  
- 384-bit ECC ≈ 7680-bit RSA  
- 521-bit ECC ≈ 15360-bit RSA  
  
**Hash Functions**  
- SHA-2 Family (FIPS 180-4)  
- SHA-3 (Keccak) - FIPS 202  
- Legacy Hash Functions (Deprecated)  
  
SHA-2 Family (FIPS 180-4)  
- SHA-224: 224-bit hash, 512-bit blocks  
- SHA-256: 256-bit hash, 512-bit blocks  
- SHA-384: 384-bit hash, 1024-bit blocks  
- SHA-512: 512-bit hash, 1024-bit blocks  
  
SHA-3 (Keccak) - FIPS 202  
- SHA3-224: 224-bit hash  
- SHA3-256: 256-bit hash  
- SHA3-384: 384-bit hash  
- SHA3-512: 512-bit hash  
- SHAKE128/SHAKE256: Extendable-output functions  
  
Legacy Hash Functions (Deprecated)  
- MD5: 128-bit hash, cryptographically broken  
- SHA-1: 160-bit hash, deprecated for security  
  
**Digital Signatures**  
- RSA Signature Schemes  
- DSA (Digital Signature Algorithm) - FIPS 186-4  
- ECDSA (Elliptic Curve DSA)  
- EdDSA (Edwards-curve Digital Signature Algorithm)  
  
**RSA Signature Schemes**  
- **PKCS#1 v1.5**: Legacy padding scheme  
- **PSS**: Probabilistic Signature Scheme (recommended)  
  
**DSA (Digital Signature Algorithm) - FIPS 186-4**  
- **Key Sizes**: 1024, 2048, 3072 bits  
- **Hash Functions**: SHA-1 (deprecated), SHA-2 family  
  
**ECDSA (Elliptic Curve DSA)**  
- **Curves**: P-256, P-384, P-521  
- **Advantages**: Smaller key sizes, faster operations  
  
**EdDSA (Edwards-curve Digital Signature Algorithm)**  
- **Variants**: Ed25519, Ed448  
- **Benefits**: High security, resistance to implementation errors  
  
  
5. **Data Format Specifications**  
  
**JSON (JavaScript Object Notation) - RFC 7159**  
- Basic Structure  
- JSON Schema for Validation  
  
Basic Structure  
```
{
    "name": "John Doe",
    "age": 30,
    "email": "john@example.com",
    "address": {
        "street": "123 Main St",
        "city": "Anytown",
        "zipcode": "12345"
    },
    "phones": ["555-1234", "555-5678"]
}

```
JSON Schema for Validation  
```
{
    "$schema": "https://json-schema.org/draft/2020-12/schema",
    "type": "object",
    "properties": {
        "name": {"type": "string"},
        "age": {"type": "integer", "minimum": 0},
        "email": {"type": "string", "format": "email"}
    },
    "required": ["name", "age"]
}

```
  
**XML (Extensible Markup Language)**  
- Basic Structure  
- XML Namespaces  
  
Basic Structure  
```
<?xml version="1.0" encoding="UTF-8"?>
<person>
    <name>John Doe</name>
    <age>30</age>
    <email>john@example.com</email>
    <address>
        <street>123 Main St</street>
        <city>Anytown</city>
        <zipcode>12345</zipcode>
    </address>
</person>

```
  
XML Namespaces  
```

<root xmlns:person="http://example.com/person"
      xmlns:address="http://example.com/address">
    <person:name>John Doe</person:name>
    <address:street>123 Main St</address:street>
</root>

```
  
  
**CSV (Comma-Separated Values) - RFC 4180**  
Basic Format Rules  
- Records separated by line breaks (CRLF)  
- Fields separated by commas  
- Fields containing commas, quotes, or line breaks must be quoted  
- Quotes within fields are escaped by doubling  
  
Example  
```
Name,Age,Email,City
"Doe, John",30,john@example.com,Anytown
"Smith, Jane",25,jane@example.com,"New York, NY"

```
  
**YAML (YAML Ain't Markup Language)**  
Basic Structure  
```
person:
  name: John Doe
  age: 30
  email: john@example.com
  address:
    street: 123 Main St
    city: Anytown
    zipcode: "12345"
  phones:
    - "555-1234"
    - "555-5678"

```
  
  
6. **API Documentation Standards**  
  
**REST API Design Principles**  
- HTTP Methods and Their Uses  
- Status Codes for API Responses  
- REST API URL Structure  
  
HTTP Methods and Their Uses  
- GET: Retrieve resources (idempotent, safe)  
- POST: Create new resources  
- PUT: Update/replace entire resource (idempotent)  
- PATCH: Partial resource update  
- DELETE: Remove resources (idempotent)  
- HEAD: Get resource headers only  
- OPTIONS: Query supported methods  
  
**Status Codes for API Responses**  
- 2xx Success  
- 4xx Client Errors  
- 5xx Server Errors  
  
2xx Success:  
- 200 OK: Request successful  
- 201 Created: Resource created  
- 202 Accepted: Request accepted for processing  
- 204 No Content: Successful but no content returned  
  
4xx Client Errors:  
- 400 Bad Request: Invalid request syntax  
- 401 Unauthorized: Authentication required  
- 403 Forbidden: Access denied  
- 404 Not Found: Resource not found  
- 429 Too Many Requests: Rate limit exceeded  
  
5xx Server Errors:  
- 500 Internal Server Error: Generic server error  
- 502 Bad Gateway: Invalid upstream response  
- 503 Service Unavailable: Server temporarily unavailable  
  
REST API URL Structure  
```
https://api.example.com/v1/users/123/posts
└─────┬─────┘ └──┬──┘ └┬┘ └──┬──┘ └─┬─┘
   Base URL    Version API  Resource Collection

```
  
**OpenAPI Specification (Swagger)**  
Basic OpenAPI Document Structure  
```
openapi: 3.0.3
info:
  title: Example API
  version: 1.0.0
  description: Example API for OSINT data collection
servers:
  - url: https://api.example.com/v1
paths:
  /users/{userId}:
    get:
      summary: Get user by ID
      parameters:
        - name: userId
          in: path
          required: true
          schema:
            type: integer
      responses:
        '200':
          description: User details
          content:
            application/json:
              schema:
                $ref: '#/components/schemas/User'
components:
  schemas:
    User:
      type: object
      properties:
        id:
          type: integer
        name:
          type: string
        email:
          type: string
          format: email

```
  
**GraphQL Standards**  
- Basic Query Structure  
- Mutation Example  
  
Basic Query Structure  
```
query GetUser($userId: ID!) {
  user(id: $userId) {
    id
    name
    email
    posts {
      id
      title
      publishedAt
    }
  }
}

```
  
Mutation Example  
```
mutation CreatePost($input: PostInput!) {
  createPost(input: $input) {
    id
    title
    content
    author {
      name
    }
  }
}

```
  
  
7. **Security Protocol References**  
  
**TLS/SSL Implementation Details**  
- Cipher Suite Format  
- Recommended Cipher Suites (2023)  
- Certificate Fields for Analysis  
  
Cipher Suite Format  
```
TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384
 │    │     │    │      │   │   │
 │    │     │    │      │   │   └── MAC algorithm
 │    │     │    │      │   └────── AEAD algorithm
 │    │     │    │      └────────── Encryption algorithm
 │    │     │    └───────────────── Key size
 │    │     └────────────────────── Bulk encryption algorithm
 │    └──────────────────────────── Authentication algorithm
 └───────────────────────────────── Key exchange algorithm

```
Recommended Cipher Suites (2023)  
TLS 1.3:  
- TLS_AES_256_GCM_SHA384  
- TLS_AES_128_GCM_SHA256  
- TLS_CHACHA20_POLY1305_SHA256  
  
TLS 1.2:  
- TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384  
- TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256  
- TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256  
  
Certificate Fields for Analysis  
```
Subject: CN=example.com, O=Example Corp, C=US
Issuer: CN=DigiCert SHA2 High Assurance Server CA
Serial Number: 0x1234567890abcdef
Not Before: Jan 1 00:00:00 2023 GMT
Not After: Jan 1 23:59:59 2024 GMT
Subject Alternative Names: example.com, www.example.com, api.example.com

```
  
**SSH Protocol (RFC 4251)**  
- SSH Connection Process  
- SSH Key Types  
- SSH Configuration Analysis  
  
SSH Connection Process  
- Protocol Version Exchange: Client and server exchange version strings  
- Algorithm Negotiation: Agree on encryption, MAC, and compression algorithms  
- Key Exchange: Establish shared secret using Diffie-Hellman  
- Authentication: User authentication (password, key, etc.)  
- Channel Setup: Establish encrypted communication channels  
  
SSH Key Types  
- RSA: Legacy, minimum 2048-bit recommended  
- ECDSA: Elliptic curve, 256/384/521-bit  
- Ed25519: Modern, high-security curve  
- DSA: Deprecated  
  
SSH Configuration Analysis  
```
# Common SSH configuration locations
~/.ssh/config          # User configuration
/etc/ssh/ssh_config    # System-wide client config
/etc/ssh/sshd_config   # Server configuration
~/.ssh/authorized_keys # Authorized public keys
~/.ssh/known_hosts     # Known server fingerprints

```
  
**IPSec Protocol Suite**  
- IPSec Protocols  
- IPSec Modes  
- IPSec Security Associations (SA)  
  
IPSec Protocols  
- AH (Authentication Header): Provides authentication and integrity  
- ESP (Encapsulating Security Payload): Provides confidentiality, authentication, and integrity  
- IKE (Internet Key Exchange): Key management protocol  
  
IPSec Modes  
- Transport Mode: Protects payload only  
- Tunnel Mode: Protects entire IP packet  
  
IPSec Security Associations (SA)  
Parameters that define IPSec connection:  
- Security Parameter Index (SPI)  
- Destination IP address  
- Security protocol (AH or ESP)  
- Encryption algorithm and keys  
- Authentication algorithm and keys  
