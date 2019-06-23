```console
$ mythos analyze PayrollKit_flat.sol PayrollKit

Compiling with Solidity version: v0.4.24+commit.e67f0147

UUID: 0fe55936-2247-4604-84e5-05b1f7d2abb4
API Version: v1.4.23
Harvey Version: 0.0.27
Maestro Version: 1.2.16
Maru Version: 0.4.8
Mythril Version: 0.21.2

Report found: 110 issues
Covered instructions: 0
Covered paths: 0
Selected compiler version: vUnknown

Title: (SWC-111) Use of Deprecated Solidity Functions
Severity: Medium
Head: Use of disallowed keyword "var".
Description: Keyword "var" is disallowed as of Solidity version 0.5.0, it is not possible anymore to create variable declarations without static types.
Source code:

PayrollKit_flat.sol 2378:8
--------------------------------------------------
var previousBalanceFrom = balanceOfAt(_from, block.number)
--------------------------------------------------

==================================================

Title: (SWC-111) Use of Deprecated Solidity Functions
Severity: Medium
Head: Use of disallowed keyword "var".
Description: Keyword "var" is disallowed as of Solidity version 0.5.0, it is not possible anymore to create variable declarations without static types.
Source code:

PayrollKit_flat.sol 2392:8
--------------------------------------------------
var previousBalanceTo = balanceOfAt(_to, block.number)
--------------------------------------------------

==================================================

Title: (SWC-111) Use of Deprecated Solidity Functions
Severity: Medium
Head: Use of disallowed keyword "var".
Description: Keyword "var" is disallowed as of Solidity version 0.5.0, it is not possible anymore to create variable declarations without static types.
Source code:

PayrollKit_flat.sol 4449:8
--------------------------------------------------
var subnode = keccak256(node, label)
--------------------------------------------------

==================================================

Title: (SWC-111) Use of Deprecated Solidity Functions
Severity: Medium
Head: Use of disallowed keyword "var".
Description: Keyword "var" is disallowed as of Solidity version 0.5.0, it is not possible anymore to create variable declarations without static types.
Source code:

PayrollKit_flat.sol 4621:8
--------------------------------------------------
var record = records[node]
--------------------------------------------------

==================================================

Title: (SWC-118) Incorrect Constructor Name
Severity: Medium
Head: Potential incorrect constructor name "ENS".
Description: Until Solidity version 0.4.21 a constructor can only be defined as a function that has the same name as the contract "ENS". It has been found that there is a function with a very similar name "ENS" that only deviates based lower/upper case characters.
Source code:

PayrollKit_flat.sol 4405:4
--------------------------------------------------
function ENS() public {
        records[0].owner = msg.sender;
    }
--------------------------------------------------

==================================================

Title: (SWC-118) Incorrect Constructor Name
Severity: Medium
Head: Potential incorrect constructor name "Controlled".
Description: Until Solidity version 0.4.21 a constructor can only be defined as a function that has the same name as the contract "Controlled". It has been found that there is a function with a very similar name "Controlled" that only deviates based lower/upper case characters.
Source code:

PayrollKit_flat.sol 2220:4
--------------------------------------------------
function Controlled()  public { controller = msg.sender;}
--------------------------------------------------

==================================================

Title: (SWC-118) Incorrect Constructor Name
Severity: Medium
Head: Potential incorrect constructor name "MiniMeToken".
Description: Until Solidity version 0.4.21 a constructor can only be defined as a function that has the same name as the contract "MiniMeToken". It has been found that there is a function with a very similar name "MiniMeToken" that only deviates based lower/upper case characters.
Source code:

PayrollKit_flat.sol 2306:4
--------------------------------------------------
function MiniMeToken(
        MiniMeTokenFactory _tokenFactory,
        MiniMeToken _parentToken,
        uint _parentSnapShotBlock,
        string _tokenName,
        uint8 _decimalUnits,
        string _tokenSymbol,
        bool _transfersEnabled
    )  public
    {
        tokenFactory = _tokenFactory;
        name = _tokenName;                                 // Set the name
        decimals = _decimalUnits;                          // Set the decimals
        symbol = _tokenSymbol;                             // Set the symbol
        parentToken = _parentToken;
        parentSnapShotBlock = _parentSnapShotBlock;
        transfersEnabled = _transfersEnabled;
        creationBlock = block.number;
    }
--------------------------------------------------

==================================================

Title: (SWC-118) Incorrect Constructor Name
Severity: Medium
Head: Potential incorrect constructor name "PublicResolver".
Description: Until Solidity version 0.4.21 a constructor can only be defined as a function that has the same name as the contract "PublicResolver". It has been found that there is a function with a very similar name "PublicResolver" that only deviates based lower/upper case characters.
Source code:

PayrollKit_flat.sol 4528:4
--------------------------------------------------
function PublicResolver(AbstractENS ensAddr) public {
        ens = ensAddr;
    }
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2643:90
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2645:46
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2542:49
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 285:15
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2323:24
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2373:38
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2378:53
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2392:49
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2403:35
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PayrollKit_flat.sol 2464:29
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 794:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 808:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 835:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 867:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 977:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 1046:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 1123:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 2155:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 2185:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 2766:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 3248:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 3414:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 3951:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 4114:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.15" are allowed.
Source code:

PayrollKit_flat.sol 4352:0
--------------------------------------------------
pragma solidity ^0.4.15;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.0" are allowed.
Source code:

PayrollKit_flat.sol 4381:0
--------------------------------------------------
pragma solidity ^0.4.0;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.0" are allowed.
Source code:

PayrollKit_flat.sol 4479:0
--------------------------------------------------
pragma solidity ^0.4.0;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.18" are allowed.
Source code:

PayrollKit_flat.sol 4693:0
--------------------------------------------------
pragma solidity ^0.4.18;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 4705:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 5123:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 8:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 68:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 86:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 111:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 149:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 252:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 272:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 322:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 383:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 410:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 424:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 461:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 494:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 536:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 551:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 578:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 737:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PayrollKit_flat.sol 51:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-107) Reentrancy
Severity: Low
Head: The contract executes an external message call.
Description: An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.
Source code:

PayrollKit_flat.sol 6073:19
--------------------------------------------------
repo.getLatest()
--------------------------------------------------

==================================================

Title: (SWC-107) Reentrancy
Severity: Low
Head: The contract executes an external message call.
Description: An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.
Source code:

PayrollKit_flat.sol 6072:25
--------------------------------------------------
PublicResolver(ens.resolver(appId)).addr(appId)
--------------------------------------------------

==================================================

Title: (SWC-107) Reentrancy
Severity: Low
Head: The contract executes an external message call.
Description: An external function call to a fixed contract address is executed. Make sure that the callee contract has been reviewed carefully.
Source code:

PayrollKit_flat.sol 6072:40
--------------------------------------------------
ens.resolver(appId)
--------------------------------------------------

==================================================

Title: (SWC-109) Uninitialized Storage Pointer
Severity: Low
Head: Dangerous use of uninitialized storage variables.
Description: Uninitialized storage variables of user-defined type can point to unexpected storage locations. Initialize variable "finance" or set the storage attribute "memory".
Source code:

PayrollKit_flat.sol 6122:8
--------------------------------------------------
Finance finance
--------------------------------------------------

==================================================

Title: (SWC-109) Uninitialized Storage Pointer
Severity: Low
Head: Dangerous use of uninitialized storage variables.
Description: Uninitialized storage variables of user-defined type can point to unexpected storage locations. Initialize variable "vault" or set the storage attribute "memory".
Source code:

PayrollKit_flat.sol 6121:8
--------------------------------------------------
Vault vault
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "records" in contract "ENS" shadows another state variable with the same name "records" in contract "PublicResolver".
Source code:

PayrollKit_flat.sol 4394:4
--------------------------------------------------
mapping(bytes32=>Record) records
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_ADD_OVERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_ADD_OVERFLOW" in contract "SafeMath64".
Source code:

PayrollKit_flat.sol 1054:4
--------------------------------------------------
string private constant ERROR_ADD_OVERFLOW = "MATH_ADD_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_MUL_OVERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_MUL_OVERFLOW" in contract "SafeMath64".
Source code:

PayrollKit_flat.sol 1056:4
--------------------------------------------------
string private constant ERROR_MUL_OVERFLOW = "MATH_MUL_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_DIV_ZERO" in contract "SafeMath" shadows another state variable with the same name "ERROR_DIV_ZERO" in contract "SafeMath64".
Source code:

PayrollKit_flat.sol 1057:4
--------------------------------------------------
string private constant ERROR_DIV_ZERO = "MATH_DIV_ZERO"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_ADD_OVERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_ADD_OVERFLOW" in contract "SafeMath8".
Source code:

PayrollKit_flat.sol 1131:4
--------------------------------------------------
string private constant ERROR_ADD_OVERFLOW = "MATH64_ADD_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_SUB_UNDERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_SUB_UNDERFLOW" in contract "SafeMath8".
Source code:

PayrollKit_flat.sol 1132:4
--------------------------------------------------
string private constant ERROR_SUB_UNDERFLOW = "MATH64_SUB_UNDERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_MUL_OVERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_MUL_OVERFLOW" in contract "SafeMath8".
Source code:

PayrollKit_flat.sol 1133:4
--------------------------------------------------
string private constant ERROR_MUL_OVERFLOW = "MATH64_MUL_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_DIV_ZERO" in contract "SafeMath64" shadows another state variable with the same name "ERROR_DIV_ZERO" in contract "SafeMath8".
Source code:

PayrollKit_flat.sol 1134:4
--------------------------------------------------
string private constant ERROR_DIV_ZERO = "MATH64_DIV_ZERO"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_TOKEN_TRANSFER_FROM_REVERTED" in contract "Vault" shadows another state variable with the same name "ERROR_TOKEN_TRANSFER_FROM_REVERTED" in contract "Finance".
Source code:

PayrollKit_flat.sol 1226:4
--------------------------------------------------
string private constant ERROR_TOKEN_TRANSFER_FROM_REVERTED = "VAULT_TOKEN_TRANSFER_FROM_REVERT"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT256" in contract "Finance" shadows another state variable with the same name "MAX_UINT256" in contract "Payroll".
Source code:

PayrollKit_flat.sol 1343:4
--------------------------------------------------
uint256 internal constant MAX_UINT256 = uint256(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT64" in contract "Finance" shadows another state variable with the same name "MAX_UINT64" in contract "Payroll".
Source code:

PayrollKit_flat.sol 1344:4
--------------------------------------------------
uint64 internal constant MAX_UINT64 = uint64(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "vault" in contract "VaultRecoverable" shadows the state variable with the same name "vault" in contract "Finance".
Source code:

PayrollKit_flat.sol 759:8
--------------------------------------------------
address vault
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "vault" in contract "PayrollKit" shadows the state variable with the same name "vault" in contract "Finance".
Source code:

PayrollKit_flat.sol 6121:8
--------------------------------------------------
Vault vault
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "vault" in contract "PayrollKit" shadows the state variable with the same name "vault" in contract "Finance".
Source code:

PayrollKit_flat.sol 6151:8
--------------------------------------------------
Vault vault
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "name" in contract "APMNamehash" shadows the state variable with the same name "name" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 3257:25
--------------------------------------------------
string name
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "name" in contract "PublicResolver" shadows the state variable with the same name "name" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 4607:35
--------------------------------------------------
string name
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "name" in contract "PayrollKit" shadows the state variable with the same name "name" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 6198:8
--------------------------------------------------
string name
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "name" in contract "PayrollKit" shadows the state variable with the same name "name" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 6227:22
--------------------------------------------------
string name
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "symbol" in contract "PayrollKit" shadows the state variable with the same name "symbol" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 6199:8
--------------------------------------------------
string symbol
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "symbol" in contract "PayrollKit" shadows the state variable with the same name "symbol" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 6227:35
--------------------------------------------------
string symbol
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "version" in contract "Repo" shadows the state variable with the same name "version" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 3365:8
--------------------------------------------------
Version storage version
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "version" in contract "Repo" shadows the state variable with the same name "version" in contract "MiniMeToken".
Source code:

PayrollKit_flat.sol 3392:33
--------------------------------------------------
uint16[3] version
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_AUTH_FAILED" in contract "AragonApp" shadows another state variable with the same name "ERROR_AUTH_FAILED" in contract "Kernel".
Source code:

PayrollKit_flat.sol 993:4
--------------------------------------------------
string private constant ERROR_AUTH_FAILED = "APP_AUTH_FAILED"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "SCRIPT_START_LOCATION" in contract "EVMScriptRegistry" shadows another state variable with the same name "SCRIPT_START_LOCATION" in contract "BaseEVMScriptExecutor".
Source code:

PayrollKit_flat.sol 4018:4
--------------------------------------------------
uint256 internal constant SCRIPT_START_LOCATION = 4
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_SUB_UNDERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_SUB_UNDERFLOW" in contract "SafeMath64".
Source code:

PayrollKit_flat.sol 1055:4
--------------------------------------------------
string private constant ERROR_SUB_UNDERFLOW = "MATH_SUB_UNDERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ens" in contract "PublicResolver" shadows another state variable with the same name "ens" in contract "KitBase".
Source code:

PayrollKit_flat.sol 4516:4
--------------------------------------------------
AbstractENS ens
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "ens" in contract "PayrollKit" shadows the state variable with the same name "ens" in contract "PublicResolver".
Source code:

PayrollKit_flat.sol 6101:16
--------------------------------------------------
ENS ens
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_CAN_NOT_FORWARD" in contract "TokenManager" shadows another state variable with the same name "ERROR_CAN_NOT_FORWARD" in contract "Payroll".
Source code:

PayrollKit_flat.sol 4759:4
--------------------------------------------------
string private constant ERROR_CAN_NOT_FORWARD = "TM_CAN_NOT_FORWARD"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "IVaultRecoverable" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 74:29
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "IVaultRecoverable" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 76:33
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "VaultRecoverable" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 767:12
--------------------------------------------------
ERC20 token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "VaultRecoverable" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 780:33
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "Finance" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 1751:12
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "Finance" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 1784:12
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "MiniMeToken" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 2696:8
--------------------------------------------------
MiniMeToken token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "Payroll" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 5804:12
--------------------------------------------------
address token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "PayrollKit" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 6206:8
--------------------------------------------------
MiniMeToken token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "token" in contract "PayrollKit" shadows the state variable with the same name "token" in contract "TokenManager".
Source code:

PayrollKit_flat.sol 6227:68
--------------------------------------------------
MiniMeToken token
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT64" in contract "Payroll" shadows another state variable with the same name "MAX_UINT64" in contract "PayrollKit".
Source code:

PayrollKit_flat.sol 5222:4
--------------------------------------------------
uint64 internal constant MAX_UINT64 = uint64(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "finance" in contract "PayrollKit" shadows the state variable with the same name "finance" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6122:8
--------------------------------------------------
Finance finance
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "finance" in contract "PayrollKit" shadows the state variable with the same name "finance" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6154:8
--------------------------------------------------
Finance finance
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "finance" in contract "PayrollKit" shadows the state variable with the same name "finance" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6168:8
--------------------------------------------------
Finance finance
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "finance" in contract "PayrollKit" shadows the state variable with the same name "finance" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6197:8
--------------------------------------------------
Finance finance
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "denominationToken" in contract "PayrollKit" shadows the state variable with the same name "denominationToken" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6116:8
--------------------------------------------------
MiniMeToken denominationToken
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "denominationToken" in contract "PayrollKit" shadows the state variable with the same name "denominationToken" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6169:8
--------------------------------------------------
MiniMeToken denominationToken
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "allowedTokens" in contract "PayrollKit" shadows the state variable with the same name "allowedTokens" in contract "Payroll".
Source code:

PayrollKit_flat.sol 6246:8
--------------------------------------------------
address[] memory allowedTokens
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_VAULT_NOT_CONTRACT" in contract "VaultRecoverable" shadows another state variable with the same name "ERROR_VAULT_NOT_CONTRACT" in contract "Finance".
Source code:

PayrollKit_flat.sol 749:4
--------------------------------------------------
string private constant ERROR_VAULT_NOT_CONTRACT = "RECOVER_VAULT_NOT_CONTRACT"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT64" in contract "Uint256Helpers" shadows another state variable with the same name "MAX_UINT64" in contract "Finance".
Source code:

PayrollKit_flat.sol 256:4
--------------------------------------------------
uint256 private constant MAX_UINT64 = uint64(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "tokenFactory" in contract "MiniMeToken" shadows another state variable with the same name "tokenFactory" in contract "PayrollKit".
Source code:

PayrollKit_flat.sol 2287:4
--------------------------------------------------
MiniMeTokenFactory public tokenFactory
--------------------------------------------------

==================================================

Done
```