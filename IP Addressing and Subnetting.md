# IP Addressing and Subnetting

IPv4 addresses occupy a range from 0.0.0.0 to 255.255.255.255
There are 32 bits total in these IP addresses with each octet (seperated by a .) representing 8 bits.

Since there are only 2 possible values in Binary, 1 & 0, and 32 bits total in an IP address, this means 2^32 = 4,294,967,296 is the total number of available IP addresses in the IPv4 address space.

## Powers of 2 Method for Decimal -> Binary Conversion
 ### 192.168.1.1 (Example IP)

 To convert the above the IP address to Binary, you would start with the first octet which is 192.
 
 1. Start with the largest power of 2 that is equal to or less than your number, in this case 192, and work your way down.

 2. Starting with 192 from the address above, what power of 2 is the largest power that is equal to or less than 192? The answer is 2^7 = 128. You cant use 2^8 because that equals 256 which we cannot use since the address space only goes to 255. 

 3. Subtract your largest power of 2 value (128) from your IP octet value, 192. 192 - 128 = 64 = Binary Digit of 1.

 4. Using this method, go down the octet list and subtract the highest power of 2 from the REMAINDER each time and determine the binary digit. If you CAN subtract from it without getting a negative number, designate the binary digit 1, if you CANNOT, binary digit = 0.

![alt text](conversion.jpg)
