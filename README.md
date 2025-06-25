# Custom File Encryption & Decryption Tool

A secure file encryption/decryption utility built with Python, using modern cryptographic standards (AES or RSA). This tool allows users to protect sensitive files with custom passkeys and ensure safe transmission or storage using industry-recommended encryption algorithms.

## Overview

This tool provides a command-line interface for encrypting and decrypting files using symmetric (AES) or asymmetric (RSA) encryption methods. Built with the `cryptography` or `PyCryptodome` library, it handles key management, padding, encoding, and secure file handling.

## Features

- **AES Encryption (Symmetric)**
  - File encrypted with a secret key (user-defined or generated)
  - CBC mode with PKCS7 padding and IV handling
  - Secure key and IV generation

- **RSA Encryption (Asymmetric)**
  - Public/private key pair encryption
  - Encrypt files with public key and decrypt with private key
  - Optional key generation and saving to `.pem`

- **File I/O Handling**
  - Supports binary and text files
  - Preserves file extensions and metadata
  - Output naming with `.enc` or `.dec`

- **Security Enhancements**
  - Keys stored outside code
  - Optional password hashing for added key security
  - Uses `os.urandom` or `secrets` for entropy

## Tech Stack

| Component     | Technology                 |
|---------------|-----------------------------|
| Language      | Python 3.x                  |
| Encryption    | AES-256 / RSA-2048          |
| Library       | `cryptography` / `pycryptodome` |
| Interface     | CLI                         |




