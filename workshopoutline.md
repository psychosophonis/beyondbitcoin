# Workshop Outline

## Week One:

- Using an Exchange to buy Ether/Bitcoin
- Setting up a Wallet.
- Transferring Ether/Bitcoin for exchange to wallet.
- Sending Ether/Bitcoin between wallets.
- Establish a Glossary and develop a Diagram of the Architecture.
- Document and discuss use cases.

## Week Two:

* To discuss:
  * Suggested structure of tonight's class
  * Technical functionality of block chain / hashing / nonce / work (from last week)
  * On Slack, there is a new channel called "uses" ... any new use of blockchain technology discovered, please place here
  * Fully functional prototype concept: a red LED sitting on a Raspberry Pi lights when someone transfers $1 worth of Ethere to a specified account (key?). (Where do we get the Raspberry Pi's from?) Why?
    * Test real world transaction
    * Test IOT devices capability to connect / integrate with blockchain
    * Confirm that transaction can securely cause an electronic device / IOT activation
  * Research Required for fully functional prototype
    * Can Ethereum node sit on Raspberry Pi? (what is a 'full node' and why would it be required?)
      * See here: https://pgaleone.eu/raspberry/ethereum/archlinux/2017/09/06/ethereum-node-raspberri-pi-3/
    * Raspberry Pi connected to network
    * Raspberry Pi triggeting LED light (shield needed?)
* Set up Wallet
  * Purchase Ether/Bitcoin
  * Send Ether / Bitcoin between wallets
* Contract languages. What are they? and how are they different?
  * Solidity
  * Serpent
  * Mutan
  * LLL
* Run through full dApp (Ethereum) 'Hello World' tutorial. Tutorials to chose from are:
  * dApp for beginners: https://dappsforbeginners.wordpress.com/tutorials/setting-up-your-development-environment/
  * Voting app in Ethereum: https://medium.com/@mvmurthy/full-stack-hello-world-voting-ethereum-dapp-tutorial-part-1-40d2d0d807c2
  * https://forum.ethereum.org/discussion/1634/tutorial-1-your-first-contract


## Week Three:

This week's goal is to run the Hello World contract that runs on Ethereum.

To start:
1) Installing and setting up CLI (or stay with Ethereum Wallet) https://gist.github.com/cryptogoth/10a98e8078cfd69f7ca892ddbdcf26bc
   * Creating Account (in Rinkoby)
   * Getting test Ether
2) Test transfering Ether from one account to another
   * eth.sendTransaction({from: '0x036a03fc47084741f83938296a1c8ef67f6e34fa', to: '0xa8ade7feab1ece71446bed25fa0cf6745c19c3d5', value: web3.toWei(1, "ether")})
3) Run Hello World example https://github.com/ethereum/go-ethereum/wiki/Contract-Tutorial
   * Install Solidity compiler
   * Run 'Hello World' contract

## Week Four:
- Create a simple dApp (distributed application) - a front end for the voting contract.
- Discussion: Revisiting use cases - How can we use smart contracts to create new forms of organisation?
- Can we use a contract to propose and vote on a dApp to develop for the rest of term?

## Week Five:

NEXT POLYGONDOOR BITCOIN WORKSHOP

- Videos of Vitalik (on Ethereal channel) https://www.youtube.com/watch?v=W4S6WrTnepk

- Go to https://www.stateofthedapps.com/ and try and understand one of those apps
	- Show how many are a ‘game’ (have a quick review of them)
	- Show how one can drill in and see transactions on etherscan

- Show the reddit page: https://www.reddit.com/r/ethereum/

- Discuss the MetaMask / Infuria concept (of accessing Ethereal without a local node)

- Say that I used these: https://github.com/fivedogit/solidity-baby-steps/tree/master/contracts/

- Can only send to contract … cannot send between accounts
	•	Sender -> Contract
	•	Contract -> Receiver (using money it received).

- Previous question about the below code going wrong …. now understand that each transaction is only to contract account:
        // Subtract from the sender
        balanceOf[_from] -= _value;
        // Add the same to the recipient
        balanceOf[_to] += _value;

- You can have as many instances of a contract as you like … each one will have a different address.

- https://ethereum.github.io/browser-solidity/ is very useful

- Go over the contract I’ve written

- Chart of Ethereum structure: https://drive.google.com/file/d/0ByR5ajtUjzNQeGJ6ajkxWGU5ckE/view?usp=sharing



## Week Six:

- Backend dApp Dev and Front End Wireframing/Specification.

## Week Seven:

- Continued dApp Dev.
- Discussion: Making things happen? Contracts with non-human objects – can we turn on an led using the blockchain..and question why we would.

## Week Eight:

- Experiments with making things happen.
- Switching on a LED using a smart contract.
- Continued dApp Dev.

## Week Nine:

- Finalise Dapp Dev and sum up what we’ve learnt about the Blockchain.

## Week Ten:

- dApp Launch Party and discussion : Where to from here?
