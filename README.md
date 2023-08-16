# -AES-encryption-and-decryption.
Verilog

## Introduction 
This project takes a word of 128 bits and  keys with lengths of 128, 192, and 256 bits.Then it makes an Encryption to this word by using the keys and then it make a decryption to the Encrypted word by using "The AES algorithm.".

## The Explanation of The Project
The AES algorithm is steps. if you made it you will make the Encryption and Decryption .
There is a variable  we must use  called "Nr" it mean "Number of Round" :
  - if key is 128 bits  Nr=10 Round
  - if key is 192 bits  Nr=12 Round
  - if key is 265 bits  Nr=14 Round
### Steps of Encryption :
```
1- AddRoundKey
2- for loop from 1 to Nr-1
  1- SubBytes() 
  2-ShiftRows() 
  3-MixColumns() 
  4-AddRoundKey()
3-SubBytes()
4-ShiftRows()
5-AddRoundKey()
```
These are the steps to make Encryption .If you want to know the details and  what are this functions and how it works I will but some links that Explains all of them  in the end of the Exeplanation
###  Steps of Decryption :
It looks like the steps of encryption but there are some differences
```
1-AddRoundKey() 
2-for loop from  Nr-1 to -1 
  1-InvShiftRows() 
  2-InvSubBytes() 
  3-AddRoundKey()
  4-InvMixColumns()
3-InvShiftRows()
4-InvSubBytes()
5-AddRoundKey()
```
## Some Useful Links To Explain The AES Algorithm
-<a href="https://classroom.google.com/u/0/c/NTQyNTUyODA3MjA2">Document</a>

-<a href="https://youtu.be/O4xNJsjtN6E">Video1</a>

-<a href="https://youtu.be/Lt0nkqccEhc?t=3">Video2</a>

-<a href="https://youtu.be/0ryUIpyif54?t=1">Video3</a>

-<a href="https://youtu.be/Tx_37dF03ig">ShiftRow,MixColumns and SubBuytes Video</a>

