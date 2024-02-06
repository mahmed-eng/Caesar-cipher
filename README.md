# Caesar Cipher Web Implementation

## Introduction:
The provided program is a web-based implementation of the Caesar Cipher, a simple substitution cipher technique. It allows users to encrypt and decrypt messages using a specified shift value. The program uses HTML for the structure, CSS for styling, and JavaScript for the logic behind the encryption and decryption processes.

## Overview:
The Caesar Cipher is a basic encryption algorithm where each letter in the plaintext is shifted a certain number of places down or up the alphabet. In this implementation, the user can input a plain text and a shift value, and the program will generate the corresponding encrypted or decrypted text.

## Time Complexity:
The time complexity of both the encryption and decryption functions is O(n), where n is the length of the input text. This is because the algorithm iterates through each character of the input text exactly once, performing constant-time operations for each character.

## Best for:
This program is suitable for educational purposes, introductory cryptography exploration, or simple cases where a lightweight encryption method is needed. It's best suited for scenarios where security requirements are not high, as the Caesar Cipher is vulnerable to brute-force attacks due to its limited number of possible keys.

## Not a Good Practice:
The Caesar Cipher is considered insecure for real-world applications due to its susceptibility to brute-force attacks. It has a fixed and small number of possible keys (26 in the case of the English alphabet), making it easy for an attacker to try all possible combinations.

## Steps of Algorithm:

### User Input:
- Accepts the plain text and shift value from the user through HTML input elements.

### Encryption Function (`encrypt()`):
- Converts the plain text to uppercase for consistency.
- Iterates through each character of the plain text.
- Checks if the character is an uppercase letter.
- Applies the Caesar Cipher formula to encrypt the letter.
- Leaves non-alphabetic characters unchanged.
- Displays the encrypted text as the result.

### Decryption Function (`decrypt()`):
- Converts the cipher text to uppercase for consistency.
- Iterates through each character of the cipher text.
- Checks if the character is an uppercase letter.
- Applies the reverse Caesar Cipher formula to decrypt the letter.
- Leaves non-alphabetic characters unchanged.
- Displays the decrypted text as the result.

## Note: 
The decryption function uses the modulo operation to handle cases where the shift goes beyond the bounds of the alphabet, ensuring a valid output.
