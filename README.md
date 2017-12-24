# aes128_systemverilog
The present example deals with a block cipher, called Advanced Encryption Standard (AES), which accepts a plaintext and a cipherkey as inputs and computes the corresponding ciphertext. All input and output data to and from the algorithm are provided as a sequence of bits. 

Those bits may represent any kind of characters, numbers, or symbols in an arbitrary encoding, which is not further discussed here. Once the ciphertext is obtained from the AES block cipher, it can be transmitted over an insecure channel (for instance, the Internet) without compromising the confidentiality of the corresponding plaintext. Only a recipient who owns the same cipherkey will be able to decrypt
the ciphertext.

Currently I have developed a SystemVerilog testbench for the AES-128. The testbench have only two classes: "aes" and "d_aes". 
