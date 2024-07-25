# Swisstronik-ERC20

### 1. Install Dependency and Clone File

git clone https://github.com/zerosecxz/Swisstronik-ERC20.git

```bash
npm install
```

### 2. Set .env File

create .env file in root project

```bash
PRIVATE_KEY="your private key"
```

### 3. Create Smart Contract

- Open contract folder
- Create Token.sol file
- Copy this code and paste there

```bash
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract TestToken is ERC20 {
    constructor()ERC20("IzzyToken","IZZY"){}

    function mint1000tokens() public {
        _mint(msg.sender,1000*10**18);
    }

    function burn1000tokens() public{
        _burn(msg.sender,1000*10**18);
    }

}
```

### 5. Compile Smart Contract

```bash
npm run compile
```

### 6. Deploy Smart Contract

```bash
npm run deploy
```

### 6 Mint, Check and Transfer Token

```bash
npm run mint

Check Supply
npm run check-supply

Check Balance
npm run balance-of

Tranfer Token
npm run transfer
```
### 6 Finish

Feel free for Donate me :) 
0xfE7e5bd620d959590c8ea99c6Cc390C5a66cC566


