# 20260131 | OSINT: Appendices (Chapter 31.1 Technical Reference) by Raghav Dinesh  
#wrap #paper  
  
**Contents**  
|‣ Open Source Intelligence  
|‣‣ Appendices  
|‣‣‣ Technical Reference  
1. Common port numbers and services  
2. HTTP status codes and meanings  
3. DNS record types and purposes  
4. File signatures (magic numbers) directory  
5. Character encoding reference tables  
6. Regular expression syntax quick reference  
7. Network protocol header structures  
  
  
**Technical Reference**  
This technical reference provides quick access to essential technical information for OSINT practitioners, including common protocols, file formats, and technical specifications needed for effective intelligence collection and analysis.  
  
  
1. **Common Port Numbers and Services**  
  
**Well-Known Ports (0-1023)**  

| Port | Protocol | Service | Description |
| ---- | -------- | --------------- | ------------------------------------------ |
| 20 | TCP | FTP-DATA | File Transfer Protocol Data |
| 21 | TCP | FTP | File Transfer Protocol Control |
| 22 | TCP | SSH | Secure Shell |
| 23 | TCP | TELNET | Telnet Protocol |
| 25 | TCP | SMTP | Simple Mail Transfer Protocol |
| 53 | TCP/UDP | DNS | Domain Name System |
| 67 | UDP | DHCP-SERVER | Dynamic Host Configuration Protocol Server |
| 68 | UDP | DHCP-CLIENT | Dynamic Host Configuration Protocol Client |
| 69 | UDP | TFTP | Trivial File Transfer Protocol |
| 80 | TCP | HTTP | Hypertext Transfer Protocol |
| 110 | TCP | POP3 | Post Office Protocol v3 |
| 119 | TCP | NNTP | Network News Transfer Protocol |
| 123 | UDP | NTP | Network Time Protocol |
| 143 | TCP | IMAP | Internet Message Access Protocol |
| 161 | UDP | SNMP | Simple Network Management Protocol |
| 194 | TCP | IRC | Internet Relay Chat |
| 443 | TCP | HTTPS | HTTP over TLS/SSL |
| 465 | TCP | SMTPS | SMTP over TLS/SSL |
| 587 | TCP | SMTP-SUBMISSION | SMTP Message Submission |
| 636 | TCP | LDAPS | LDAP over TLS/SSL |
| 993 | TCP | IMAPS | IMAP over TLS/SSL |
| 995 | TCP | POP3S | POP3 over TLS/SSL |
  
  
**Registered Ports (1024-49151)**  

| Port  | Protocol | Service       | Description                         |
| ----- | -------- | ------------- | ----------------------------------- |
| 1433  | TCP      | MS-SQL        | Microsoft SQL Server                |
| 1521  | TCP      | ORACLE        | Oracle Database                     |
| 1723  | TCP      | PPTP          | Point-to-Point Tunneling Protocol   |
| 1883  | TCP      | MQTT          | Message Queuing Telemetry Transport |
| 3306  | TCP      | MYSQL         | MySQL Database                      |
| 3389  | TCP      | RDP           | Remote Desktop Protocol             |
| 5432  | TCP      | POSTGRESQL    | PostgreSQL Database                 |
| 5672  | TCP      | AMQP          | Advanced Message Queuing Protocol   |
| 5900  | TCP      | VNC           | Virtual Network Computing           |
| 6379  | TCP      | REDIS         | Redis Database                      |
| 8080  | TCP      | HTTP-ALT      | Alternative HTTP Port               |
| 8443  | TCP      | HTTPS-ALT     | Alternative HTTPS Port              |
| 9200  | TCP      | ELASTICSEARCH | Elasticsearch REST API              |
| 27017 | TCP      | MONGODB       | MongoDB Database                    |
  
  
**HTTP Status Codes and Meanings**  
**1xx Informational Responses**  

| Code | Message             | Description                                   |
| ---- | ------------------- | --------------------------------------------- |
| 100  | Continue            | Request received, continue with request       |
| 101  | Switching Protocols | Server switching protocols per client request |
| 102  | Processing          | Server processing request (WebDAV)            |
  
**2xx Success**  

| Code | Message         | Description                                |
| ---- | --------------- | ------------------------------------------ |
| 200  | OK              | Request successful                         |
| 201  | Created         | Resource created successfully              |
| 202  | Accepted        | Request accepted for processing            |
| 204  | No Content      | Request successful, no content to return   |
| 206  | Partial Content | Partial resource delivered (range request) |
  
**3xx Redirection**  

