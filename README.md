# Unit 18 Blockchain Homework

## ZBank Private Testnet

The testnet is designed to be used to explore potentials for blockchain at ZBank.

### Initial Setup

The genesis block for our testnet was created using puppeth, a tool bundled with the Go Ethereum tool.  Our network is called joeyjojojuniorshabadoo. There are two nodes on the testnet: node1 and node2.

In order to begin mining, open a terminal window and navigate to the blockchain-project folder. Once there, enter the following command:

- ./geth --datadir node1 --unlock "0xdEC3896dCF02cF87e70c01Da23306479627Da436" --mine --rpc --allow-insecure-unlock

and then enter the password "homersimpson" (there is no prompt for the password)

Then open a second terminal window in the blockchain-project folder and enter the following command:

- ./geth --datadir node2 --unlock "0xDa6A84C42C2f33205d690027DE2d9d285685CDAE" --mine --port 30304 --bootnodes "enode://SEALER_ONE_ENODE_ADDRESS@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock

and enter the password "nedflanders"

> get the SEALER_ONE_ENODE_ADDRESS from the first terminal window

Now both of the nodes should be activated, connected and mining.

### Connect to MyCrypto

Now connect the nodes to MyCrypto to begin sending ETH by taking the following steps:

1. Open the MyCrypto app and make sure you are on the joeyjojojuniorshabadoo network (you may need the chain/network ID, which is 702)
2. Access the wallet for node1 by opening the Keystore File in the node1 folder
3. Enter the password for node1

### Send ETH to Node2

1. Enter the public address for node2 into the "To Address" box (node2 public address is 0xDa6A84C42C2f33205d690027DE2d9d285685CDAE)
2. Enter the amount
3. Enter the fee
4. Send the ETH

