# Universal Denomination sample cryptocurrency

A simple guide on how to create your own cryptocurrency in 13 steps.

## Easily Create your own Cryptocurrency on the Ethereum network

1. Get metamask and log into the Rinkerby Testnet.

2. Go to https://www.rinkeby.io/#faucet and get some free testnet ether. You will need to post your public address to social media and then input the link into textbox on the page to get testnet ether. (All instructions are on the page)

3. Check your metamask account, it should now have some testnet ether in it.

4. Go to https://remix.ethereum.org and create a new file called MyTokenName.sol (Insert what ever you want your token to be called before the .sol)

5. Copy the contents of UniversalDenomination.sol from this repo into your newly created file.

6. On line 11 Change 'UniversalDenomination' to your token name (No Spaces). The line will read sometihng like this after you have changed it:
```
contract MyTokenName is EIP20Interface {
```

7. Change the constructor on line 26 to have the name of your token.
```
 function MyTokenName(
 ```
 
 8. In remix, create a new file called EIP20Interface.sol and copy the contents of the same file in this repo into your new file.
 
 9. On the right hand side of your remix window click 'Compile' for both files that you have created. 
 
 10. In Remix, click the run tab and ensure the 'Environment' is set to 'Injected Web3' and change the drop down next to the deploy button to the name of your token.
 
 11. Fill in the required parameters that you need to deploy your token, this takes the form: 
 _initialAmount, _tokenName, _decimalUints, _tokenSymbol. 
 So in the text box next to the deploy button you will end up with something like this: 
 
 1000000, "MyTokenName, 18, "MTN"
 
 12. Click Deploy and a metamask window will open, Click Submit and you will see on the right hand side you will have 1 pending transaction as the contract deploys to the testnet 
 
 13. Now copy your newly created contract address and paste it into https://rinkeby.etherscan.io/tokens and your new token with all of its details will be displayed.
 
 14. Congratulations, you just created a cryptocurrency. 
