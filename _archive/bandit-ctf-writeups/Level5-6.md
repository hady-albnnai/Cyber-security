# Bandit Level 5 → Level 6

## Objective
Locate a specific file based on a combination of attributes: size, permissions, and readability.

## Concepts Learned
- Searching the filesystem with find using multiple criteria
- File attributes: size (in bytes), executable permission
- Combining logical operators (!,-a) in find expressions

## Tools & Commands Introduced
- find – search for files matching given conditions
- -size – filter by file size
- -executable / ! -executable – filter by executable bit

## Approach
1. Navigate to the target directory.
2. Use find with the criteria:
   - Type: regular file (-type f)
   - Size: exactly 1033 bytes (-size 1033c)
   - Not executable (! -executable)
3. Examine the identified file.

## Example Command
find /path -type f -size 1033c ! -executable

## Key Takeaway
- find can locate files by attributes (size, permissions, type) – not just by name.
- Understanding file permissions (executable bit) is essential for security and scripting.
```
