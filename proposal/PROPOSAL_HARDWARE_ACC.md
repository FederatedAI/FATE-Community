# Proposal: Hardware Accleration Support
Author: <[Junxue ZHANG](https://github.com/snowzjx), Junhuan SUN, Bin ZHAO>

Discussion: N/A

# Abstract #
This proposal intends to allow FATE to leverage hardware-based accelerators, such as GPU/FPGA, for better performance.

This proposal will contribute a universal architecture for FATE to use these hardware-based accelerators, including APIs, memory layout standards, data structure, and so on.

This proposal mainly targets accelerating cryptographic operations, such as Paillier encryption, ciphertext computation, and so on.

# Background #
In FATE, various cryptographic operations have been used to protect data privacy. Specifically, they are:  

1. Paillier Encryption w/ Obfuscation.

2. Paillier Encryption w/o Obfuscation.

3. Paillier Decryption.

4. Ciphertext Matrix Addition.

5. Ciphertext & Cleartext Matrix Element-wise Multiplication.

6. Ciphertext & Cleartext Matrix Multiplication.

7. Ciphertext Matrix Summation.

8. RSA Encryption/Decryption.

9. RSA Blind.

10. RSA Unblind.

Although preserving data privacy, these cryptographic operations also cause a dramatic performance penalty. In our experiment, these cryptographic operations cause >~80% total time when executing an end-to-end application. Thus, if we can efficiently accelerate these cryptographic operations, the end-to-end performance of FATE could be significantly improved.

# Proposal #
[A precise statement of the proposed change.]

# Non-Goals #
[Anything explicitly not covered by the proposed change.]

# Rationale #
[A discussion of alternative approaches and the trade-offs, advantages, and disadvantages of the specified approach.]

# Compatibility #
[A discussion of any compatibility issues that need to be considered]

# Implementation #
[A description of the steps in the implementation, who will do them, and when.]

# Open issues (if applicable) #

N/A
