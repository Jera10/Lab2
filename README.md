# Cryptography Tool

A simple Python tool for generating encryption keys, encrypting files, and decrypting files using symmetric key encryption with the Fernet module from the `cryptography` library.

## Features

- **Key Generation**: Generate and save a symmetric encryption key.
- **File Encryption**: Encrypt files using the generated key.
- **File Decryption**: Decrypt encrypted files back to their original state.
- **Command-Line Interface**: Easily interact with the tool using command-line arguments.

### Interaction
Generate a key by running the command; python generate_key.py
Use the crypto_tool.py script to encrypt a file using the generated key.
    - python crypto_tool.py encrypt -f <filename> -k <keyfile>
        Reads the content of secret.txt.
        Encrypts the content using the key from key.key.
        Creates a new file named secret.txt.encrypted containing the encrypted data.
        Note: The original secret.txt file remains unchanged.
Use the crypto_tool.py script to decrypt an encrypted file back to its original form.
    - python crypto_tool.py decrypt -f <encrypted_filename> -k <keyfile>
        Reads the content of secret.txt.encrypted.
        Decrypts the content using the key from key.key.
        Restores the original file secret.txt with the decrypted data.
        Note: The encrypted file secret.txt.encrypted remains unchanged.