```C
// Synopsis
#include <arpa/inet.h>
uint32_t htonl(uint32_t hostlong);
uint16_t htons(uint16_t hostshort);
uint32_t ntohl(uint32_t netlong);
uint16_t ntohs(uint16_t netshort);
```
- `Network Byte Order` is always Big Endian (most significant byte on the left most);  
  `Host Byte Order` can either be Big Endian or Small Endian, depending on specific machines.  
- when receive or send a number through network, we should convert it to host/network byte order.  
- In C, this is done by using `htonl()`, `htons()`, `ntohl()`, `ntohs()` functions.  
