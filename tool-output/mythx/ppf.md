```console
$ mythos analyze PPF_flat.sol PPF

Compiling with Solidity version: v0.4.24+commit.e67f0147

UUID: 39835c31-1ba4-48e7-8a6d-186b8932888c
API Version: v1.4.23
Harvey Version: 0.0.27
Maestro Version: 1.2.16
Maru Version: 0.4.8
Mythril Version: 0.21.2

Report found: 3 issues
Covered instructions: 0
Covered paths: 0
Selected compiler version: vUnknown

Title: (SWC-120) Weak Sources of Randomness from Chain Attributes
Severity: Medium
Head: Potential use of a weak source of randomness "block.number".
Description: Using past or the current block hashes through "block.number" as a source of randomness is predictable. The issue can be ignored if this is unrelated to randomness or if the usage is related to a secure implementation of a commit/reveal scheme.
Source code:

PPF_flat.sol 116:15
--------------------------------------------------
block.number
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PPF_flat.sol 83:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Title: (SWC-103) Floating Pragma
Severity: Low
Head: A floating pragma is set.
Description: It is recommended to make a conscious choice on what version of Solidity is used for compilation. Currently multiple versions "^0.4.24" are allowed.
Source code:

PPF_flat.sol 103:0
--------------------------------------------------
pragma solidity ^0.4.24;
--------------------------------------------------

==================================================

Done
```