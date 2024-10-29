# Simple Text Encryptor

The **Simple Text Encryptor** is a Java program that encrypts or decrypts text data using a **Linear Feedback Shift Register (LFSR)** method. This tool operates on **text input only**, rather than files, making it ideal for quick encryption or decryption of short strings or hexadecimal data.

## Overview

This program demonstrates a basic encryption technique using bitwise manipulation. It uses LFSR to encrypt or decrypt text input, displaying the result in hexadecimal format.

## How It Works

1. **Data Input**: You’ll be prompted to enter the text you wish to encrypt or decrypt. Input can be:
   - **Plain text** (e.g., `HelloWorld`)
   - **Hexadecimal format** (e.g., `\x4F\x57\x41`)

2. **Initial Value**: Enter a hexadecimal value prefixed with `0x` (e.g., `0x4F574154`). This initializes the LFSR to start the encryption or decryption.

3. **Output**: The program outputs the encrypted or decrypted result in hexadecimal format.

## Example Usage

```
Insert Data: HelloWorld
Insert Initial Value: 0x4F574154
Output: \x93\xA4\xB1\xCE\x85\x8C\xBA\xB4\xDF\xC8
```

## Key Components

- **LFSR Encryption (`Crypt`)**: The core function that applies bitwise encryption based on the initial LFSR value and a fixed feedback polynomial.
- **Hexadecimal Handling (`hexStringToByteArray`)**: Processes hexadecimal strings to byte arrays for efficient manipulation.

## Limitations

- **Text Input Only**: This encryptor is designed to work with text input, not files. It processes plain text or hexadecimal strings but does not read from or write to files.
- **Basic Encryption**: Suitable for demonstration; not intended for securing highly sensitive data.
