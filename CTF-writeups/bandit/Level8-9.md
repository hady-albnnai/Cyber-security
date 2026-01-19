# Bandit Level 8 → Level 9

## Objective
Identify the unique line in a file that appears exactly once.

## Concepts Learned
- Sorting data to group identical lines
- Using uniq to find duplicate or unique entries
- Piping commands (sort | uniq) for text processing

## Tools & Commands Introduced
- sort – arrange lines in order
- uniq -u – output only lines that are not repeated
- Pipeline (|) – connect output of one command to input of another

## Approach
1. Sort the file so identical lines become consecutive.
2. Pipe the sorted output to uniq -u to print the line that occurs only once.

## Example Command
sort filename | uniq -u

## Key Takeaway
- The combination sort | uniq is a classic pattern for frequency analysis in text data.
- uniq requires sorted input to correctly detect adjacent duplicates.
