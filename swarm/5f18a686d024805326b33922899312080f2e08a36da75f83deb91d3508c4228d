// SPDX-License-Identifier: GPL-3.0

pragma solidity >=0.7.0 <0.9.0;
import "remix_tests.sol";
import "../contracts/AdventureTimeToken.sol";

contract AdventureTimeTokenTest is AdventureTimeToken {

    constructor() AdventureTimeToken(1000000) {}  // Inicializa el token con 1,000,000 de suministro inicial

    function testTokenInitialValues() public {
        Assert.equal(name(), "AdventureTimeToken", "Token name did not match");
        Assert.equal(symbol(), "ATIME", "Token symbol did not match");
        Assert.equal(decimals(), 18, "Token decimals did not match");
        Assert.equal(totalSupply(), 1000000 * (10 ** decimals()), "Token supply should match the initial supply");
    }
}
