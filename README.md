## sec practical
# HOW TO DOWNLOAD IPFS
🔹 Step 1: Go to the official website
Visit: https://docs.ipfs.tech/install/ipfs-desktop/

🔹 Step 2: Download IPFS Desktop
Choose the right version for your operating system:

Windows .exe


🔹 Step 3: Install it
Windows: Run the .exe and follow the installer.


🔹 Step 4: Run IPFS Desktop
Open the app — it will start the IPFS daemon and give you a friendly GUI to interact with your node.

Windows: Add the ipfs.exe directory to your system's PATH environment variable.


Desktop: Open the app, it should show your peer ID and connected nodes.
![image](https://github.com/user-attachments/assets/d1b6b3e6-a9d0-4e34-b9b1-ce58492f04d7)


# FILE UPLOADING
1. I clicked on the file selection in IPFS desktop.
2. Then i selected the option "import" and uploaded a  pdf file and audio and a admit card file and also a image.
3. Once the file was uploaded, IPFS generate a unique CID(content indentifier) for the file

   ![Screenshot 2025-04-10 113433](https://github.com/user-attachments/assets/82311470-ef31-4eea-9a42-0f1fdff48bac)

## Encrypting and decrypting

1) Download IPFS CLI:
```
wget https://dist.ipfs.tech/go-ipfs/v0.22.0/go-ipfs_v0.22.0_linux-amd64.tar.gz
```
2) Extract the tar file:
```
tar -xvzf go-ipfs_v0.22.0_linux-amd64.tar.gz
```
3) Install IPFS:
```
cd go-ipfs
./install.sh
```
4) Initialize IPFS Node:
```
~/.local/bin/ipfs init
```
5) Start IPFS Daemon:
```
~/.local/bin/ipfs daemon
```
6) Create a sample file:
```
echo "hello, IPFS!" > hello.txt
```
7) Add original file to IPFS:
```
~/.local/bin/ipfs add hello.txt
```
8) Encrypt the file using OpenSSL:
```
openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in hello.txt -out hello.enc
```
9) Upload the encrypted file to IPFS:
```
~/.local/bin/ipfs add hello.enc
```
10) Decrypt the file:
```
openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in retrieved.enc -out decrypted.txt
```
11) See decrypted content:
```
cat decrypted.txt
```
12) Add decrypted file to IPFS:
```
~/.local/bin/ipfs add decrypted.txt
```
![WhatsApp Image 2025-04-21 at 14 44 51_b088d58e](https://github.com/user-attachments/assets/21c80cd0-af32-4a47-ab0d-b6cac0fd7d0f)


# BLOCKCHAIN PRACTICAL METAMASK WALLLET

#CREATE METAMASK WALLET (Sepolia testnet)
  #introduction 
  This is a practical task demonstrate how to create a Metamask wallet and perform a trasaction using the sepolia Testnet

# Transtion detail
Network: sepolia testent amount sent: 0.02ETH Transaction hash: 0x7a95585dd38725214ee4c0b74dac13d8a39a410555b40bea68cf929b5ff629f1

# Getting sepolia ETH from Faucet 
1.Visited the google cloud Sepolia Faucet.

2.Logged in with my google account.

3.Entered my Metamask wallet address.

4.Clicked on "Request 0.02 ETH".

5.ETH was sent to my wallet within a few seconds.

6.Verified the transaction on sepolia Etherscan.

![Screenshot 2025-04-09 214614](https://github.com/user-attachments/assets/1b00e5dd-08f4-4dbd-84c5-59ee2a21d2c5)


# steps  followed
1.Connected Metamask to Sepolia Testnet.

2.Claimed Sepolia ETH from faucet.

3.Sent ETH to another Address.

4.Verified transaction was confirmed.


![Screenshot 2025-04-09 214501](https://github.com/user-attachments/assets/0eabafe0-46f7-4094-9c74-0d91af31ffba)

# HYPERLEDGER FABRIC PRACTICAL 
1. installing golang
   
   ```sudo apt install golang-go```
   
Installs Golang, which is necessary for running Hyperledger Fabric binaries.
![Screenshot 2025-04-16 102328](https://github.com/user-attachments/assets/ed04f672-42e1-4339-8f88-ccaae2e6dfb9)

3. Check Docker version
   ```docker --version```
   Verifies that Docker is installed and running correctly.

   ![Screenshot 2025-04-16 103341](https://github.com/user-attachments/assets/15740a40-31e4-4f04-964d-a455761430ec)


4. Check Docker compose version
```docker -compose  --version```
Verifies the installation of Docker Compose.
![Screenshot 2025-04-16 103419](https://github.com/user-attachments/assets/87c8d15b-e8ae-4202-9782-77e3af4da03d)



5. List Files in current dictionary
   ```is ```
   Shows the list of files and folders in the current directory.

6. Clone the Fabric Samples Repository and Move into the Cloned Folder

```git clone https://github.com/Akshitakaushik123/fabric-samples.git; cd fabric-samples```

Downloads the official Hyperledger Fabric sample code from GitHub. Enters the cloned folder where Fabric examples are available.


![Screenshot 2025-04-16 104000](https://github.com/user-attachments/assets/36606832-000b-4d91-86a4-cef29f5abb98)


6. Download Fabric Binaries
```  curl -sSL https://bit.ly/2ysbOFE | bash -s```


Downloads necessary Fabric binaries and Docker images like peer, orderer, and cryptogen.


![Screenshot 2025-04-16 130952](https://github.com/user-attachments/assets/b1a3a5d8-78f7-46cc-a90c-faf92bbeb160)



7.Enter the Test Network Directory

```cd test-network```
Navigates to the directory that contains scripts for running a sample Fabric network.


8. View the Network Script
```./network.sh```
Shows the options available with the network.sh script.


![Screenshot 2025-04-16 133627](https://github.com/user-attachments/assets/246ece54-e75d-40fc-bf36-16f88b255c82)

10. Start the Fabric Network
```./network.sh up```
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.






10.Create a Channel
```./network.sh createChannel```
Creates a default channel (usually named mychannel) and joins the peers to it.



![Screenshot 2025-04-16 132703](https://github.com/user-attachments/assets/3c137537-53f8-4a4c-bf8a-18196289e5e0)

11. Shut Down the Network
```./network.sh down```
Stops all containers and deletes the crypto material and artifacts created during the setup.



![Screenshot 2025-04-16 132938](https://github.com/user-attachments/assets/5722ca1c-f5d2-430d-af8f-6f05f69c23d1)

#solidity


#1. Use Remix (Beginner-Friendly, No Setup Needed)
Go to  https://remix.ethereum.org

It’s an online IDE to write, compile, deploy, and test Solidity contracts.

Example: Hello World Contract
```// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract HelloWorld {
    string public message = "Hello, Blockchain!";

    function setMessage(string memory _message) public {
        message = _message;
    }
}
```
In Remix:

Click File Explorer → Create new file → name it HelloWorld.sol

Paste the code above.

Click Solidity Compiler → Compile

Go to Deploy & Run Transactions → Deploy the contract

Use the UI to call setMessage() or read message




#2. Install Hardhat (For Local Dev with Node.js)
If you want to build real projects:
```npm install --save-dev hardhat
npx hardhat
```
Choose "Create a basic sample project".

Then you can:

Write your contracts in contracts/

Write tests in test/

Deploy using scripts in scripts/

✅ Hardhat also supports local Ethereum nodes (Hardhat Network) and real testnets.







#3. Use MetaMask for Deployments to Testnet
Install MetaMask, create a wallet, and connect to a testnet like Goerli or Sepolia. You’ll need free test ETH from a faucet (I can help with that too).
Tools & Resources
Remix IDE: best for quick testing

Hardhat: advanced dev workflows

```Solidity Docs: https://docs.soliditylang.org/```

```CryptoZombies: fun gamified Solidity tutorial → https://cryptozombies.io/```

## Create a voting system with multiple candidates. Each address can vote only once.
```
pragma solidity ^0.8.0;

contract Voting {
    struct Candidate {
        string name;
        uint voteCount;
    }

    Candidate[] public candidates;
    mapping(address => bool) public hasVoted;

    constructor(string[] memory candidateNames) {
        for (uint i = 0; i < candidateNames.length; i++) {
            candidates.push(Candidate(candidateNames[i], 0));
        }
    }

    function vote(uint candidateIndex) public {
        require(!hasVoted[msg.sender], "You have already voted");
        require(candidateIndex < candidates.length, "Invalid candidate index");

        candidates[candidateIndex].voteCount++;
        hasVoted[msg.sender] = true;
    }

    function getCandidates() public view returns (Candidate[] memory) {
        return candidates;
    }

    function totalCandidates() public view returns (uint) {
        return candidates.length;
    }
}
```
![image](https://github.com/user-attachments/assets/3ca00e3f-5ef9-47b8-ac4f-0dfe12202604)
![image](https://github.com/user-attachments/assets/a3d22f46-14e2-4b16-9c42-8445dd170215)


## Write a contract that manages a list of student records (name, roll number). Allow adding and retrieving student data.
```
pragma solidity ^0.8.0;

contract StudentRecords {
    struct Student {
        string name;
        uint rollNumber;
    }

    Student[] public students;

    function addStudent(string memory _name, uint _rollNumber) public {
        students.push(Student(_name, _rollNumber));
    }

    function getStudent(uint index) public view returns (string memory, uint) {
        require(index < students.length, "Invalid index");
        Student memory s = students[index];
        return (s.name, s.rollNumber);
    }

    function totalStudents() public view returns (uint) {
        return students.length;
    }
}
```
![image](https://github.com/user-attachments/assets/414c9b03-d58f-46c8-a829-d338a10deb3d)
![image](https://github.com/user-attachments/assets/33c2639e-8690-4a9d-8e27-6b7b12c93aba)


## Develop a contract that only allows the deployer (owner) to call a specific function (use modifiers).
```
pragma solidity ^0.8.0;

contract OwnerOnly {
    address public owner;

    constructor() {
        owner = msg.sender;
    }

    modifier onlyOwner() {
        require(msg.sender == owner, "Not the contract owner");
        _;
    }

    function privilegedAction() public onlyOwner {
        // Protected logic here
    }
}
```
![image](https://github.com/user-attachments/assets/d59c7cb4-d0ba-412b-b3ac-24e7f2a75eee)
![image](https://github.com/user-attachments/assets/39f24ed2-33b4-4651-a3e4-bc7c6494fd90)



## Write a contract where people can donate Ether and the top 3 donors are tracked
```
pragma solidity ^0.8.0;

contract TopDonors {
    struct Donor {
        address addr;
        uint amount;
    }

    Donor[3] public topDonors;

    function donate() public payable {
        require(msg.value > 0, "Must donate some ETH");

        // Check if already a top donor
        for (uint i = 0; i < 3; i++) {
            if (topDonors[i].addr == msg.sender) {
                topDonors[i].amount += msg.value;
                sortTopDonors();
                return;
            }
        }

        // Replace the lowest if new donor is bigger
        if (msg.value > topDonors[2].amount) {
            topDonors[2] = Donor(msg.sender, msg.value);
            sortTopDonors();
        }
    }

    function sortTopDonors() internal {
        for (uint i = 0; i < 3; i++) {
            for (uint j = i + 1; j < 3; j++) {
                if (topDonors[j].amount > topDonors[i].amount) {
                    Donor memory temp = topDonors[i];
                    topDonors[i] = topDonors[j];
                    topDonors[j] = temp;
                }
            }
        }
    }

    function getTopDonors() public view returns (Donor[3] memory) {
        return topDonors;
    }
}
```
![image](https://github.com/user-attachments/assets/3e07eb74-cbc6-4af6-bc49-23dd21e10b63)
![image](https://github.com/user-attachments/assets/a054973c-9941-48af-87ee-1e198f5b3a4b)


## Implement a simple auction system where users can place bids, and the highest bidder wins.
```
pragma solidity ^0.8.0;

contract SimpleAuction {
    address public highestBidder;
    uint public highestBid;
    address public owner;

    constructor() {
        owner = msg.sender;
    }

    function bid() public payable {
        require(msg.value > highestBid, "Bid too low");

        // Refund previous bidder
        if (highestBid > 0) {
            payable(highestBidder).transfer(highestBid);
        }

        highestBidder = msg.sender;
        highestBid = msg.value;
    }

    function endAuction() public {
        require(msg.sender == owner, "Only owner can end auction");
        payable(owner).transfer(address(this).balance);
    }
}
```
![image](https://github.com/user-attachments/assets/e713b9ad-cf8a-4297-8ae8-7c12080ec553)
![image](https://github.com/user-attachments/assets/2f1e35bf-9459-450f-913c-6519c78b1ac8)


## Create a contract that splits incoming Ether between 3 fixed addresses.
```pragma solidity ^0.8.0;

contract EtherSplitter {
    address payable public addr1;
    address payable public addr2;
    address payable public addr3;

    constructor(address payable _a1, address payable _a2, address payable _a3) {
        addr1 = _a1;
        addr2 = _a2;
        addr3 = _a3;
    }

    receive() external payable {
        uint share = msg.value / 3;
        addr1.transfer(share);
        addr2.transfer(share);
        addr3.transfer(msg.value - 2 * share); // Handle rounding
    }
}
```
![image](https://github.com/user-attachments/assets/dae8c819-6eae-444b-9ca9-052a6060fe08)
![image](https://github.com/user-attachments/assets/b43626ea-c669-4dc4-a5bb-0bc41226b59f)











