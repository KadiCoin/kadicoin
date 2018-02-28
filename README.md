**KadiCoin Project**

KadiCoin is an experimental cryptocurrency.<br>
Its name comes from Kadikoy, Turkiye where a group of friends meet at.<br>
Our aim is to create an awareness of Blockchain Technology and its use cases.<br>

**Installation**

sudo apt-get -y update<br>
sudo apt-get -y upgrade<br>

sudo apt-get install -y wget<br>
sudo apt-get install -y curl<br>
sudo apt-get install -y git<br>
sudo apt-get install -y build-essential<br>
sudo apt-get install -y autoconf<br>
sudo apt-get install -y automake<br>
sudo apt-get install -y libtool<br>
sudo apt-get install -y pkg-config<br>
sudo apt-get install -y libevent-dev<br>
sudo add-apt-repository ppa:bitcoin/bitcoin<br>
sudo apt-get update<br>
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev<br>
sudo apt-get install -y libboost-all-dev<br>
sudo apt-get install -y libssl-dev<br>
sudo apt-get install -y libzmq3-dev<br>
sudo apt-get install -y qdbus qmlscene qt5-default qt5-qmake qttools5-dev-tools qtbase5-dev-tools qtchooser qtdeclarative5-dev xbitmaps xterm libqt5svg5-dev qttools5-dev qtscript5-dev qtdeclarative5-folderlistmodel-plugin qtdeclarative5-controls-plugin<br>

**Get Source Code from GitHub and Build**<br><br>
git clone https://github.com/KadiCoin/kadicoin.git<br>
cd kadicoin<br>
./autogen.sh<br>
./configure<br>
make<br>
sudo make install<br>

**Create Config File**<br><br>
mkdir ~/.KadiCoin<br>
cd ~/.KadiCoin<br>
nano KadiCoin.conf<br>

**Sample KadiCoin.conf**<br><br>
\# Online Config Generator:<br>
\# https://jlopp.github.io/bitcoin-core-config-generator/

server=1<br>
\# Bind to given address and always listen on it. Use [host]:port notation for IPv6. Replace it with your own IP.<br>
\# bind=192.168.0.26<br>

\# Specify a non-default location to store blockchain and other data.<br>
\# datadir=/data<br>

\# Run this node on the Bitcoin Test Network.<br>
\# testnet=1<br>

\# Run this node on its own independent test network.<br>
regtest=1<br>

\# Username for JSON-RPC connections<br>
rpcuser=kadicoinrpcuser<br>

\# Password for JSON-RPC connections<br>
rpcpassword=Put Some Strong Password Here<br>

**Run KadiCoind**<br><br>
\# Run KadiCoind and see its messages on your console<br>
KadiCoind -printtoconsole<br>
\# Run KadiCoind as a daemon (service)<br>
KadiCoind -daemon<br>
