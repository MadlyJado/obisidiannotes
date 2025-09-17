
You can either start TLS by switching to the protocol's TLS port

SMTP (25) - Unsecured
SMTPS (582) - TLS wrapped around SMTP



TLS Handsake (1.2)

Step 1: Client Hello:

- Says the versions of TLS supported (by the client)
- Says the ciphers supported (by the client)
- Includes a random number (for use in later steps)

Step 2: Server Hello

- Server chooses a TLS version from the list the client provided
- Server chooses a cipher from the list the client provided
- Server sends its own SSL certificate
- Server might indicate it wants the client to send its own certificate too

Step 3: Client verifies server SSL certificate



AAA

Authentication - Authenticate the user's account info (User/Password)
Authorization - Give the user the right access they need, and deny them if they don't
Accounting - Audit/Account for changes the user makes in the system