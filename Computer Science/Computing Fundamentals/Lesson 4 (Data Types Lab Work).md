==Notable definitions:
4 bits = Nibble
8 bits = Byte
16 bits = Word
32 bits = Double word
64 bits = QuadWord==

In this lesson you practiced converting base 10 to base 2. and vice versa (normal numbers to binary)
If a number has a subscript (e.g. 11001001$_2$)

==Base 2 to base 10==
1x2$^10$+1x2$^9$+1x2$^8$+1x2$^7$ + 0x2$^6$ +1x2$^5$ +1x2$^4$ +1x2$^3$ +1x2$^2$ +1x2$^1$+1x2$^0$
0+0+4+0+16+32+64+0+256+0+1024
EXERCISE
a) 14
b)199
c)10
d)75
e)830
f)41
g)232
h)1396

==Base 10 to base 2==
To convert from base 2 to base 10, you need to divide the number you want to turn into binary by 2 until you cannot divide without getting decimals, and write down the remainder each time.
Examples:

157 (ODD) can't be divided by 2. So you take away one and then divide it by 2. That represents a 1 in binary.

157 / 2 (take away 1) = 78,                     remainder 1.
78 / 2 (no need to take away 1) = 39, remainder 0.
39 / 2 (-1) = 19                                            remainder 1.
19 / 2 (-1) = 9                                              remainder 1.
9 / 2 (-1) = 4                                                remainder 1.
4 / 2 = 2                                                        remainder 0.
2 / 2 = 1                                                        remainder 0.
1 / 2 (-1) = 0                                                remainder 1.
 
157 = 10011101 (write it from left to right, bottom to top)

EXERCISE
a) 302 = 100101110
b)1157=10010000101
c)1414=10110000110
d) 54=110110
e)1851=11100111011
f)6501=1100101100101
g)8=1000
h)76=1001100

76/2=38(0)
38/2=19(0)
19/2=9(1)
9/2=4(1)
4/2=2(0)
2/2=1(0)
1/2=0(1)

6501/2=3250(1)
3250/2=1625(0)
1625/2=812(1)
812/2=406(0)
406/2=203(0)
203/2=101(1)
101/2=50(1)
50/2=25(0)
25/2=12(1)
12/2=6(0)
6/2=3(0)
3/2=1(1)
1/2=0(1)

1851/2=925(1)
925/2=462(1)
462/2=231(0)
231/2=115(1)
115/2=57(1)
57/2=28(1)
28/2=14(0)
14/2=7(0)
7/2=3(1)
3/2=1(1)
1/2=0(1)

54/2= 27(0)
27/2=13(1)
13/2=6(1)
6/2=3(0)
3/2=1(1)
1/2=0(1)

1414/2=707(0)
707/2=353(1)
353/2=176(1)
176/2=88(0)
88/2=44(0)
44/2=22(0)
22/2=11(0)
11/2=5(1)
5/2=2(1)
2/2=1(0)
1/2=0(1)

==ASCII code==
You just folbinary to low a table for this. If you feel masochistic I GUESS you could try memorizing it.

EXERCISE
a)HELLO WORLD! = 01001000 01000101 01001100 01001100 01001111 00100000 01010111 01001111 01010010 01001100 01000100 00100001

b)See you. =  01010011 01100101 01100101 00100000 01111001 01101111 01110101 00101110

==Booleans (Truth tables)==

-# (or ¬) means NOT (NOT A)
-^ means AND (A AND B)
-V means OR (A OR B)
-⊕ means XOR (A XOR B,  = 1 when only one of A or B is 1)
-≡ means EQ (A EQ B, A XNOR B, only outputs 1 when both inputs are equal (0 or 1))

EXERCISE
a) A V B 

| A   | B   | Q   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 1   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 1   | 1   |
b)¬A ^ (B V C)

