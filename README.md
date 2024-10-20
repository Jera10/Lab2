# Cryptography Tool

A simple Python tool for generating encryption keys, encrypting files, and decrypting files using symmetric key encryption with the Fernet module from the `cryptography` library.

## Features & Usage

- **Key Generation**: Generate and save a symmetric encryption key.
    - *Generate a key by running the command; python generate_key.py*
- **File Encryption**: Encrypt files using the generated key.
    - *Use the crypto_tool.py script to encrypt a file using the generated key.*
    - *python crypto_tool.py encrypt -f <filename> -k <keyfile>*
- **File Decryption**: Decrypt encrypted files back to their original state.
    - *Use the crypto_tool.py script to decrypt an encrypted file back to its original form.*
    - *python crypto_tool.py decrypt -f <encrypted_filename> -k <keyfile>*
- **Command-Line Interface**: Easily interact with the tool using command-line arguments.
