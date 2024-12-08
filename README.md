# Missing Input Validation in add Function

This repository demonstrates a common bug in Solidity: missing input validation. The `add` function does not check if the inputs are numbers, which can lead to unexpected behavior or errors.

## Bug

The `add` function in `bug.sol` does not perform any input validation.  If non-numeric values are passed, the function will fail silently or produce unexpected results.

## Solution

The `bugSolution.sol` file provides a corrected version of the `add` function. It includes checks to ensure both inputs are of the correct type before performing the addition.  It reverts the transaction if invalid inputs are provided, enhancing the robustness of the smart contract.