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




