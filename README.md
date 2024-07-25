# cryptography_vs_quantum_computer

Can we throw whole current cryptography to bin if we would have quantum computer?

1. What is quantum computer<br>
Let's start with explanation what is quantum computer and what is the difference between quantum computer and classic one.
Our computers use bits. Bit can have 2 values: 0 and 1. Quantum computer is using qubit (quantum bit) which can have all spectrum of values, not only 0 or 1 which
allow it to transfer much more data than bit. Quantum computer is then much faster than normal computer.

2. Basic cryptography<br>
Our current cryptography in many cases base on integer factorization. It's easy for human to say what is the result of 7 * 13,
but it's much harder to find numbers to multiply to achieve given result e.g do you know what numbers you need to multiply to get 437? 
Not that easy, right?

3. RSA (Rivest–Shamir–Adleman)<br>
One of the most widely used public key cryptosystem is RSA. RSA uses two keys public and private (sometimes called secret) key. 
When someone wants to send you message they encrypt it with public key and can be sure that only person with private key will be able to decrypt it.
Generating public and private key base on two large prime numbers along with an auxiliary value.
Why is it safe? Because we need around 19.8 quadrillion years using Google's computational power to break RSA-2048 with brute force[2].
And why it won't be safe anymore with quantum computer? Because with Shor's algorithm it will take 10-100 seconds (depending on number of qubits) to crack RSA-2048!

4. Is AES (symmetric cryptography) also vulnerable?<br>
Let's look at AES algorithm as it's one of the most popular symmetric key cryptography algorithm. By symmetric cryptography we understand 
algorithm that uses the same key for both - encryption and decryption. 
For AES key generation doesn't base on integer factorization, it's just random stream.
Why AES is resistant for attacks nowadays? Because on standard computer it would take more time than universe exists 14 billion[6].
Why AES will still be secure even in quantum computers' era? Because it will take decades to break AES 256 with Grover's algorithm.
To be honest even AES 128 would be quantum resistance.

So can we throw whole current cryptography to bin if we would have quantum computer? Definitely no!
Some algorithms like RSA will be useless but another as AES are quantum resistance.


[1]https://en.wikipedia.org/wiki/RSA_(cryptosystem)
[2]https://www.linkedin.com/pulse/quantom-encryption-time-crack-33-anders-carlius/
[3]https://www.btq.com/blog/how-far-away-is-the-quantum-threat
[4]https://www.quintessencelabs.com/blog/breaking-rsa-encryption-update-state-art
[5]https://crypto.stackexchange.com/questions/10415/how-to-choose-keys-for-a-block-cipher
[6]https://www.reddit.com/r/theydidthemath/comments/1x50xl/time_and_energy_required_to_bruteforce_a_aes256/
[7]https://www.quora.com/If-quantum-computing-came-out-tomorrow-how-long-till-AES-256-gets-broken