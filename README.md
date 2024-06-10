# File Compression and Encryption

## Overview
This project focuses on the encryption of compressed files to prevent unauthorized access. The data is first compressed using a code length and the index of a master array, then saved as an encrypted file. This encrypted file has a newer bit pattern and a smaller size, demonstrating that the data has been compressed effectively. The same file can then be decompressed using the same master array to retrieve the original data, verifying the success of the compression.

## Objectives
- Remove ASCII code-based data redundancy from the source file.
- Compress the file while simultaneously encoding it with a custom algorithm to encrypt the data.

## Features
- **Compression**: Reduces the file size by eliminating redundancies using a custom algorithm.
- **Encryption**: Protects the compressed data from unauthorized access.
- **Decompression**: Retrieves the original data from the compressed and encrypted file.
- **Master Array**: Utilized for compression and decompression, containing unique characters and their respective indices.
- **Find Index**: Locates the index of characters in the master array.
- **Unique Array**: Maintains a list of unique characters for efficient compression.

## Details
- The project addresses the 8-bit extended ASCII character set, handling a maximum of 256 characters.
- Eight different algorithmic procedures are implemented to manage the character set effectively.

## Functions
1. **Compression**: Compresses the input data by encoding it using the master array.
2. **Decompression**: Decompresses the encrypted file to retrieve the original data.
3. **Master Array**: Creates an array of unique characters for the compression process.
4. **Find Index**: Finds the index of a character in the master array.
5. **Unique Array**: Generates an array of unique characters from the input data.

## How It Works
1. **Compression and Encryption**:
    - The input data is analyzed, and redundant ASCII codes are removed.
    - Data is compressed using the length of the code and the index in the master array.
    - The compressed data is then encrypted, resulting in a file with a new bit pattern and reduced size.

2. **Decompression**:
    - The encrypted file is decrypted using the master array.
    - The original data is obtained, confirming the success of the compression and encryption process.

## Usage
1. **Prerequisites**:
    - Ensure you have a compatible environment to run the code (e.g., Python, C, etc.).
    - Basic understanding of file I/O operations and encryption algorithms.

2. **Running the Code**:
    - Implement the provided functions in your codebase.
    - Use the functions to compress, encrypt, decompress, and verify your data.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License.
