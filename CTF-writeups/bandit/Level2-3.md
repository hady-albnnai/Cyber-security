
# Bandit Level 2 → Level 3

## Objective
Read the content of a file whose name contains spaces and special characters.

## Challenge
Spaces in filenames are interpreted as argument separators by the shell. The file is named spaces in this filename.

## Concepts Learned
- Filenames with spaces require special handling
- Using quotes or escape characters to preserve literal filenames

## Methods to Access the File
1. Quotes – cat "spaces in this filename"
2. Escape spaces – cat spaces\ in\ this\ filename
3. Globbing with ./** – cat ./"spaces in this filename"

## Example Command
cat "spaces in this filename"

## Key Takeaway
- Always quote or escape special characters (spaces, dashes, etc.) in filenames.
- Prefixing with ./ can help the shell correctly parse tricky filenames.
