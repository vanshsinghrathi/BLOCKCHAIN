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
'''sudo apt install golang-go'''
Installs Golang, which is necessary for running Hyperledger Fabric binaries.
![IMG-20250410-WA0029](https://github.com/user-attachments/assets/9e5cbeb1-5188-4964-afd4-069cd9876f22)
2. Check Docker version
   '''docker --version'''
   Verifies that Docker is installed and running correctly.

   ![IMG-20250410-WA0030](https://github.com/user-attachments/assets/67e06341-ac4e-4cf9-a765-d27f49f45cb1)

3. Check Docker compose version
'''docker -compose  --version
Verifies the installation of Docker Compose.
![IMG-20250410-WA0037](https://github.com/user-attachments/assets/50f1494c-ac9a-4790-bc3e-bce1bed9d2c1)


4. List Files in current dictionary
   ''' is '''
   Shows the list of files and folders in the current directory.

5. Clone the Fabric Samples Repository and Move into the Cloned Folder

'''git clone https://github.com/Akshitakaushik123/fabric-samples.git; cd fabric-samples'''

Downloads the official Hyperledger Fabric sample code from GitHub. Enters the cloned folder where Fabric examples are available.


![IMG-20250410-WA0038](https://github.com/user-attachments/assets/e2dea4c9-906c-4706-ab73-0939bda4e1a5)

6. Download Fabric Binaries
 '''  curl -sSL https://bit.ly/2ysbOFE | bash -s'''


Downloads necessary Fabric binaries and Docker images like peer, orderer, and cryptogen.

![IMG-20250410-WA0039](https://github.com/user-attachments/assets/b9e727c2-dff7-4699-9b09-4be31597d665)


7.Enter the Test Network Directory

'''cd test-network''''
Navigates to the directory that contains scripts for running a sample Fabric network.

![IMG-20250410-WA0040](https://github.com/user-attachments/assets/50f94f69-874d-4017-9171-d0eca95c7660)

8. View the Network Script
'''./network.sh'''
Shows the options available with the network.sh script.


9. Start the Fabric Network
'''./network.sh up'''
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.

![IMG-20250410-WA0041](https://github.com/user-attachments/assets/d08c71dc-640c-42a7-bfb4-220f370aa317)

10.Create a Channel
'''./network.sh createChannel'''
Creates a default channel (usually named mychannel) and joins the peers to it.


![IMG-20250410-WA0042](https://github.com/user-attachments/assets/8f87dc9d-9e5c-4db2-abb3-616f1c8539d8)
11. Shut Down the Network
'''./network.sh down'''
Stops all containers and deletes the crypto material and artifacts created during the setup.

![IMG-20250410-WA0045](https://github.com/user-attachments/assets/838ecc92-1584-4215-8e6e-f6ef6e399f08)

