# Memory Overview
Memory is **finite** - you can run out of memory slots to use.  Programs can only store/use free memory slots.

Memory is made up of **bits**.  Data is stored as a bit, and typically one memory slot can hold 8 bits (**1 byte**).
- Bits are in **binary** (ex. 00100101)
- Programs are in **base 2**, because at the very root there are 2 possibilities... either 0 or 1
- There are 256 potential data values for **1 byte** (2^8 = 256)

There are common 32 bit and 64 bit structures, which require multiple memory slots.  If a program needs to store something in multiple slots, it is stored in "back to back" slots.
- The most "significant" bytes are stored toward the left, and this is known as **endianess**

**Strings** are often mapped to numbers through **ASCII**.

**Pointers** allow you to point to data in other memory slots, by storing a memory address of another memory slot.
- This is helpful for finding and accessing memory quickly
