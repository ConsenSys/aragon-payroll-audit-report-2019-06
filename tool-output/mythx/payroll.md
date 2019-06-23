```console
$ mythos analyze Payroll_flat.sol Payroll

Compiling with Solidity version: v0.4.24+commit.e67f0147

UUID: c73a8079-8223-4552-b0a6-34cb5740bb1e
API Version: v1.4.23
Harvey Version: 0.0.27
Maestro Version: 1.2.16
Maru Version: 0.4.8
Mythril Version: 0.21.2

Report found: 43 issues
Covered instructions: 0
Covered paths: 0
Selected compiler version: vUnknown

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

Payroll_flat.sol 285:15
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 867:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 68:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 86:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 111:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 149:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 252:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 272:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 322:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 383:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 410:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 424:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 461:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 494:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 536:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 551:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 578:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 737:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 794:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 808:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 835:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 51:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 977:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 1047:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 1067:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 1144:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 1214:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.18" are allowed.
Source code:

Payroll_flat.sol 1280:0
--------------------------------------------------
pragma solidity ^0.4.18;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

Payroll_flat.sol 8:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_SUB_UNDERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_SUB_UNDERFLOW" in contract "SafeMath8".
Source code:

Payroll_flat.sol 1153:4
--------------------------------------------------
string private constant ERROR_SUB_UNDERFLOW = "MATH64_SUB_UNDERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT64" in contract "Uint256Helpers" shadows another state variable with the same name "MAX_UINT64" in contract "Finance".
Source code:

Payroll_flat.sol 256:4
--------------------------------------------------
uint256 private constant MAX_UINT64 = uint64(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_ADD_OVERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_ADD_OVERFLOW" in contract "SafeMath64".
Source code:

Payroll_flat.sol 1075:4
--------------------------------------------------
string private constant ERROR_ADD_OVERFLOW = "MATH_ADD_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_SUB_UNDERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_SUB_UNDERFLOW" in contract "SafeMath64".
Source code:

Payroll_flat.sol 1076:4
--------------------------------------------------
string private constant ERROR_SUB_UNDERFLOW = "MATH_SUB_UNDERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_MUL_OVERFLOW" in contract "SafeMath" shadows another state variable with the same name "ERROR_MUL_OVERFLOW" in contract "SafeMath64".
Source code:

Payroll_flat.sol 1077:4
--------------------------------------------------
string private constant ERROR_MUL_OVERFLOW = "MATH_MUL_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_DIV_ZERO" in contract "SafeMath" shadows another state variable with the same name "ERROR_DIV_ZERO" in contract "SafeMath64".
Source code:

Payroll_flat.sol 1078:4
--------------------------------------------------
string private constant ERROR_DIV_ZERO = "MATH_DIV_ZERO"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_ADD_OVERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_ADD_OVERFLOW" in contract "SafeMath8".
Source code:

Payroll_flat.sol 1152:4
--------------------------------------------------
string private constant ERROR_ADD_OVERFLOW = "MATH64_ADD_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_VAULT_NOT_CONTRACT" in contract "VaultRecoverable" shadows another state variable with the same name "ERROR_VAULT_NOT_CONTRACT" in contract "Finance".
Source code:

Payroll_flat.sol 749:4
--------------------------------------------------
string private constant ERROR_VAULT_NOT_CONTRACT = "RECOVER_VAULT_NOT_CONTRACT"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_MUL_OVERFLOW" in contract "SafeMath64" shadows another state variable with the same name "ERROR_MUL_OVERFLOW" in contract "SafeMath8".
Source code:

Payroll_flat.sol 1154:4
--------------------------------------------------
string private constant ERROR_MUL_OVERFLOW = "MATH64_MUL_OVERFLOW"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_DIV_ZERO" in contract "SafeMath64" shadows another state variable with the same name "ERROR_DIV_ZERO" in contract "SafeMath8".
Source code:

Payroll_flat.sol 1155:4
--------------------------------------------------
string private constant ERROR_DIV_ZERO = "MATH64_DIV_ZERO"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "ERROR_TOKEN_TRANSFER_FROM_REVERTED" in contract "Vault" shadows another state variable with the same name "ERROR_TOKEN_TRANSFER_FROM_REVERTED" in contract "Finance".
Source code:

Payroll_flat.sol 1325:4
--------------------------------------------------
string private constant ERROR_TOKEN_TRANSFER_FROM_REVERTED = "VAULT_TOKEN_TRANSFER_FROM_REVERT"
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT256" in contract "Finance" shadows another state variable with the same name "MAX_UINT256" in contract "Payroll".
Source code:

Payroll_flat.sol 1442:4
--------------------------------------------------
uint256 internal constant MAX_UINT256 = uint256(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: State variable shadows another state variable.
Description: The state variable "MAX_UINT64" in contract "Finance" shadows another state variable with the same name "MAX_UINT64" in contract "Payroll".
Source code:

Payroll_flat.sol 1443:4
--------------------------------------------------
uint64 internal constant MAX_UINT64 = uint64(-1)
--------------------------------------------------

==================================================

Title: (SWC-119) Shadowing State Variables
Severity: Low
Head: Local variable shadows a state variable.
Description: The local variable "vault" in contract "VaultRecoverable" shadows the state variable with the same name "vault" in contract "Finance".
Source code:

Payroll_flat.sol 759:8
--------------------------------------------------
address vault
--------------------------------------------------

==================================================

Done
