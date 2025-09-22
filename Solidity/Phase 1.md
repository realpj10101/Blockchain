
# Solidity Basics

First train: (calculator)
	Create a contract which has:
	has a function  add(uint256 a, uint256 b) 
	save the sun result on state variable
	publish event named 


``` solidity
// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.13;

contract Calculator {
    uint256 public lastResult;

    event SumCalculated(uint256 result);

    function add(uint256 a, uint256 b) public {
        lastResult = a + b;
        emit SumCalculated(lastResult);
    }

    function getLastResult() public view returns (uint256) {
        return lastResult;
    }
}
```

```solidity
// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.13;

import "forge-std/Test.sol";
import "../src/Calculator.sol";

contract CalculatorTest is Test {
    Calculator calc;

    function setUp() public {
        calc = new Calculator();
    }

    function testAdd() public {
        calc.add(2, 3);
        assertEq(calc.getLastResult(), 5);
    }
}
```