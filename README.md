AGX Coin
 
POS/MASTERNODE
 
 AgroxCoin Core (fork of PIVX) integration/staging repository
======================================

Quick installation of the AgroxCoin daemon under linux. See detailed instructions there [build-unix.md](build-unix.md)

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/agroxofficial/AgroxCoin.git
    cd AgroxCoin
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip agroxd
    sudo strip agrox-cli
    sudo strip agrox-tx
    cd ..

Running the daemon:

    agroxd 

Stopping the daemon:

    agrox-cli stop

Demon status:

    agrox-cli getinfo
    agrox-cli mnsync status
 




FEATURES
Coin Ticker: AGX
Block Time: 1 min
Masternode Collateral: 1000 AGX
Total Supply:  21,000,000 AGX
Premine: 197,000 AGX
Staking Time: 24 hours

 