Bandit Level 14 → Level 15
Objective
Submit the current level's password to a plain‑TCP service listening on localhost:30000.

Concepts Learned
Client‑server communication over TCP using nc (netcat)

Sending data to a network port and reading the response

Tools & Commands Introduced
nc (netcat) – network utility for reading/writing TCP connections

Pipeline (|) – feed data from one command into a network connection

Approach
Retrieve the current password from /etc/bandit_pass/bandit14.

Send the password to localhost on port 30000 using nc.

Capture the service's reply, which contains the password for the next level.

Example Command
text
echo "<password>" | nc localhost 30000
Key Takeaway
Many network services communicate via simple, plain‑text TCP protocols.

nc is a versatile tool for quick network testing and data transmission.
