# WALLETS
1. custodial wallets: are centralized, and some bode else controls your money e.g coinbase, kraken.
2. cryto-currency wallets(hot wallet): e.g metamask, phantom, rabby.
    tools that will make using your hot wallet safer:
    - web3 Antivirus
    - fire.xyz
3. hardware wallets(cold wallets - permanently offline): it stores private keys offline, reducing exposure to online hacking attempts r.g trezor, but it's online sometimes.
# ADVANCED WALLETS
4. multi-sig wallets: is a smart contract that governs transactions. 
these can be setup so that they require several amount of people to sign a transaction for it to go through. e.g safe, aragon.
you can customize this so that any X number of people are required to sign before a transaction is submittted out of Y.

example:
if 3 people are needed to sign out of a possible 5 people, this is known as 3 of 5 wallets. 

if you're doing multi sig, don't store all your private keys on the same device.

5. social recovery wallets(similar to multi-sig): 
how it works
- there's a single "single key" that can be used to approve transactions.
- there is a set of at least 3 (or a much higher number) of guardian. of which a majority can cooperate to change the signing key of the account.

6. shamir backup: you give out shares of your key to trusted users, where you can recover you key when shares are combined. 

A secret recovery share is usually a sequence of 20 to 33 english words carrying a part of the cryptographic secret. like Trezor cold wallet has the feature. e.g safe, argent, trezor.


check-out "wise-signer.cyfrin.io": is made to help teach people to verify transaction they send.
- hit "start training now" or "play now" button.
- go to "simulated wallet" section.






# practice

- command
ma_buba@DESKTOP-4JPC4VR:~/wallet-security$ cast 4byte 0x474cf53d
- output
depositETH(address,address,uint16)

- command
ma_buba@DESKTOP-4JPC4VR:~/wallet-security$ cast decode-calldata "depositETH(address,address,uint16)" 0x474cf53d000000000000000000000000f39fd6e51aad88f6f4ce6ab8827279cfffb9226600000000000000000000000023618e81e3f5cdf7f54c3d65f7fbc0abf5b21e8f0000000000000000000000000000000000000000000000000000000000000000
- output
0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266
0x23618e81E3f5cdF7f54C3d65f7FBc0aBf5B21E8f
0


you can use "tools.cyfrin.io" to decode it.
click "abi-encoding" button or "safe hash calculation" if for a hardware wallet like imported on a metamask.

openzepplin has this "https://safeutils.openzeppelin.com/"
also allows you to check this safe hash to verify a transaction.

and also "swiss-knife.xyz" also include with some EIP-712 hash generator 

- AFTER BUYING HARDWARE WALLET, PRACTICE THIS IMMEDIATELY AND KNOW WHAT YOU'RE SIGNING
https://updraft.cyfrin.io/courses/advanced-web3-wallet-security/signer-advanced/verify-multi-sig-signatures
