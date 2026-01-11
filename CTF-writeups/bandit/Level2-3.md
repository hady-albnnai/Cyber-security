# Bandit Level 2 → Level 3

## Goal
Find the password hidden in a file named `spaces in this filename`.

## Challenge
The filename contains spaces, which terminals interpret as separate arguments.

## Solution

### Method 1: Use quotes
```bash
cat "spaces in this filename"
