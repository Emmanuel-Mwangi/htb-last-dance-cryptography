# The Last Dance — Hack The Box Cryptography Write-Up

## Objective

This challenge involved analyzing the supplied Python implementation of ChaCha20, identifying the vulnerability caused by reusing the same key and nonce, understanding how stream-cipher keystreams work, recovering the reused keystream through XOR operations, and decrypting the hidden flag.

### Skills Learned

-	Symmetric cryptography
-	Stream cipher concepts
-	XOR-based encryption and decryption
-	Identifying nonce-reuse vulnerabilities
-	Basic cryptographic analysis using CyberChef
-	Python source-code analysis


## 🔎 Initial Analysis
- After downloading and extracting the challenge files, two files are provided:
<div>
    <img src="https://i.imgur.com/L8fIdLp.png" />
</div>


- When analyzing source.py, the script imports the ChaCha20 cipher, the hidden flag, and Python’s os module:
<div>
    <img src="https://i.imgur.com/fag73vy.png" />
</div>


- The challenge defines an encryptMessage() function that takes a message, a key, and a nonce:
<div>
    <img src="https://i.imgur.com/0lRLIBP.png" />
</div>







