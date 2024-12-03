
# Caesar Cipher Encryption and Decryption

This Python script implements the **Caesar Cipher**, a basic encryption technique that shifts letters of the alphabet by a specified number. It can both **encrypt** and **decrypt** messages using a given shift value.

## Overview

The script provides two main functions:
1. **Encrypting a message**: It shifts the letters of the input message by a specified number (shift value).
2. **Decrypting a message**: It reverses the encryption process using the same shift value.

## Features

- Encrypt and decrypt messages using the Caesar Cipher.
- Handles both uppercase and lowercase letters.
- Non-alphabet characters (spaces, punctuation, etc.) are preserved.
- The shift value is customizable (1-25).

## How It Works

The Caesar Cipher works by shifting each letter of the plaintext by a fixed number of positions down or up the alphabet. For example, with a shift of 3:
- 'A' becomes 'D'
- 'B' becomes 'E'
- and so on.

To decrypt, the process is reversed by shifting in the opposite direction.

### Example:

- **Encryption**:  
  - Plaintext: `Hello World`  
  - Shift: 3  
  - Encrypted: `Khoor Zruog`

- **Decryption**:  
  - Ciphertext: `Khoor Zruog`  
  - Shift: 3  
  - Decrypted: `Hello World`


## Usage

1. When the script runs, you will be prompted to choose whether you want to **encrypt** or **decrypt** a message. 
2. You will then need to enter the message you want to process.
3. Finally, you'll be asked to input the **shift value** (an integer between 1 and 25).

Example Interaction:

```
Caesar Cipher Encryption/Decryption
Do you want to (E)ncrypt or (D)ecrypt a message? e
Enter your message: Hello World
Enter the shift value (1-25): 3
Encrypted message: Khoor Zruog
```

For decryption:

```
Caesar Cipher Encryption/Decryption
Do you want to (E)ncrypt or (D)ecrypt a message? d
Enter your message: Khoor Zruog
Enter the shift value (1-25): 3
Decrypted message: Hello World
```

## Code Explanation

### Functions

1. **`encrypt_message(plaintext, shift)`**:
   - Encrypts the given plaintext using the Caesar Cipher with the specified shift.
   - Handles both uppercase and lowercase letters and leaves non-alphabet characters unchanged.

2. **`decrypt_message(encrypted_text, shift)`**:
   - Decrypts the given encrypted text by reversing the shift used during encryption.
   - Preserves non-alphabet characters.

3. **`main()`**:
   - The main function that drives the script, prompting the user to select the action (encrypt or decrypt), input the message, and provide the shift value.
   - Calls the `encrypt_message` or `decrypt_message` functions based on the user's input and displays the result.