| Code | Message            | Description                             |
| ---- | ------------------ | --------------------------------------- |
| 301  | Moved Permanently  | Resource permanently moved to new URL   |
| 302  | Found              | Resource temporarily at different URL   |
| 304  | Not Modified       | Resource not changed since last request |
| 307  | Temporary Redirect | Resource temporarily at different URL   |
| 308  | Permanent Redirect | Resource permanently moved to new URL   |
  
**4xx Client Errors**  

| Code | Message                | Description                           |
| ---- | ---------------------- | ------------------------------------- |
| 400  | Bad Request            | Malformed request syntax              |
| 401  | Unauthorized           | Authentication required               |
| 403  | Forbidden              | Server understood but refused request |
| 404  | Not Found              | Resource not found                    |
| 405  | Method Not Allowed     | HTTP method not supported             |
| 406  | Not Acceptable         | Cannot produce acceptable response    |
| 408  | Request Timeout        | Server timeout waiting for request    |
| 409  | Conflict               | Request conflicts with current state  |
| 410  | Gone                   | Resource no longer available          |
| 413  | Payload Too Large      | Request entity too large              |
| 414  | URI Too Long           | Request URI too long                  |
| 415  | Unsupported Media Type | Media type not supported              |
| 418  | I'm a teapot           | RFC 2324 April Fools' joke            |
| 429  | Too Many Requests      | Rate limit exceeded                   |
  
**5xx Server Errors**  

| Code | Message                    | Description                           |
| ---- | -------------------------- | ------------------------------------- |
| 500  | Internal Server Error      | Generic server error                  |
| 501  | Not Implemented            | Server doesn't support functionality  |
| 502  | Bad Gateway                | Invalid response from upstream server |
| 503  | Service Unavailable        | Server temporarily unavailable        |
| 504  | Gateway Timeout            | Upstream server timeout               |
| 505  | HTTP Version Not Supported | HTTP version not supported            |
  
  
**DNS Record Types and Purposes**  
**Core DNS Record Types**  

| Type | Purpose | Example |
| ----- | ---------------------- | ---------------------------------------------------------- |
| A | IPv4 address mapping | example.com. IN A 192.0.2.1 |
| AAAA | IPv6 address mapping | example.com. IN AAAA 2001:db8::1 |
| CNAME | Canonical name alias | www.example.com. IN CNAME example.com. |
| MX | Mail exchange server | example.com. IN MX 10 mail.example.com. |
| NS | Name server delegation | example.com. IN NS ns1.example.com. |
| SOA | Start of authority | Contains zone metadata |
| PTR | Reverse DNS lookup | 1.2.0.192.in-addr.arpa. IN PTR example.com. |
| TXT | Text records | example.com. IN TXT "v=spf1 include:_spf.example.com ~all" |
  
**Extended DNS Record Types**  

| Type | Purpose | Example |
| ------ | ----------------------------------- | --------------------------------------------------------- |
| SRV | Service location | _sip._tcp.example.com. IN SRV 10 60 5060 sip.example.com. |
| CAA | Certificate authority authorization | example.com. IN CAA 0 issue "letsencrypt.org" |
| DNAME | Domain name redirection | example.com. IN DNAME example.net. |
| DNSKEY | DNS public key | Used in DNSSEC |
| DS | Delegation signer | Used in DNSSEC |
| RRSIG | Resource record signature | Used in DNSSEC |
| NSEC | Next secure record | Used in DNSSEC |
| NSEC3 | Next secure record v3 | Used in DNSSEC |
  
  
**File Signatures (Magic Numbers) Directory**  
**Image Formats**  

| Format | Signature (Hex) | Signature (ASCII) | Description |
| ------ | ----------------------------------- | ----------------- | -------------------------- |
| JPEG | FF D8 FF | ÿØÿ | JPEG image |
| PNG | 89 50 4E 47 0D 0A 1A 0A | .PNG.... | PNG image |
| GIF | 47 49 46 38 | GIF8 | GIF image |
| BMP | 42 4D | BM | Bitmap image |
| TIFF | 49 49 2A 00 | II*. | TIFF image (little-endian) |
| TIFF | 4D 4D 00 2A | MM.* | TIFF image (big-endian) |
| WebP | 52 49 46 46 ?? ?? ?? ?? 57 45 42 50 | RIFF....WEBP | WebP image |
| ICO | 00 00 01 00 | .... | Icon file |
  
**Document Formats**  

