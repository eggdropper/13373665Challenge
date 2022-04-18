# 13373665 Challenge Solutions
<p align="center">
<img height="100px" src="https://infura-ipfs.io/ipfs/QmNjhxherviDtQJHAb7U3WukJuBseLh3uWiRyBtUeQKQfG" alt="QmNjhxherviDtQJHAb7U3WukJuBseLh3uWiRyBtUeQKQfG" title="">
</p>

The solutions to the easter egg hunt.

## Table of Contents  

- [Round 1](#round-1)
  * [Challenge 1](#challenge-1)
  * [Challenge 2](#challenge-1)
  * [Challenge 4](#challenge-1)
  * [Challenge 5](#challenge-1)

## Round 1

### Challenge 1

Cardano's mneumonics for private key seed phrases are based off the BIP39 standard. And the 15 numbers shown correspond to a mneumonic seed phrase. Each number corresponds to an index in the word list. Match the number with the word to get the seed phrase. You can find the word lists here: https://github.com/bitcoin/bips/tree/master/bip-0039

### Challenge 2

Cardano NFT's rely on [IPFS](https://ipfs.io/) for distrubuted file hosting. When files are uploaded, a hash is used to identify it and you can paste that hash into an IPFS gateway to find them. These files technically live on the 'dark web', hence the hint. Pasting the hash into any gateway should've resulted in a screenshot of the mneumonic.

### Challenge 4

The mneumonic here is encoded in hex. Pasting the string into a hex-unicode decoder would result in the wallet's mneumonic.

### Challenge 5

The picture of the stegasaurus hints the hunter should use a stenographic technique. Stenography is the technique of hiding data in images. No password was used to hash the mnuemonic text. I used the `steghide` linux package to encode the image. In hindsight I see that some of the online tools were not able to extract the data. 

