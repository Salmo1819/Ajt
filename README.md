pragma solidity ^0.8.2;
import "./ERC20Standard.sol";
contract AJTtoken is ERC20Standard {
	constructor() public {
		totalSupply = 123;
		name = "Alvinjade token";
		decimals = 4;
		symbol = "AJT";
		version = "1.0";
		balances[msg.sender] = totalSupply;
	}
}
