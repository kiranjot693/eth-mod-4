# Eth-intermediate-module-4
*Aim of the Project*
Create an ERC20 token and deploy it on the Avalanche network for Degen Gaming. It consists of minting, burning, transferring, redeeming tokens, and checking the account balance.


*Logic of the code*

1. Write the license identifier and solidity version.

2. Import the open Zeppelin contracts and hardhat/console.sol dependencies.

3. Create a contract named as DegenToken which is Ownable and ERC20Burnable.

4. It consists of a constructor which defines the name and symbol of the token as "Degen Token" and "DGN " respectively.

5. The function mint_tokens consists of minting a specific amount to a particular address. It is declared public so that it can be accessed outside the contract.

6. The transfer_Token function takes the receiver's address and amount to be transferred as its parameters. It has a require statement that confirms that the balance of the sender should be greater than or equal to the amount to be transferred else the string message is returned. If the condition returns to true, then the approve  and transferFrom  function transfers the tokens(amount) from the sender to the receiver.

7. The getBalance function is declared external and returns the unsigned int value of the valance in the sender's account/address.

8. The burn_Tokens take the unsigned int value of the amount as its parameter. It is declared as external. The require statement checks that the balance of the sender should be greater than or equal to the amount to be transferred else the string message is returned. If the condition returns to the true, then the burn function burns the specific amount of tokens from the sender's account.

9. The redeem_Tokens is declared public and pure. It returns the five rewards(strings) which will be redeemed if the conditions are satisfied.

10. The user enters a particular number. The require statement checks that the entered number should be less than the total number of the choices provided, if yes then the condition matching with the choice is executed and that particular numbered reward is redeemed by paying the listed tokens.

*Functionality of the code*

1. Open the Remix IDE(https://remix.ethereum.org) and clone the repository provided in the module.

2. Open the contacts folder and write the above code.

3. Compile the DegenToken.sol contract.

4. In the deploy section, select Injected Provider environment which will help us to connect with the metamask.

5. Paste the address of the account currently running in the meta mask in the At Address section.

6. Open the deployed contract. Run different functions of minting, burning, transferring, redeeming tokens, and checking the account balance.

7. Verify the transactions by pasting the same address in the Snowtrace Testnet site.(https://testnet.snowtrace.io)

8. If all the tests are passed, then the contract has successfully followed every requirement of the project.
