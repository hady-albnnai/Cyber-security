Bandit Level 15 → Level 16
Objective
Submit the current level's password to an SSL‑secured service on localhost:30001.

Concepts Learned
Establishing a secure TLS connection using openssl s_client

Transmitting data over an encrypted channel

Interacting with network services that require SSL encryption

Tools & Commands Introduced
openssl s_client – command‑line TLS/SSL client

-connect host:port – target server and port specification

-quiet – suppress verbose certificate output (optional)

Approach
Open a TLS connection to the service.

Submit the password for the current level through the encrypted session.

Retrieve the password for the next level from the service's response.

Example Command
text
echo "<current_password>" | openssl s_client -connect localhost:30001 -quiet 2>/dev/null
Key Takeaway
SSL/TLS ensures confidentiality and integrity of data in transit.

Command‑line tools like openssl s_client enable direct testing of secure services.

Self‑signed certificates are acceptable in controlled lab environments but require proper validation in production.

