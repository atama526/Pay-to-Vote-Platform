# Pay-to-Vote-Platform
Dapp where users can contribute ropsten eth to try to be the winner of a voting contest at the current time. At any given time, the current winner is the user who has paid the most ropsten eth. Users can contribute multiple times and their vote at any given time is the total of all of their contributions.

![Algorithm schema](./PayToVote_Home.PNG)

## How it works?

Using Infura provider, the front end connects with the Ropsten test Ethereum Network, allowing users to send ether to the contract to be the winner of the vote.
- Using the Dapp front end you will be able to see the current winners of the vote, also your own account details (Address, name, balance). You have the option to set your name so it´s linked to your address and finally you can also check the transactions you have sent to the smart contract with a link to etherscan info.  

### code by folder

- **contract:** - Folder Includes - Solidity Smart Contract, contract byteCode and ABI, Web3 instance of the contract and Tests using Hardhat & chai.
- **express:** - Express API routes and server configuration
- **lib:** - Mongo DB config - Calls to the DB
- **next:** - Folder includes - *Application Pages: Index, Enter, Address - *Layout Components - Styling and utils


### How to use it? 

- Access: https://alejandro-trial-project.tk.co/
- Database data API: https://alejandro-trial-project.tk.co/express/

In order to use the app you must have a Metamask account with ether on Ropsten test network 
http://www.herongyang.com/Ethereum/MetaMask-Extension-Add-Ropsten-Test-Network.html
 
### Dependencies

This project used the following technologies: 

- React + Next.js for the frontend [React Tutorial](https://reactjs.org/tutorial/tutorial.html) - [Next tutorial](https://nextjs.org/learn/basics/create-nextjs-app)
- [Tailwinds CSS](https://tailwindcss.com/) for styling
- Express for API endpoints
    - [Express “hello world” example](https://expressjs.com/en/starter/hello-world.html)
- MongoDB for data storage
    - [Usage examples](https://www.mongodb.com/docs/drivers/node/current/usage-examples/) — categorized by type of operation
- Web3.js, Ethers.js, and [useDapp](https://usedapp-docs.netlify.app/docs) for Web3 integration
- [mongo-express](https://github.com/mongo-express/mongo-express) for admin database viewing
- Nginx to serve everything over SSL
- Docker & docker-compose for environment management
- Python 3 for tooling scripts (local run, deployment, test kickoffs)
- [Mocha](https://mochajs.org/) for automated testing
- Solidity for smart contracts
    - [Solidity by example](https://docs.soliditylang.org/en/latest/solidity-by-example.html)
- [Hardhat](https://hardhat.org/) for smart contract deployments
    - [Hardhat - getting started](https://hardhat.org/getting-started/)

### Project Building sequence
```
 1. Smart Contract: Solidity - test- deployment
 2. Proyect infra - Web3, contract instance, Docker setup.
 3. Next Pages implementation: web3 functions, fetching and storing data, MongoDB, API, error handling, etc.
 4. Tailwinds CSS styling
 5. Bugs & Errors fixing
 6. Deployment

