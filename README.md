# RFID-wallet
RFID Card based EVM wallet abstraction

## Main Wallet characteristics

* Smart Contract wallet abstraction.
* Wallet enablement/disablement using password or confidence (one or multiple) wallet address, set by user.
* Private and optional pin code used in transactions that try to use a value above specific threshold(set by user setting threshold 0 to require it in every tx).
* Autoblocking mechanism when suspicius use detected.
* Configurable single transaction limit and daily limit.
* Option of token holding(ERC20, ERC721...) adds the possibility of tokenitzation of services(i.e. Public services tokenization, restaurant vouchers, bus ticket...).
* EIP-165(Standard interface detection) support to enable safe transfer.
* Deployer smart contract who deploys the whallet contract, so the user is the unique responsable of the wallet and can adjust the configuration based on him securty requieriments.
* Wallet Name service built in on deployer smart contract.
* Confident RFID-Wallet hardware verification.
* User can access to wallet configuration through app front end using the passphrase(if metaTX) or from confident wallet.
* If user have enough confidence in RFID-Wallet company, a company addres can be one of the confident address. this garantees ful recoverability of the wallet.

## Smart contract conceputal definition 


<p align="center">
	<img src="smart-scontracts.PNG"  height="550">
</p>
