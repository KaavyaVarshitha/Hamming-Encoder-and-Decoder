# Hamming-Encoder-and-Decoder

 ## Summary
 Implemented a hamming (7,4) encoder and decoder using VHDL individually and then are connected together using an error bus in between the output of the encoder and the input of the decoder. The functionality of the system is tested by injecting errors and the output is verified and compared with the system with no errors. This is a simulation project done in xilinx Vivado.

 ## Hamming (7,4) code
 The hamming (7,4) code is a method of encoding and decoding data that can correct single bit errors and detect bit errors. It works by adding three parity bits to the four bit data word forming a seven bit codeword. The parity bits are calculated based on the position of the data bits. Using this scheme, the decoder identifies and corrects any single bit error by comparing the received parity bits with the expected ones. If two bits are flipped, the error can be detected and not corrected since there will be two possible original codewords that differ by two bits.

 ## Encoder
 The encoder is designed to take a 4-bit input every rising clock edge. The encoder then calculates the parity bits using logic gates and then produces a 7-bit encoded output with the parity bits calculated and inserted at the right places.
 
 Input: 1100
 
 Codeword: 0111100
 
 ![image](https://github.com/KaavyaVarshitha/Hamming-Encoder-and-Decoder/assets/143062029/20d40ef5-2756-424c-9a16-8e7b248b6c0f)

 ## Decoder
 The decoder takes a 7-bit encoded input along with an error signal, clock and reset. At every rising clock edge, a 7-bit codeword is decoded.
 
 Input: 1011010
 
 Output: 1010
 
 ![image](https://github.com/KaavyaVarshitha/Hamming-Encoder-and-Decoder/assets/143062029/7cf37a08-05f5-4e99-96a8-b808e1351aa8)

 ## Final Hamming (7,4) Coder.
 System with no errors:
 
 ![image](https://github.com/KaavyaVarshitha/Hamming-Encoder-and-Decoder/assets/143062029/80ccc665-fc3e-4709-824b-d70984270274)
 
 System with errors:
 
 ![image](https://github.com/KaavyaVarshitha/Hamming-Encoder-and-Decoder/assets/143062029/eec9f98d-f231-40a5-aa5b-29d67541c189)

 ## Authors

Solution|Author(s)
--------|---------
Hamming (7,4) | [Kaavya Varshitha Raman Shantha](https://github.com/KaavyaVarshitha) 

## Version history

Version|Date|Comments
-------|----|--------
1.0|Nov 2023|Initial release






 
