# MetaCrafters

## Integrating Smart Contracts with a Frontend Application
This project showcases the seamless integration of a smart contract with a frontend application using cutting-edge technologies like Ethereum, React, and Hardhat.

## Smart Contract Details
The smart contract, **Assessment.sol**, is at the heart of this project. It enables users to set and retrieve a naming message, providing a simple yet effective demonstration of smart contract functionality.

## Frontend Interaction
The React-based frontend application is designed to interact with the deployed smart contract, offering two primary features:
- Fetching the current naming message.
- Setting a new naming message.

## Prerequisites
- Node.js
- MetaMask extension for your browser

## Getting Started

### 1. Clone the Repository:
Begin by cloning the project repository to your local machine:
```bash
git clone <repository-url>
```

### 2. Install Dependencies:
Navigate to the project directory and install the required dependencies:
```bash
cd <project-directory>
npm install
```

### 3. Start a Local Ethereum Network:
Launch a local Ethereum network using Hardhat:
```bash
npx hardhat node
```
Keep note of the network URL provided, as you'll need it to configure MetaMask in the next step.

### 4. Configure MetaMask:
1. Install the MetaMask extension in your browser and set up a new Ethereum network using the URL from the local Hardhat network.
2. Import an account from the local Hardhat network into MetaMask.

### 5. Deploy the Smart Contract:
Deploy the **Assessment.sol** smart contract to your local network with the following command:
```bash
npx hardhat run scripts/deploy.js --network localhost
```
Ensure your local Ethereum network is running before executing the deployment.

### 6. Update Frontend Configuration:
In the `index.js` file, replace the `nameAddress` variable with the contract address obtained after deployment.

### 7. Start the Frontend Development Server:
Run the frontend server to view your application:
```bash
npm run dev
```
Access the application by navigating to `http://localhost:3000` in your browser.

## Usage Guide
- **View Current Naming:** The main page will display the current naming message retrieved from the smart contract.
- **Set New Naming:** Enter a new naming message and click "Set naming." Ensure your MetaMask account connected to the local network has sufficient funds. The new message will be stored on the blockchain and displayed on the page.

## Resources
- Ethereum
- React
- Hardhat
- MetaMask

## Author
**Himanshu Rajak**

## License
This project is licensed under the MIT License. See the [LICENSE]() file for more information.