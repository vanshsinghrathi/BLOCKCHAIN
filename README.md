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

#HYPERLEDGER FABRIC PRACTICAL 
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


