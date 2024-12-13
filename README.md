# Linkcoin v2 client for Windows only

## Disclaimer
Proceed at your own risk.
Not financial advise.
This is purely experimental.
I will not be held liable for any loss or damages.

## Introduction
An anonymous dev reached out to me to provide a solution for the current issue with Linkcoin revival.  
Currently the chain is stuck at block 387 and is unable to continue.

![telegram-cloud-photo-size-5-6260434156051873879-x](https://github.com/user-attachments/assets/3c40c9b2-a33b-46af-9a05-b710bf3799fa)

This new Linkcoin v2 client for Windows is able to get past this block checkpoint.  
However, it will require a full chain restart.  
If you still want to run this software, make sure to backup your wallet and block data before you proceed.  
Final warning, I will not be held liable for any loss or damage.  
This is purely experimental.  
Not financial advise.

![telegram-cloud-photo-size-5-6260434156051873873-y](https://github.com/user-attachments/assets/733e89e9-1dcd-4aaf-a730-05caa077a60b)

## Instructions

### Setup Wallet
* Download and Run `linkcoin-qt.exe`.
* Exit the app.
* Create a `linkcoin.conf` file in the following directory:
`C:\Users\<Username>\AppData\Roaming\LinkCoin`

  Use template below:

```
dns=1
irc=1
listen=1
dnsseed=1
daemon=1
server=1
rpcport=9600
debug=1
txindex=1
rpcallowip=127.0.0.1
rpcbind=127.0.0.1
rpcuser=linkcoin
rpcpassword=linkcoin
addnode=198.7.123.24:9600
addnode=162.220.160.74:9600
```
* Run `linkcoin-qt.exe` and let it sync.
* Generate a Receive address.

### Start Mining
* Download [CPU miner](https://github.com/pooler/cpuminer/releases/tag/v2.5.1).
* Extract contents and use command prompt to navigate to the file.
* Run miner using the following  command:
```
minerd -a scrypt -o http://127.0.0.1:9600 --coinbase-addr=<your wallet> -u linkcoin -p linkcoin
```
![telegram-cloud-photo-size-5-6260434156051874214-y](https://github.com/user-attachments/assets/b269f80f-4421-4a30-9231-263ea7fa671b)

Join Telegram:
[@linkcoin2011
](https://t.me/linkcoin2011)



