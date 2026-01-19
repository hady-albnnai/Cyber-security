# Bandit Level 6 → Level 7

## Objective
Find the file somewhere on the server with these properties:
- Owned by user bandit7.
- Owned by group bandit6.
- Size is 33 bytes.

## Commands Used
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password

## Password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
