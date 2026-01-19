# Bandit Level 12 → Level 13

## Objective
Recover a password from a file that has been compressed and archived multiple times with different methods.

## Concepts Learned
- Recognizing file types with the file command
- Using xxd to revert a hexdump back to binary
- Decompressing various formats: gzip ,bzip2, tar
- Iterative problem‑solving: repeatedly decompressing until the plaintext is found

## Tools & Commands Introduced
- xxd – create or reverse a hex dump
- file – determine file type
- gzip / bzip2 – compress/decompress files
- tar – archive utility

## Approach
1. Convert the provided hexdump back to a binary file.
2. Identify the file type using file.
3. Apply the appropriate decompression or extraction command based on the identified type.
4. Repeat steps 2–3 until a human‑readable password file is obtained.

## Example Workflow (Generic)
xxd -r hexdump.txt > binary
file binary
# Based on output, decompress with gzip, bzip2, tar, etc.

## Key Takeaway
- Many file types have distinct "magic bytes" that file uses for identification.
- Compression and archiving can be layered; patience and methodical checking are essential.
- Working in a temporary directory (`/tmp`) keeps the home directory clean.
