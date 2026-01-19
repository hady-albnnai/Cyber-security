# Bandit Level 11 → Level 12

## Objective
Decode a text file encoded with the ROT13 cipher.

## Concept
ROT13 is a simple letter‑substitution cipher that replaces each letter with the letter 13 positions ahead in the alphabet. It is its own inverse: applying ROT13 twice returns the original text.

## Tools & Commands Introduced
- tr – translate or delete characters
- Pipeline | – connect the output of one command to the input of another

## Approach
1. Read the encoded file.
2. Apply the ROT13 substitution using tr with the appropriate character mapping.

## Example Command
cat encoded.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

## Key Takeaway
- ROT13 is often used to obfuscate text without real security.
- The tr command is useful for simple character‑by‑character transformations.
