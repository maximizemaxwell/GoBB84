# GoBB84: Go-based BB84 Quantum Key Distribution Simulator
![Ias](https://embed.pixiv.net/artwork.php?illust_id=124045485&mdate=1730870793)

## Overview
GoBB84 is a project that simulates BB84 Quantum Key Distribution(QKD)
protocol using the GO language.
In this project **Evelyn** and **Astra** are trying to share secret key.
However, **Ias** attempts to intercept their communication through eavesdropping.
Evelyn and Astra use BB84 protocol to securely exchange their key and detect Ias's eavesdropping attempts.
GoBB84 includes quantum gate operations, secret key exchange, and eavesdropping detection features, 
allowing users to analyze the advantages of quantum cryptography over classical encryption methods.

---

## Short Backgrounds on Quantum Cryptography

### QKD
Quantum Key Distribution (QKD) is a technique that uses the principles of quantum mechanics to securely share an encryption key
while detecting any eavesdropping attempts. 
Classical encryption systems rely on complex mathematical problems (e.g., prime factorization), 
but they may become vulnerable with advancements in quantum computing. 
In contrast, quantum cryptography leverages the laws of physics to ensure theoretically absolute security.

### BB84 Protocol

![eve&astra](https://pbs.twimg.com/media/Gh4PpGLWwAA8bsZ.jpg:large)
The BB84 (Bennett & Brassard 1984) protocol is one of the most well-known quantum key distribution methods.
It enables Evelyn and Astra to securely share a secret key while detecting any eavesdropping attempts by Ias.


The main steps of BB84 are as follows:

1. Evelyn generates a random bit sequence and encodes qubits using randomly chosen bases before sending them to Astra.
2. Astra measures the qubits using a random basis (matching bases yield correct values, while mismatched bases result in random outcomes).
3. Evelyn and Astra publicly share their basis choices and retain only the matching cases.
4. If Ias (the eavesdropper) intercepts the qubits, errors are introduced, and Evelyn and Astra can detect the eavesdropping attempt by analyzing the error rate.

