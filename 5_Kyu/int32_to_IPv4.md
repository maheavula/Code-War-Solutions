## Problem Statement 

Take the following IPv4 address: 128.32.10.1

This address has 4 octets where each octet is a single byte (or 8 bits).

1st octet 128 has the binary representation: 10000000
2nd octet 32 has the binary representation: 00100000
3rd octet 10 has the binary representation: 00001010
4th octet 1 has the binary representation: 00000001
So 128.32.10.1 == 10000000.00100000.00001010.00000001

Because the above IP address has 32 bits, we can represent it as the unsigned 32 bit number: 2149583361

Complete the function that takes an unsigned 32 bit number and returns a string representation of its IPv4 address.

Examples

2149583361 ==> "128.32.10.1"

32         ==> "0.0.0.32"

0          ==> "0.0.0.0"


## Solution

```python
# Provide your solution here.
def int32_to_ip(int32):
    bin_ip = bin(int32)[2:].zfill(32)
    bin_oct = bin_ip[:8] + "." + bin_ip[8:16] + "." + bin_ip[16:24] + "." + bin_ip[24:32]
    lst_bin = bin_oct.split(".")
    fin_bin = [str(int(i,2)) for i in lst_bin]
    return '.'.join(fin_bin)
