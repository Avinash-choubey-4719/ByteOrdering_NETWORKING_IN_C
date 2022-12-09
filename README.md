# ByteOrdering_NETWORKING_IN_C

Unfortunately, not all computers store the bytes that comprise a multibyte value in the same order. Consider a 16-bit internet that is made up of 2 bytes.
There are two ways to store this value.

Little Endian − In this scheme, low-order byte is stored on the starting address (A) and high-order byte is stored on the next address (A + 1).

Big Endian − In this scheme, high-order byte is stored on the starting address (A) and low-order byte is stored on the next address (A + 1).

To allow machines with different byte order conventions communicate with each other, the Internet protocols specify a canonical byte order convention for 
data transmitted over the network. This is known as Network Byte Order.

While establishing an Internet socket connection, you must make sure that the data in the sin_port and sin_addr members of the sockaddr_in structure are 
represented in Network Byte Order.
