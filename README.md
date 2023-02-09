# DDAPP
Didactic Decentralized Application (dApp)

This Android Project is intended for dApp teachings purposes.

Technically, this application works as user interface for WOC, GorillaPool e Bitails APIs, that allows the user to use the Bitcoin Blockchain, sending TXs and reading TX's details with the help of these APIs.

It is worth for Building Descentralized Application - DAPP on Android Platform using the Bitcoin Network

This template includes classes that enables the creation and use of Bitcoin legacy wallets from a hexadecimal private key.

Features of this Android DAPP Template per Button:

01) PVT KEY - insert a private Key in Hexadecimal format Only to access your Compressed or Uncompressed P2PKH Bitcoin Address;

02) WRITE BC - attach text data to an unspendable 0 sat UTXO using OP_FALSE OP_RETURN and send it in a transaction to the Bitcoin MemPool;

03) SEND SATS - send satoshis to any P2PKH Bitcoin address, and if you want it attaches an optional description to the transaction as an unspendable 0 sat UTXO using OP_FALSE OP_RETURN;
     
     It is possible to send the same amount of Satoshis to many different address, by creating a lists like this:
     
     1add1...; 1add2....; 1add3; ...; 1addn;
     
     The code allows up to 250 different addresses at the same time, but it was not tested up to this limit;
     
     The Change Wallet Address option is the address to where you can send the change of a previous address during a transaction. You can use this option when you don´t want to use the previous address anymore.


04) READ BC - reads from the blockchain TXID related to your P2PKH address and display the data if there is found unspendable 0 sat UTXO using OP_FALSE OP_RETURN;

05) SPEC UTXOS - allows you to select which set of UTXOs related to you P2PKH address will be used in the next transaction;

06) TX VERIFY - displays the TXID and hexadecimal body of the last TX send to the Mempool;

07) TO PBKEY - send satoshis to an public key in SEC format and an optional description;

08) SPEND PBKEY - send all the satoshis from a P2PK script hash to an P2PKH address;

09) TOR TOKEN - creates a Token controlled by your P2PKH address PVT KEY, the UTXO merges the public key script and data inserted through OP_TRUE OP_RETURN opcodes;

10) ODR TOKEN - creates a Token controlled by your P2PKH address PVT KEY, the UTXO merges the public key script and data inserted through OP_PUSHDATA1, or OP_PUSHDATA2, or OP_PUSHDATA4 and OP_DROP opcodes;

11) SEND TOKEN - transfer a single TOR TOKEN or ODR TOKEN to another P2PKH address through its script hash;

12) MELT TOKEN - melts a single TOR TOKEN or ODR TOKEN and send its backed satoshis to the indicated P2PKH address through its script hash;

13) 2TR TOKEN - creates a TRUE TOKEN from a TOR TOKEN or ODR TOKEN, such token is an open access token for teaching purposes, where anyone can use the satoshis on it;

14) PASSWORD - insert a password of at least 8 char and get the related PVT KEY of that password or access your Compressed or Uncompressed P2PKH Bitcoin Address related to that password;

15) LISTEN - listens the blockchain to search for new TX in a specific address and send data through it to. Intended for new applications building purposes. (Disabled by default but can be re-enabled in the code);

16) DIDACTIC - just to display some internal results as a debugger for the developer. (Disabled by default but can be re-enabled in the code);


The code of all JAVA classes of the project are open, nevertheless they are still poorly documented, and it is not neatly written as well.
Though template worked well on our tests, we do not warrant it to be free of bugs or any malfunctionality whatsoever. Therefore, use at your own risk.

The set of classes employed in this template project includes:

Ecc.java - Ellipitic curve secp256k1;

EcdsaSecretus.java - ECDSA based on secp256k1 elliptic curve;

SHA256G.java - SHA256 hash function with methods to deal with different input/output types;

TonelliShanks.java - to deal with some Ellipical Curves operations;

Ripemd160.java - RIPEMD160 hash function to deal with bitcoin wallets;

Keygen.java - Classe to deal with private/public key generation and encoding, generation of BSV wallets, SEC public key encode and decode, DER ECDSA singature encoding and decode.


# Contribuição

Você pode contribuir com este desenvolvimento enviado BSV para o seguinte endereço:

185vbyAYDqZCNBaxHNVM7pxzV2RBX4zFiS
