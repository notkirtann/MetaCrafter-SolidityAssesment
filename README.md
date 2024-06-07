<h1> Solidity Assessment </h1>
This Solidity program is a "My Token" program in which we create a token which can be used to visualise how we can use Solidity programming language to create a TOKEN in real life. This can also be used in Ethereum. The purpose of the program is for those who are relatively new to Blockchain and want to get a feel of how it works. Ethereum which is based on Blockchain can be programmed using Solidity.

<h2> Description </h2>
This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. This program has two functions. "mint" function will store and increase the value of tokens and add it to balances. "burn" function will do the opposite and will deduct the value from the balances of respective tokens. This program serves as a simple and straightforward introduction to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

<h3>Getting started</h3>
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/. Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension. In thi scase it's myToken.sol. A code will be written which can be found inside myToken.sol file. To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile myToken.sol" button.

### Working
Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button. Once the contract is deployed, you can interact with it by calling the mint and burn function. Click on the "MyToken" contract in the left-hand sidebar, and then click on the "mint" function. Finally, click on the "transact" button to execute the function and add values to the mint function. The outsatnding balance can be checked using _balances. The same can be done for burn function where we can decrease the total balance of the tokens according to the value specified by the user.

<h3>CODE EXPLANATION</h3>
    1. I created contract having public variables that store the details about our coin (Token Name, Token Abbrv., Total Supply)
    2. Then in contract i created a mapping of addresses to balances (address => uint)
    3. Then crated mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Then created a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly i used ef else condition, so that burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.

## Author
Metacrafter : Kirtan Nahar

