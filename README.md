# Learning-Solidity

// SPDX-License-Identifier: MIT
pragma solidity 0.8.7;

// contract HelloWorld{
//     string public myString = "hello World";
// }

//DATA TYPES
// contract ValueTypes{
//     bool public b = true;
//     uint public u = 123; //greater than zero but cannot be -ve
//     //uint == uint256 0 to 2**256 -1
//     //        uint8 0 to 2**8 -1
//     //        uint16 0 to 2**16 -1
//     int public i = -132; //can be -ve  int == int256  -2**255 to 2**255-1

//     //to find min and max value of integer

//     int public minInt = type(int).min;
//     int public maxInt = type(int).max;

//     //address data type

//     address public addr = 0xB4Ad5c5b026A711C14499CD4764101657b566086;
//     bytes32 public b32 = 0x7465737400000000000000000000000000000000000000000000000000000000;
// }

//Functions
// contract funcIntr{
//     //external means when we deploy the contract we will be able to call this function
//     //pure means this function is read-only(will not wrtie on the blockchain)
//     function add(uint x, uint y)external pure returns (uint){
//         return x+y;
//     }

// }

// contract GlobalVar{
//     //view is also read-only view functions can read data from state and global variables
//     //msg.sender gives address of the user calling the function
//     //block.timestamp stores the time when that function is called
//     //block.number returns the value of block number
//     function globalVars() external view returns (address, uint, uint) {
//         address sender = msg.sender;
//         uint timeStamp = block.timestamp;
//         uint blockNum = block.number;
//         return(sender, timeStamp, blockNum);
//     }
// }

// contract ViewAndPureFunctions {
//     //both are read-only functions(getters)
//     //diff between view and pure
//     // view function : can read data from the blockchain, state variable or smartcontract
//     // pure functions : cannot read data from blockchain.

//     uint public num; //this variable will be saved on the blockchain

//     function viewFunc() external view returns (uint){
//         return num;
//     }

//     function purefunc(uint x) external pure returns (uint){
//         return x;
//     }

//     //this is a view function as it is reading data from the blockchain
//     function addToNum(uint x) external view returns(uint){
//         return num + x;
//     }

//     function add(uint x, uint y) external pure returns(uint){
//         return y + x;
//     }

// }
