
# SahaCoin - Power of the Sahara Cryptocurrency
![Logo](https://www.sahacoin.org/images/logo.png)

SahaCoin is a decentralised and eco-friendly currency with near-instant transaction speeds and negligible transaction fees built upon Proof of Stake. Sahacoin is based on the latest Proof-of-Stake technology. No more power hungry mining that is harmful to the environment like in Bitcoin.

Everyone gets paid to keep the network secure. Everyone shares the bank history, so its transparent. The software is open source so you know its safe. It is anonymous and anyone can open an account. It is extremely fast, you can send money to anyone in the world within minutes.

## Installation

Install SahaCoin Wallet on Windows or Linux, download wallet https://www.sahacoin.org/index.php?r=site/download


Install SahaCoin node on Ubuntu Server 18.04

```bash
# Update your Ubuntu server
sudo apt-get update && sudo apt-get upgrade -y
  
# Install the required dependencies
sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev libboost-program-options-dev libminiupnpc-dev libzmq3-dev libprotobuf-dev protobuf-compiler unzip software-properties-common cmake -y

# Install the repository ppa:bitcoin/bitcoin
sudo add-apt-repository ppa:bitcoin/bitcoin

#Install Berkeley DB
sudo apt-get update && sudo apt-get install libdb4.8-dev libdb4.8++-dev -y

Download the SahaCoin Linux daemon
wget "https://www.sahacoin.org/index.php?r=site/daemon" -O sahacoin-daemon-linux.tar.gz

#Extract the tar file
tar -xzvf sahacoin-daemon-linux.tar.gz

#Download the SahCoin Linux tools
wget "https://www.sahacoin.org/index.php?r=site/linux" -O sahacoin-qt-linux.tar.gz

#Extract the tar file
tar -xzvf sahacoin-qt-linux.tar.gz

#Install the daemon and tools for SahaCoin Wallet
sudo mv sahacoind sahacoin-cli sahacoin-tx /usr/bin/

#Create the data directory for your SahaCoin
mkdir $HOME/.sahacoin

#Edit SahaCoin conf file
nano $HOME/.sahacoin/sahacoin.conf -t

#Paste the following lines

rpcuser=rpc_sahacoin
rpcpassword=dR2oBQ3K1zYMZQtJFZeAerhWxaJ5Lqeq9J2
rpcallowip=127.0.0.1
listen=1
server=1
txindex=1
daemon=1

#Save file and start your node with following command

sahacoind
```
    

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate! Please adhere to this project's `code of conduct`.


## License

[MIT](https://choosealicense.com/licenses/mit/)