| Format | Signature (Hex) | Signature (ASCII) | Description |
| ---------- | ----------------------- | ----------------- | ------------------------ |
| PDF | 25 50 44 46 | %PDF | PDF document |
| DOC | D0 CF 11 E0 A1 B1 1A E1 | ÐÏ..¡±.á | Microsoft Word document |
| DOCX | 50 4B 03 04 | PK.. | Office Open XML document |
| RTF | 7B 5C 72 74 66 31 | {\\rtf1 | Rich Text Format |
| PostScript | 25 21 50 53 | %!PS | PostScript file |
  
**Archive Formats**  

| Format | Signature (Hex)      | Signature (ASCII) | Description       |
| ------ | -------------------- | ----------------- | ----------------- |
| ZIP    | 50 4B 03 04          | PK..              | ZIP archive       |
| ZIP    | 50 4B 05 06          | PK..              | Empty ZIP archive |
| RAR    | 52 61 72 21 1A 07 00 | Rar!...           | RAR archive       |
| 7Z     | 37 7A BC AF 27 1C    | 7z¼¯'..           | 7-Zip archive     |
| TAR    | 75 73 74 61 72       | ustar             | TAR archive       |
| GZIP   | 1F 8B                | ..                | GZIP compressed   |
  
**Executable Formats**  

| Format | Signature (Hex) | Signature (ASCII) | Description           |
| ------ | --------------- | ----------------- | --------------------- |
| PE     | 4D 5A           | MZ                | Windows PE executable |
| ELF    | 7F 45 4C 46     | .ELF              | Linux ELF executable  |
| Mach-O | FE ED FA CE     | þíúÎ              | macOS Mach-O (32-bit) |
| Mach-O | FE ED FA CF     | þíúÏ              | macOS Mach-O (64-bit) |
| Java   | CA FE BA BE     | ÊþºÞ              | Java class file       |
  
**Media Formats**  

| Format | Signature (Hex) | Signature (ASCII) | Description |
| ------ | ----------------------------------- | ----------------- | ----------------------- |
| MP3 | 49 44 33 | ID3 | MP3 audio with ID3 tag |
| MP3 | FF FB | ÿû | MP3 audio without ID3 |
| WAV | 52 49 46 46 ?? ?? ?? ?? 57 41 56 45 | RIFF....WAVE | WAV audio |
| AVI | 52 49 46 46 ?? ?? ?? ?? 41 56 49 20 | RIFF....AVI | AVI video |
| MP4 | 66 74 79 70 | ftyp | MP4 video (at offset 4) |
| OGG | 4F 67 67 53 | OggS | Ogg media file |
  
  
**Character Encoding Reference Tables**  
**ASCII Control Characters (0-31)**  

| Dec | Hex | Char | Name            | Description        |
| --- | --- | ---- | --------------- | ------------------ |
| 0   | 00  | NUL  | Null            | String terminator  |
| 7   | 07  | BEL  | Bell            | Audio alert        |
| 8   | 08  | BS   | Backspace       | Move cursor back   |
| 9   | 09  | HT   | Tab             | Horizontal tab     |
| 10  | 0A  | LF   | Line Feed       | New line (Unix)    |
| 13  | 0D  | CR   | Carriage Return | New line (Mac)     |
| 26  | 1A  | SUB  | Substitute      | End of file marker |
| 27  | 1B  | ESC  | Escape          | Escape character   |
  
**ASCII Printable Characters (32-126)**  

| Range | Characters | Description |
| ------- | --------------------------------------------------- | ----------------------- |
| 32-47 | Space ! " # $ % & ' ( ) * + , - . / | Symbols and punctuation |
| 48-57 | 0 1 2 3 4 5 6 7 8 9 | Numeric digits |
| 58-64 | : ; < = > ? @ | Symbols and punctuation |
| 65-90 | A B C D E F G H I J K L M N O P Q R S T U V W X Y Z | Uppercase letters |
| 91-96 | [ \\ ] ^ _ ` | Symbols and punctuation |
| 97-122 | a b c d e f g h i j k l m n o p q r s t u v w x y z | Lowercase letters |
| 123-126 | { \| } ~ | Symbols and punctuation |
  
**UTF-8 Encoding Patterns**  

| Unicode Range | UTF-8 Pattern | Bytes | Description |
| ------------------ | ----------------------------------- | ----- | ------------------------------ |
| U+0000 - U+007F | 0xxxxxxx | 1 | ASCII characters |
| U+0080 - U+07FF | 110xxxxx 10xxxxxx | 2 | Latin extended, Cyrillic, etc. |
| U+0800 - U+FFFF | 1110xxxx 10xxxxxx 10xxxxxx | 3 | Most common characters |
| U+10000 - U+10FFFF | 11110xxx 10xxxxxx 10xxxxxx 10xxxxxx | 4 | Supplementary planes |
  
  
**Regular Expression Syntax Quick Reference**  
**Basic Metacharacters**  

| Symbol | Meaning | Example |
| ------ | ----------------------------------- | -------------------------------- |
| . | Any single character except newline | a.b matches "aab", "abb", "acb" |
| * | Zero or more of preceding | ab* matches "a", "ab", "abb" |
| + | One or more of preceding | ab+ matches "ab", "abb", not "a" |
| ? | Zero or one of preceding | ab? matches "a", "ab" |
| ^ | Start of line | ^abc matches "abc" at line start |
| $ | End of line | abc$ matches "abc" at line end |
| \| | Alternation (OR) | cat\|dog matches "cat" or "dog" |
| \\ | Escape character | \\. matches literal dot |
  
**Character Classes**  

| Class | Meaning            | Equivalent          |
| ----- | ------------------ | ------------------- |
| \\d   | Digit              | [0-9]               |
| \\D   | Non-digit          | [^0-9]              |
| \\w   | Word character     | [a-zA-Z0-9_]        |
| \\W   | Non-word character | [^a-zA-Z0-9_]       |
| \\s   | Whitespace         | [ \\t\\n\\r\\f\\v]  |
| \\S   | Non-whitespace     | [^ \\t\\n\\r\\f\\v] |
| \\b   | Word boundary      |                     |
| \\B   | Non-word boundary  |                     |
  
**Quantifiers**  

| Quantifier | Meaning | Example |
| ---------- | --------------------------- | ---------------------------------- |
| {n} | Exactly n occurrences | a{3} matches "aaa" |
| {n,} | n or more occurrences | a{3,} matches "aaa", "aaaa", etc. |
| {n,m} | Between n and m occurrences | a{2,4} matches "aa", "aaa", "aaaa" |
| *? | Non-greedy zero or more | .*? matches shortest possible |
| +? | Non-greedy one or more | .+? matches shortest possible |
| ?? | Non-greedy zero or one | .?? matches shortest possible |
  
**Common OSINT Regular Expressions**  

| Purpose | Pattern | Description |
| ------------- | ------------------------------------------------------- | ------------------------- |
| Email | \\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Z\|a-z]{2,}\\b | Basic email validation |
| IPv4 | \\b(?:[0-9]{1,3}\\.){3}[0-9]{1,3}\\b | IPv4 address |
| IPv6 | ([0-9a-fA-F]{1,4}:){7}[0-9a-fA-F]{1,4} | IPv6 address (simplified) |
| URL | https?://[^\\s]+ | Basic URL matching |
| Phone (US) | \\b\\d{3}-\\d{3}-\\d{4}\\b | US phone format |
| Credit Card | \\b\\d{4}[\\s-]?\\d{4}[\\s-]?\\d{4}[\\s-]?\\d{4}\\b
 | Credit card number |
| SSN | \\b\\d{3}-\\d{2}-\\d{4}\\b | US Social Security Number |
| MAC Address | ([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2}) | MAC address |
| Bitcoin | [13][a-km-zA-HJ-NP-Z1-9]{25,34} | Bitcoin address |
| Hash (MD5) | \\b[a-f0-9]{32}\\b | MD5 hash |
| Hash (SHA1) | \\b[a-f0-9]{40}\\b | SHA1 hash |
| Hash (SHA256) | \\b[a-f0-9]{64}\\b | SHA256 hash |
  
  
Network Protocol Header Structures  
IPv4 Header  
```
 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|Version|  IHL  |Type of Service|          Total Length         |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|         Identification        |Flags|      Fragment Offset    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|  Time to Live |    Protocol   |         Header Checksum       |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                       Source Address                          |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    Destination Address                        |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    Options                    |    Padding    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```
  
TCP Header  
```
 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|          Source Port          |       Destination Port        |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                        Sequence Number                        |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    Acknowledgment Number                      |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|  Data |           |U|A|P|R|S|F|                               |
| Offset| Reserved  |R|C|S|S|Y|I|            Window             |
|       |           |G|K|H|T|N|N|                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|           Checksum            |         Urgent Pointer        |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    Options                    |    Padding    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                             data                              |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```
  
HTTP Request Format  
```
Method Request-URI HTTP-Version CRLF
*(( general-header | request-header | entity-header ) CRLF)
CRLF
[ message-body ]
Example:
GET /index.html HTTP/1.1
Host: www.example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
Accept: text/html,application/xhtml+xml,application/xml
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Connection: keep-alive

```
  
DNS Message Format  
```
 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                              ID                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|QR|   Opcode  |AA|TC|RD|RA|   Z    |   RCODE   |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    QDCOUNT                    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    ANCOUNT                    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    NSCOUNT                    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|                    ARCOUNT                    |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+

```
