## SwapNexus

SwapNexus is a robust cross chain token transfer platform, which is based on ICP (Internet Computer Protocol) blockchain. It allows for cross chain transfer of ICP based tokens. 
Our platform allows to seamlessly swap between a user's tokens, based on the ongoing market rate. 

First, the user specifies the allowance, i.e., the maximum amount of tokens that can be transferred. This ensures that no more than an amount pre defined by the user can be transferred. On the main page, the user can link his **Plug Wallet** in which he has some tokens on different ICP chains. Once he enters the amount of one token, we automatically calculate the amount of the second token, based on the current conversion rate. The tranfer process involves two major steps- 

- **Burn** - When the user enters the amount of the first token and clicks on swap, the tokens on the first blockchain are burnt, i.e., the amount is debited from his account and credited to a special account, called the minter account. The minter account is a special account, which has infinite number of tokens, and acts as the bridge between the two blockchains.

- **Mint** - Minting means to create (mint) new currency in the second blockahin, effectively implemented by the transfer of converted tokens from the minter account to the same user's account on the second blockhain.

This mechanism ensures that the data is decentralized, and the host website does not hold the rights of changing the policies or accessing other information. This is implemented through Motoko programming language, on which we implement the logic for burning and minting the tokens.
