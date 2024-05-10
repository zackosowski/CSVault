Computer processors consist of a bunch of tiny switches called "transistors".
* these transistors can either be ON or OFF, just like a light switch
* on and off positions are referred to as 1 and 0
* electrical signals flip the switches to 1 and 0
* the binary number system allows us to give meaning to 1s and 0s
* every computer uses these 1s and 0s to execute every task
* every file on your computer is just a series of 1s and 0s

A single 1 or 0 is the smallest unit of data in a computer- a "**bit**"
* a group of eight bits is called a **byte**
* 1024 bytes is called a **kilobyte**
* 1024 kilobytes is called a **megabyte**
* 1024 megabytes is called a **gigabyte**
* 1024 gigabytes is called a **terabyte**
* 1024 terabytes is called a **petabyte**

#### Decimal System
<hr>

Numeral systems are writing systems for expressing numbers. Everyday, you use a base 10 number system called the decimal system. "Deci" meaning 10. Base 10 because we have 10 fingers. Here is an example of how we represent the number 125 in the decimal system:

| 100 | 10  | 1   |
| --- | --- | --- |
| 1   | 2   | 5   |

* In the human world (decimal) we use powers of 10 for place values
	* 10<sup>0</sup> = 1, 10<sup>1</sup> = 10, 10<sup>2</sup> = 100, 10<sup>3</sup> = 1000, etc.
* The rightmost column is the 1s column
* The middle, the 10s
* the leftmost, the 100s
* Thus we have (100 x 1) + (10 x 2) + (1 x 3) = (100 + 20 + 5) = 125

#### Binary System
<hr>

Computer systems operate in a base 2 system called Binary. Base 2 because transistors have 2 positions, 1 or 0. 

Here is how we represent the the number 125 in a byte of binary:

| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 0   | 1   | 1   | 1   | 1   | 1   | 0   | 1   |

**= 01111101**

-   In the computer world (binary) we use powers of 2 for place values
    - 2<sup>0</sup> = 1, 2<sup>1</sup> = 2, 2<sup>2</sup> = 4, 2<sup>3</sup> = 8, etc.
- The rightmost column is the 1s place
- the next column is the 2s, then 4s, then 8s, and so on.
* Thus we have 
	* (128 x 0) + (64 x 1) + (32 x 1) + (16x 1) + (8 x 1)+ (4 x 1) + (2 x 0) + (1 x 1) =
	* (0 + 64 + 32 + 16 + 8 + 4 + 0 + 1) = 125

<hr>

Even though computers only use binary, they can count as high as we can, they just do it with a small vocabulary, 1 and 0.  For numbers that are too large to represent with one byte of data, simply add more bytes separated by a space.
* 421 = 00000001 10100101

Everything that computers process is done by sending power to transistors, changing their states to OFF (0) or ON (1).

<hr>

**<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">QUESTIONS</span>**

<details>
	<summary>What is the largest number you can represent with a byte of binary?</summary>
		<p style="font-style: italic">11111111 = 255</p>
</details>


<details>
	<summary>How many bytes are needed to represent the decimal number 100,000 in binary?</summary>
		<p style="font-style: italic">00000001 10000110 10100000 = 3 bytes</p>
</details>


<details>
	<summary>It is possible to tell if a binary number is even or odd very easily. How?</summary>
		<p style="font-style: italic">If the rightmost digit is a one, the number is odd. If its a zero, its even.</p>
</details>

<hr>

<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

Your windows operating system has a little program that lets you explore all Unicode characters. Open the program and poke around those character.

Top open the Character Map program...
* Press the Windows Key
* Search for "Character Map" and open
* Select characters and copy them
* Paste them anywhere!