# SEC - Introduction-to-Blockchain
Semester 2 - Skill Enhancement Course - Introduction to Blockchain

# Create ERC20 Token

My Token address : [0x1f5640FBa970C56b96a30918E911facD3033b01B](https://goerli.etherscan.io/token/0xff1cad700e094C4b6F0d4ba285d154fc56856BC3)

My wallet address : [0x683ee4a4921Ba0E3d4B4Ed9313C4386ca16D8487](https://goerli.etherscan.io/address/0xe688552eae7b81c82faaac259384ce2e002ba2c8)

Steps:-
1) Create a Account on Metamask Wallet using the Metamask extension.
2) In Metamask, go to Settings and connect the wallet to a test network, such as the Goerli Test-Network.
3) Currently we do not have any GoerliETH so we need to mine it as it will be needed for the gas fees to deploy our token.
4) From a faucet such as [https://goerli-faucet.pk910.de/](https://goerli-faucet.pk910.de/) we mine our GoerliETH.
5) Then, we go to an ERC token generator such as [https://20lab.app/](https://20lab.app) to build and deploy our token without prior experience in coding in Solidity. 
6) Configure the token's properties, such as the total supply, symbol, name, decimals, and token balances for each address.
7) Pay the gas fees to deploy the Token to the testnet
8) In Etherscan, we can see the information on our Token by putting its token address.
![image](https://github.com/PindropHailstorm/SEC---Introduction-to-Blockchain/assets/119025864/967262ad-5f95-4f95-bc67-e21f9ba967ee)

Our token is deployed.


To start the first Hyperledger Fabric network, we'll use the Fabric-samples repository. It includes important tools like CLI tool binaries and Fabric Docker Images that are necessary for using Fabric. 

Dependencies to install:

# 1.Install Docker

    sudo apt-get -y install docker-compose

# 2. Install Golang-go

    sudo apt install golang-go

# 3. Install jq

    sudo apt install jq

# 4. Install Node/java

    sudo apt install npm
    npm install node

# 5. Installing Fabric-samples Repository

    curl -sSLO https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/install-fabric.sh && chmod +x install-fabric.sh
    
Then you can pull docker containers by running one of these commands:

    ./install-fabric.sh docker samples
    ./install-fabric.sh d s 

To install binaries for Fabric samples you can use the command below:

    ./install-fabric.sh binary
    
# Building the network

1.Navigate through the Fabric-samples folder and then through the Test network folder where you can find script files using these we can run our network.

    cd fabric-samples/test-network

2.Run the ./network.sh down command to remove any previous network containers or artifacts that still exist. 

    ./network.sh down
3.Bring up a network using the following command, creating a fabric network that consists of two peer nodes and one ordering node.

    ./network.sh up 



