Steps to make web3.0 app
firstly install truffle globally by writing npm install -g truffle@version

then write truffle init in terminal to create a project
then make package.json and add dependency then run command npm install in terminal

then make a file in contracts folder by any name for example todolist.sol
,then import solidity by writing `pragram solidity@version`

then, write contract classname{
    // CODE BODY
}

to compile your program to test write 
truffle compile in terminal

then check truffle-config.js file and change to this one ->
module.exports = {
  networks: {
    development: {
     host: "127.0.0.1",     // Localhost (default: none)
     port: 7545,            // Standard Ethereum port (default: none)
     network_id: "*",       // Any network (default: none)
    },
    solc: {
       optimizer: {
         enabled: false,
         runs: 200
       }
    } 
  }
}


now lets create a migration file in order to get the smart contract in the blockchain so
go to migrations folder and make this file in it` 2_deploy_contracts.js` 

