# Deploying, Minting and Transfering tokens on the swisstronik network

The contract has been deployed to address 0x164271f32089B5E53D57c7Bd70Ba07143e237A18 on the swisstronik network.
1000 tokens have been minted from the mint.js file under scripts.
1 token has been sent to 0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1 to test on the success of the transfer


To run the project:

```open shell or cmd and run
mkdir Tokenfolder
cd Tokenfolder
mkdir hardhat
cd hardhat
npm init --yes #to initialise project
npm install --save-dev @nomicfoundation/hardhat #to install hardhat
npx hardhat #to complete the project setup
npm i @swisstronik/swisstronik.js #to install swisstronik sdk
npm i @openzeppelin/contracts dotenv

.....Then copy the code and try testing to see if all corresponds and works in sync...
Then in shell run
npx hardhat compile
npx hardhat run scripts/deploy.js --network swisstronik
#This will produce the deployment address to your console which you will use in mint.js and transfer.js
#Yiu can mint by running
npx hardhat run scripts/mint.js --network swisstronik
#You can transfer tokens on the network by running
npx hardhat run scripts/transfer.js

```
