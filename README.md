# azureSite2SiteVpnSettings
Collection of Site to Site VPN Settings. The following configurations were successfully tested with encryption and integrity selections incrementally increased until VPN connection failed.  

## Palo Alto
IKE Phase 1
- Encryption - AES256
- Integrity - SHA256
- DH Group - DHGroup14

IKE Phase 2 (IPsec)
- IPsec Encryption - AES256
- IPsec Integrity - SHA1
- PFS Group - PFS2

IPsec SA lifetime in Kilobytes - 1024000000

IPsec SA lifetime in seconds - 28800

Use policy based traffic selector - Disabled

DPD timeout in seconds- 45

Connection Mode - Default

Use custom traffic selectors - Disabled

IKE Protocol - IKEv2

## Cisco Meraki
IKE Phase 1
Encryption - AES256
Integrity - SHA256
DH Group - DHGroup2

IKE Phase 2 (IPsec)
IPsec Encryption - AES256
IPsec Integrity - SHA256
PFS Group - 2

IPsec SA lifetime in Kilobytes
102400000

IPsec SA lifetime in seconds
28800

Use policy based traffic selector
Disabled

DPD timeout in seconds
45

Connection Mode
Default

Use custom traffic selectors
Disabled

IKE Protocol
IKEv2
