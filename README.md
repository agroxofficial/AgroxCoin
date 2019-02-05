AgroxCoin Coin
 
POS/MASTERNODE
 
 
 
 agroXCoin Core  integration/staging repository
======================================

Quick installation of the agroXCoin daemon under linux. See detailed instructions there [build-unix.md](build-unix.md)

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/agroxofficial/agroX.git
    cd agroX
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
 
 


FEATURES:
 
	Coin Ticker: AGX
	Block Time: 1 min
	Masternode Collateral: 1000 AGX
	Total Supply:  21,000,000 AGX
	Premine: 197,000 AGX
	Staking Time: 24 hours
	
Reward Diagram:

	Listed below is the block reward distribution table for AGX masternode owners and
	non-masternode owners, whom have their wallets open for staking. With each block a
	different node is randomly selected and rewarded. The ‘minted’ block rewards are
	distributed on a sliding percentage scale between masternode owners and staked owners to
	create a fair distribution of coins. Be sure to read the AGX whitepaper for more details on
	masternode and staking.	
	
![Image description](http://66.42.42.97/img/1.png)

![Image description](http://66.42.42.97/img/2.png)

 
