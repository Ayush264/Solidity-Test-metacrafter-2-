# Solidity-Test-metacrafter-2-
This solidity program "token.sol" is a simple program which imitates the token creation with 3 variables and (minting and burning coins) process on my local Blockchain with remix IDE.

### DESCRIPTION
## MyToken Smart Contract

This Solidity smart contract implements a basic token with minting and burning capabilities. Below is a detailed description of the components and functionality provided by this contract.

### Components

1. **Public State Variables**:
    - **token_Name**: Holds the name of the token, which is set to "CHOOTA BHEEM".
    - **token_Abbrvtn**: Stores the abbreviation of the token, "CB".
    - **totalSupply**: Tracks the total number of tokens in circulation.

2. **Mapping**:
    - **map_balances**: Associates each address with its corresponding token balance. This allows the contract to keep track of how many tokens each address owns.

### Functions

1. **Mint Function**: `mintToken(address t_address, uint t_value)`
    - **Purpose**: To create new tokens and assign them to a specified address.
    - **Parameters**:
        - `t_address`: The address to which the new tokens will be credited.
        - `t_value`: The number of tokens to be created.
    - **Operation**:
        - Increases `totalSupply` by `t_value`.
        - Increments the balance of `t_address` by `t_value`.

2. **Burn Function**: `burnToken(address t_address, uint t_value)`
    - **Purpose**: To destroy tokens from a specified address, reducing the total supply.
    - **Parameters**:
        - `t_address`: The address from which tokens will be deducted.
        - `t_value`: The number of tokens to be burned.
    - **Operation**:
        - Checks if `t_address` has at least `t_value` tokens.
        - If the balance is sufficient, decreases `totalSupply` by `t_value`.
        - Decrements the balance of `t_address` by `t_value`.
     
          ## Executing  Program

To run the MyToken smart contract, visit [Remix Ethereum](https://remix.ethereum.org/), create a new file named `MyToken.sol`, and paste the contract code. Then, compile and deploy the contract using the "Solidity Compiler" and "Deploy & Run Transactions" tabs.
![image](https://github.com/Ayush264/Solidity-Test-metacrafter-2-/assets/121258575/af65df47-b175-402d-b851-0ad2b2bc678d)

  -After deployment, we can interact with program by calling the functions that will appear on the left as shown in the above image.
