# [Cryptography](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

- The first recorded type of encryption was the ceaser cipher! simply shifting the alphabet a certain number over and replacing the characters with those in place.

- to decrypt a ceaser chiper we simple shift all the letters back by the same ammount they were shifted. 

If you didnt know the 'key' or how far the message had been shifted you have three main techniques crack the code. 

### frequency analysis
- Basically knowing which letters apear the most often in normal text, we can assume a given character is that letter, and work backwards from there. 

### Known Plaintext
- We we already know some part of the unencrypted message, we can work backwards from there to solve the encrypted part. This is how the enigma code was cracked by Alan Turing. 
	( Some day I will program an Enigma machine, but as you can imagine they are quite complicated )
	
### Brute Force
- There are only so many possible shifts, Just try them all until you get a result that makes sense. 

