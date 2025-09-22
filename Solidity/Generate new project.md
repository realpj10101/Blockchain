1-Install Foundry 

```bash
curl -L https://foundry.paradigm.xyz | bash
foundryup
```

Foundry => Tool for solidity contracts

When you install **foundryup** it gives you three main tools
1- **forge** => For build, test and manage solidity projects
2- **cast** => For working with network and contracts from command line 
3- **anvil** => Local blockchain for test and develop

2- Create new project

```bash
forge init <project-name>
```

3- Run the project
```bash
cd <project-name>
forge build 
```


1- Contracts in solidity(Like class in C#)
```solidity
contract <Name> [is <Parent>] {
    // variables + functions
}
```

contract -> Fixed keyword
Name -> Contract name
[is  Parent] -> Optional, inherit from other contract/interface

```solidity
contract Person is Human {
    // ...
}
```

2- Variable 
```solidity
<type> [visibility] [constant|immutable] <name> [= initialValue];
```

type -> type of data (string, unit256)
visibility -> Optional, for states (public, private, internal)
constant|immutable -> Optional, If is fixed
name -> variable name
initial value 

3- function
```solidity
function <name>(params) <modifiers/visibility> [returns(...)] { ... }
```

```solidity
function add(uint256 a, uint256 b) public pure returns (uint256) {
    return a + b;
}

function deposit() external payable { ... }

function getOwner() public view returns (address) {
    return owner;
}
```


