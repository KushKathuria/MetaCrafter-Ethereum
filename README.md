Public State Variables:

token_Name: Holds the name of the token, which is set to "AlphaBeta".
token_Abbrvtn: Stores the abbreviation of the token, "AB".
totalSupply: Tracks the total number of tokens in circulation.
Mapping:

map_balances: Associates each address with its corresponding token balance. This allows the contract to keep track of how many tokens each address owns.
Functions
Mint Function: mintToken(address t_address, uint t_value)

Purpose: To create new tokens and assign them to a specified address.
Parameters:
t_address: The address to which the new tokens will be credited.
t_value: The number of tokens to be created.
Operation:
Increases totalSupply by t_value.
Increments the balance of t_address by t_value.
Burn Function: burnToken(address t_address, uint t_value)

Purpose: To destroy tokens from a specified address, reducing the total supply.
Parameters:
t_address: The address from which tokens will be deducted.
t_value: The number of tokens to be burned.
Operation:
Checks if t_address has at least t_value tokens.

If the balance is sufficient, decreases totalSupply by t_value.

Decrements the balance of t_address by t_value.
