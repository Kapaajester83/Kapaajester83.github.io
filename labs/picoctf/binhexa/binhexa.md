
https://play.picoctf.org/practice/challenge/404?page=2

Description
How well can you perfom basic binary operations? Start searching for the flag here 

nc titan.picoctf.net 61002

CLI

kappa@kappa-Aspire-Z5600:~$ nc titan.picoctf.net 61002

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 00001010
Binary Number 2: 11010110


Question 1/6:
Operation 1: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 1101011
Correct!

Question 2/6:
Operation 2: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 0
Incorrect. Try again
Enter the binary result: 00000010
Correct!

Question 3/6:
Operation 3: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 10100
Correct!

Question 4/6:
Operation 4: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 100001011100
Correct!

Question 5/6:
Operation 5: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11100000
Correct!

Question 6/6:
Operation 6: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11011110
Correct!

Enter the results of the last operation in hexadecimal: DE

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6862762d}


https://miniwebtool.com/bitwise-calculator/bit-shift/
https://www.rapidtables.com/calc/math/binary-calculator.html
https://www.rapidtables.com/convert/number/binary-to-hex.html


<< (Logical left shift)
>> (Logical right shift)
| (OR)
& (AND)
* (Multiplication)
+ (Addition)
