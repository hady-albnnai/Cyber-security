# Bandit Level 9 → Level 10

## Objective
Extract human-readable strings from a binary or mixed-format file using pattern matching.

## Concepts Learned
- Using strings to extract printable characters from binary data
- Filtering output with grep using a repeated-character pattern
- Recognizing obfuscated data in non-text files

## Tools & Commands Introduced
- strings – extract printable character sequences from a file
- grep – filter lines containing a specific pattern
- Pipeline (|) to chain text-processing tools

## Approach
1. Use strings to retrieve all readable text from the file.
2. Pipe the result to grep and search for lines containing a repeated delimiter (==).
3. Isolate the password from the matched line.

## Example Command
strings data.bin | grep "==="


## Key Takeaway
- Binary files often contain embedded text that can be revealed with strings.
- Pattern matching (grep) is useful for isolating relevant sections in noisy output.
