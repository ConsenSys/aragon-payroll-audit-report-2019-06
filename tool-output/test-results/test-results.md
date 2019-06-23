## Tests

```js
  npm run test

> @aragon/future-apps-payroll@0.0.1 test aragon-apps/future-apps/payroll
> TRUFFLE_TEST=true npm run ganache-cli:test


> @aragon/future-apps-payroll@0.0.1 ganache-cli:test aragon-apps/future-apps/payroll
> ./node_modules/@aragon/test-helpers/ganache-cli.sh

Starting ganache-cli...
Running ganache-cli with pid 53025 in port 8545
Running tests...
Compiling ./contracts/Payroll.sol...
Compiling ./contracts/PayrollKit.sol...
Compiling ./contracts/test/TestImports.sol...
Compiling ./contracts/test/mocks/ExecutionTarget.sol...
Compiling ./contracts/test/mocks/MaliciousEmployee.sol...
Compiling ./contracts/test/mocks/PayrollMock.sol...
Compiling ./contracts/test/mocks/PriceFeedMock.sol...
Compiling @aragon/apps-finance/contracts/Finance.sol...
Compiling @aragon/apps-shared-migrations/contracts/Migrations.sol...
Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
Compiling @aragon/apps-vault/contracts/Vault.sol...
Compiling @aragon/os/contracts/acl/ACL.sol...
Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
Compiling @aragon/os/contracts/acl/IACL.sol...
Compiling @aragon/os/contracts/acl/IACLOracle.sol...
Compiling @aragon/os/contracts/apm/APMNamehash.sol...
Compiling @aragon/os/contracts/apm/Repo.sol...
Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
Compiling @aragon/os/contracts/apps/AppStorage.sol...
Compiling @aragon/os/contracts/apps/AragonApp.sol...
Compiling @aragon/os/contracts/common/Autopetrified.sol...
Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
Compiling @aragon/os/contracts/common/DelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
Compiling @aragon/os/contracts/common/DepositableStorage.sol...
Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
Compiling @aragon/os/contracts/common/IForwarder.sol...
Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
Compiling @aragon/os/contracts/common/Initializable.sol...
Compiling @aragon/os/contracts/common/IsContract.sol...
Compiling @aragon/os/contracts/common/Petrifiable.sol...
Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
Compiling @aragon/os/contracts/common/SafeERC20.sol...
Compiling @aragon/os/contracts/common/TimeHelpers.sol...
Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
Compiling @aragon/os/contracts/factory/DAOFactory.sol...
Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
Compiling @aragon/os/contracts/kernel/IKernel.sol...
Compiling @aragon/os/contracts/kernel/Kernel.sol...
Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
Compiling @aragon/os/contracts/lib/ens/ENS.sol...
Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
Compiling @aragon/os/contracts/lib/math/SafeMath8.sol...
Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
Compiling @aragon/os/contracts/lib/token/ERC20.sol...
Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
Compiling @aragon/ppf-contracts/contracts/PPF.sol...
Compiling @aragon/ppf-contracts/contracts/open-zeppelin/ECRecovery.sol...
Compiling @aragon/test-helpers/contracts/TimeHelpersMock.sol...

Compilation warnings encountered:

@aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function Controlled()  public { controller = msg.sender;}
    ^-------------------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function MiniMeToken(
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceFrom = balanceOfAt(_from, block.number);
        ^---------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
        var previousBalanceTo = balanceOfAt(_to, block.number);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (records[node].owner != msg.sender) throw;
                                               ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function ENS() public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
        var subnode = keccak256(node, label);
        ^---------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (ens.owner(node) != msg.sender) throw;
                                           ^---^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
    function PublicResolver(AbstractENS ensAddr) public {
    ^ (Relevant source part starts here and spans across multiple lines).
,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
        var record = records[node];
        ^--------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
        if (((contentType - 1) & contentType) != 0) throw;
                                                    ^---^
,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
    function setOwner(bytes32 node, address owner) only_owner(node) public {
                                    ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
    function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
                                                          ^-----------^
@aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
    function owner(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
    function setResolver(bytes32 node, address resolver) only_owner(node) public {
                                       ^--------------^
@aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
    function resolver(bytes32 node) public constant returns (address) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
    function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
                                  ^--------^
@aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
    function ttl(bytes32 node) public constant returns (uint64) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
    function setAddr(bytes32 node, address addr) only_owner(node) public {
                                   ^----------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
    function addr(bytes32 node) public constant returns (address ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
    function setName(bytes32 node, string name) only_owner(node) public {
                                   ^---------^
@aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
    function name(bytes32 node) public constant returns (string ret) {
    ^ (Relevant source part starts here and spans across multiple lines).

,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
    function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
    ^-----------------------------------------------------------------------------------------------------^
,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
    function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
    ^--------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
    function canForward(address sender, bytes evmCallScript) public view returns (bool);
    ^----------------------------------------------------------------------------------^
,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
    function forward(bytes evmCallScript) public;
    ^-------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_from, _to, _amount);
        ^---------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
        Approval(msg.sender, _spender, _amount);
        ^-------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewCloneToken(address(cloneToken), snapshot);
        ^------------------------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(0, _owner, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(_owner, 0, _amount);
        ^--------------------------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
            controller.transfer(this.balance);
                                ^----------^
,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
        ClaimedTokens(_token, controller, balance);
        ^----------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
    function owner(bytes32 _node) public constant returns (address);
    ^--------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
    function resolver(bytes32 _node) public constant returns (address);
    ^-----------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
    function ttl(bytes32 _node) public constant returns (uint64);
    ^-----------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
    function setOwner(bytes32 _node, address _owner) public;
    ^------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
    function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
    ^----------------------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
    function setResolver(bytes32 _node, address _resolver) public;
    ^------------------------------------------------------------^
,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
    function setTTL(bytes32 _node, uint64 _ttl) public;
    ^-------------------------------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
        records[0].owner = msg.sender;
                ^
,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
        Transfer(node, owner);
        ^-------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
        var subnode = keccak256(node, label);
                      ^--------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewOwner(node, label, owner);
        ^--------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewResolver(node, resolver);
        ^-------------------------^
,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
        NewTTL(node, ttl);
        ^---------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
        AddrChanged(node, addr);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
        ContentChanged(node, hash);
        ^------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
        NameChanged(node, name);
        ^---------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
        ABIChanged(node, contentType);
        ^---------------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
        PubkeyChanged(node, x, y);
        ^-----------------------^
,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
        TextChanged(node, key, key);
        ^-------------------------^
,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
    function allowRecoverability(address token) public view returns (bool) {
                                 ^-----------^
,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
    function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
    ^--------------------------------------------------------------------------------------^



  Contract: Payroll employees addition
    addEmployee
      when it has already been initialized
        when the sender has permissions to add employees
          when the employee has not been added yet
            when the given end date is in the past
              when the employee address is not the zero address
                ✓ starts with ID 1
                ✓ adds a new employee and emits an event
                ✓ can add another employee (101ms)
              when the employee address is not the zero address
                ✓ reverts (63ms)
            when the given end date is in the future
              when the employee address is not the zero address
                ✓ starts with ID 1
                ✓ adds a new employee and emits an event
                ✓ can add another employee (111ms)
              when the employee address is not the zero address
                ✓ reverts (65ms)
          when the employee has already been added
            when the given end date is in the past
              ✓ reverts (54ms)
            when the given end date is in the future
              ✓ reverts (64ms)
        when the sender does not have permissions to add employees
          ✓ reverts (63ms)
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll allowed tokens,
    addAllowedToken
      when it has already been initialized
        when the sender has permissions
          when it does not reach the maximum amount allowed
            ✓ can allow a token (121ms)
            ✓ can allow a the zero address (121ms)
            ✓ can allow multiple tokens (1202ms)
          when it reaches the maximum amount allowed
            ✓ can not add one more token (473ms)
            ✓ does not run out of gas to payout salary (2540ms)
        when the sender does not have permissions
          ✓ reverts (58ms)
      when it has not been initialized yet
        ✓ reverts
    isTokenAllowed
      when it has already been initialized
        when the given token is not the zero address
          when the requested token was allowed
            ✓ returns true
          when the requested token was not allowed yet
            ✓ returns false
        when the given token is the zero address
          ✓ returns false
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll bonuses
    addBonus
      when it has already been initialized
        when the sender has permissions
          when the given employee exists
            when the given employee is active
              when the given bonus greater than zero
                when there was no previous bonus
                  ✓ adds given bonus amount (117ms)
                  ✓ emits an event (66ms)
                when there was a previous bonus
                  ✓ adds given bonus amount (115ms)
                  ✓ emits an event (64ms)
              when the given bonus is zero
                ✓ adds given bonus amount (119ms)
                ✓ emits an event (64ms)
              when the given bonus way greater than zero
                ✓ reverts (119ms)
            when the given employee is not active
              ✓ reverts (54ms)
          when the given employee does not exist
            ✓ reverts (54ms)
        when the sender does not have permissions
          ✓ reverts (71ms)
      when it has not been initialized yet
        ✓ reverts (38ms)
    bonus payday
      when it has already been initialized
        when the sender is an employee
          when the employee has already set some token allocations
            when the employee has a pending bonus
              when the requested amount is zero
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (353ms)
                      ✓ emits one event per allocated token (312ms)
                      ✓ does not remove the employee and resets the bonus amount (351ms)
                    when exchange rates are expired
                      ✓ reverts (46ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (397ms)
                      ✓ emits one event per allocated token (289ms)
                      ✓ does not remove the employee and resets the bonus amount (351ms)
                    when exchange rates are expired
                      ✓ reverts (44ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (427ms)
                      ✓ emits one event per allocated token (289ms)
                      ✓ does not remove the employee and resets the bonus amount (377ms)
                    when exchange rates are expired
                      ✓ reverts (44ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (378ms)
                      ✓ emits one event per allocated token (299ms)
                      ✓ removes the employee (382ms)
                    when exchange rates are expired
                      ✓ reverts (46ms)
              when the requested amount is less than the total bonus amount
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (380ms)
                      ✓ emits one event per allocated token (326ms)
                      ✓ does not remove the employee and resets the bonus amount (375ms)
                    when exchange rates are expired
                      ✓ reverts (48ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (398ms)
                      ✓ emits one event per allocated token (367ms)
                      ✓ does not remove the employee and resets the bonus amount (354ms)
                    when exchange rates are expired
                      ✓ reverts (45ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (381ms)
                      ✓ emits one event per allocated token (306ms)
                      ✓ does not remove the employee and resets the bonus amount (354ms)
                    when exchange rates are expired
                      ✓ reverts (236ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (420ms)
                      ✓ emits one event per allocated token (296ms)
                      ✓ does not remove the employee and resets the bonus amount (375ms)
                    when exchange rates are expired
                      ✓ reverts (44ms)
              when the requested amount is equal to the total bonus amount
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (390ms)
                      ✓ emits one event per allocated token (336ms)
                      ✓ does not remove the employee and resets the bonus amount (382ms)
                    when exchange rates are expired
                      ✓ reverts (44ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (376ms)
                      ✓ emits one event per allocated token (289ms)
                      ✓ does not remove the employee and resets the bonus amount (354ms)
                    when exchange rates are expired
                      ✓ reverts (47ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (370ms)
                      ✓ emits one event per allocated token (396ms)
                      ✓ does not remove the employee and resets the bonus amount (358ms)
                    when exchange rates are expired
                      ✓ reverts (48ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending bonus (379ms)
                      ✓ emits one event per allocated token (305ms)
                      ✓ removes the employee (338ms)
                    when exchange rates are expired
                      ✓ reverts (44ms)
              when the requested amount is greater than the total bonus amount
                ✓ reverts
            when the employee does not have pending reimbursements
              when the requested amount is greater than zero
                ✓ reverts
              when the requested amount is zero
                ✓ reverts
          when the employee did not set any token allocations yet
            when the employee has a pending bonus
              when the requested amount is zero
                ✓ reverts
              when the requested amount is less than the total bonus amount
                ✓ reverts (45ms)
              when the requested amount is equal to the total bonus amount
                ✓ reverts (43ms)
              when the requested amount is greater than the total bonus amount
                ✓ reverts
            when the employee does not have pending reimbursements
              when the requested amount is greater than zero
                ✓ reverts
              when the requested amount is zero
                ✓ reverts
        when the sender is not an employee
          when the requested amount is greater than zero
            ✓ reverts
          when the requested amount is zero
            ✓ reverts
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll forwarding
    isForwarder
      when it has already been initialized
        ✓ returns true
      when it has not been initialized yet
        ✓ returns true
    canForward
      when it has already been initialized
        when the sender is an employee
          when the employee was not terminated
            ✓ returns true
          when the employee has termination date
            when the termination date has not been reached
              ✓ returns true
            when the termination date has been reached
              ✓ returns false
        when the sender is not an employee
          ✓ returns false
      when it has not been initialized yet
        ✓ returns false
    forward
      when it has already been initialized
        when the sender is an employee
          when the employee was not terminated
            ✓ executes the given script (91ms)
          when the employee has termination date
            when the termination date has not been reached
              ✓ executes the given script (90ms)
            when the termination date has been reached
              ✓ reverts (50ms)
        when the sender is not an employee
          ✓ reverts (49ms)
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll employee getters
    getEmployee
      when it has already been initialized
        when the given id exists
          ✓ adds a new employee (50ms)
        when the given id does not exist
          ✓ reverts
      when it has not been initialized yet
        ✓ reverts (177ms)
    getEmployeeByAddress
      when it has already been initialized
        when the given address exists
          ✓ adds a new employee (52ms)
        when the given id does not exist
          ✓ reverts
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll gas costs
    gas costs
      when there is only one allowed token
        ✓ expends ~335k gas for a single allowed token (224ms)
      when there are two allowed token
        ✓ expends ~295k gas per allowed token (577ms)

  Contract: Payroll initialization
    initialize
      ✓ cannot initialize the base app (47ms)
      when it has not been initialized yet
        ✓ can be initialized with a zero denomination token (59ms)
        ✓ reverts when passing an expiration time lower than one minute
        ✓ reverts when passing an invalid finance instance
        ✓ reverts when passing an invalid feed instance
      when it has already been initialized
        ✓ cannot be initialized again
        ✓ has a price feed instance, a finance instance, a denomination token and a rate expiration time (102ms)

  Contract: Payroll employees modification
    setEmployeeSalary
      when it has already been initialized
        when the sender has permissions
          when the given employee exists
            when the given employee is active
              when the given value greater than zero
                when the employee is not owed a huge salary amount
                  ✓ changes the salary of the employee (97ms)
                  ✓ adds previous owed salary to the accrued salary (284ms)
                  ✓ accrues all previous owed salary as accrued salary (313ms)
                  ✓ emits a SetEmployeeSalary event (67ms)
                when the employee is owed a huge salary amount
                  ✓ reverts (56ms)
              when the given value is zero
                ✓ changes the salary of the employee (124ms)
                ✓ adds previous owed salary to the accrued salary (243ms)
                ✓ accrues all previous owed salary as accrued salary (408ms)
                ✓ emits a SetEmployeeSalary event (72ms)
            when the given employee is not active
              ✓ reverts (56ms)
          when the given employee does not exist
            ✓ reverts (53ms)
        when the sender does not have permissions
          ✓ reverts (55ms)
      when it has not been initialized yet
        ✓ reverts
    changeAddressByEmployee
      when it has already been initialized
        when the sender is an employee
          when the given employee is active
            when the given address is a plain new address
              ✓ changes the address of the employee (80ms)
              ✓ emits an event (48ms)
            when the given address is the same address
              ✓ reverts
            when the given address belongs to another employee
              ✓ reverts
            when the given address is the zero address
              ✓ reverts
          when the given employee is not active
            when the given address is a plain new address
              ✓ changes the address of the employee (74ms)
              ✓ emits an event (47ms)
            when the given address is the same address
              ✓ reverts
            when the given address belongs to another employee
              ✓ reverts
            when the given address is the zero address
              ✓ reverts
        when the sender is not an employee
          ✓ reverts
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll payday
    payroll payday
      when it has already been initialized
        when the sender is an employee
          when the employee has a reasonable salary
            when the employee has already set some token allocations
              when the employee does not have accrued salary
                when the employee has some pending salary
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (334ms)
                            ✓ emits one event per allocated token (280ms)
                            ✓ can be called multiple times between periods of time (897ms)
                            ✓ updates the accrued salary and the last payroll date (389ms)
                            ✓ does not remove the employee (361ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (432ms)
                            ✓ emits one event per allocated token (308ms)
                            ✓ can be called multiple times between periods of time (886ms)
                            ✓ updates the accrued salary and the last payroll date (367ms)
                            ✓ does not remove the employee (329ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (377ms)
                            ✓ emits one event per allocated token (287ms)
                            ✓ can be called multiple times between periods of time (1018ms)
                            ✓ updates the accrued salary and the last payroll date (355ms)
                            ✓ does not remove the employee (373ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (380ms)
                            ✓ emits one event per allocated token (306ms)
                            ✓ can be called multiple times between periods of time (968ms)
                            ✓ updates the accrued salary and the last payroll date (351ms)
                            ✓ does not remove the employee (322ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (404ms)
                            ✓ emits one event per allocated token (325ms)
                            ✓ can be called multiple times between periods of time (975ms)
                            ✓ updates the accrued salary and the last payroll date (406ms)
                            ✓ does not remove the employee (360ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (436ms)
                            ✓ emits one event per allocated token (309ms)
                            ✓ can be called multiple times between periods of time (903ms)
                            ✓ updates the accrued salary and the last payroll date (369ms)
                            ✓ does not remove the employee (332ms)
                          when exchange rates are expired
                            ✓ reverts (75ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (390ms)
                            ✓ emits one event per allocated token (322ms)
                            ✓ can be called multiple times between periods of time (960ms)
                            ✓ updates the accrued salary and the last payroll date (388ms)
                            ✓ does not remove the employee (358ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (403ms)
                            ✓ emits one event per allocated token (527ms)
                            ✓ can be called multiple times between periods of time (958ms)
                            ✓ removes the employee (369ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                  when the requested amount is lower than the total owed salary
                    when the requested amount represents less than a second of the earnings
                      ✓ updates the last payroll date by one second (412ms)
                    when the requested amount represents more than a second of the earnings
                      when the employee has some pending reimbursements
                        when the employee has a pending bonus
                          when the employee is not terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (406ms)
                              ✓ emits one event per allocated token (433ms)
                              ✓ can be called multiple times between periods of time (1135ms)
                              ✓ updates the accrued salary and the last payroll date (401ms)
                              ✓ does not remove the employee (434ms)
                            when exchange rates are expired
                              ✓ reverts (52ms)
                          when the employee is terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (490ms)
                              ✓ emits one event per allocated token (435ms)
                              ✓ can be called multiple times between periods of time (1391ms)
                              ✓ updates the accrued salary and the last payroll date (395ms)
                              ✓ does not remove the employee (344ms)
                            when exchange rates are expired
                              ✓ reverts (54ms)
                        when the employee does not have a pending bonus
                          when the employee is not terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (384ms)
                              ✓ emits one event per allocated token (306ms)
                              ✓ can be called multiple times between periods of time (888ms)
                              ✓ updates the accrued salary and the last payroll date (416ms)
                              ✓ does not remove the employee (400ms)
                            when exchange rates are expired
                              ✓ reverts (54ms)
                          when the employee is terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (466ms)
                              ✓ emits one event per allocated token (420ms)
                              ✓ can be called multiple times between periods of time (1374ms)
                              ✓ updates the accrued salary and the last payroll date (457ms)
                              ✓ does not remove the employee (348ms)
                            when exchange rates are expired
                              ✓ reverts (49ms)
                      when the employee does not have pending reimbursements
                        when the employee has a pending bonus
                          when the employee is not terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (382ms)
                              ✓ emits one event per allocated token (325ms)
                              ✓ can be called multiple times between periods of time (920ms)
                              ✓ updates the accrued salary and the last payroll date (364ms)
                              ✓ does not remove the employee (342ms)
                            when exchange rates are expired
                              ✓ reverts (49ms)
                          when the employee is terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (368ms)
                              ✓ emits one event per allocated token (301ms)
                              ✓ can be called multiple times between periods of time (914ms)
                              ✓ updates the accrued salary and the last payroll date (358ms)
                              ✓ does not remove the employee (320ms)
                            when exchange rates are expired
                              ✓ reverts (120ms)
                        when the employee does not have a pending bonus
                          when the employee is not terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (385ms)
                              ✓ emits one event per allocated token (302ms)
                              ✓ can be called multiple times between periods of time (905ms)
                              ✓ updates the accrued salary and the last payroll date (362ms)
                              ✓ does not remove the employee (468ms)
                            when exchange rates are expired
                              ✓ reverts (49ms)
                          when the employee is terminated
                            when exchange rates are not expired
                              ✓ transfers the requested salary amount (376ms)
                              ✓ emits one event per allocated token (354ms)
                              ✓ can be called multiple times between periods of time (931ms)
                              ✓ updates the accrued salary and the last payroll date (357ms)
                              ✓ does not remove the employee (316ms)
                            when exchange rates are expired
                              ✓ reverts (49ms)
                  when the requested amount is equal to the total owed salary
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (382ms)
                            ✓ emits one event per allocated token (450ms)
                            ✓ can be called multiple times between periods of time (1222ms)
                            ✓ updates the accrued salary and the last payroll date (379ms)
                            ✓ does not remove the employee (344ms)
                          when exchange rates are expired
                            ✓ reverts (57ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (406ms)
                            ✓ emits one event per allocated token (296ms)
                            ✓ can be called multiple times between periods of time (892ms)
                            ✓ updates the accrued salary and the last payroll date (377ms)
                            ✓ does not remove the employee (334ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (392ms)
                            ✓ emits one event per allocated token (303ms)
                            ✓ can be called multiple times between periods of time (903ms)
                            ✓ updates the accrued salary and the last payroll date (431ms)
                            ✓ does not remove the employee (339ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (384ms)
                            ✓ emits one event per allocated token (294ms)
                            ✓ can be called multiple times between periods of time (913ms)
                            ✓ updates the accrued salary and the last payroll date (403ms)
                            ✓ does not remove the employee (325ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (380ms)
                            ✓ emits one event per allocated token (301ms)
                            ✓ can be called multiple times between periods of time (872ms)
                            ✓ updates the accrued salary and the last payroll date (380ms)
                            ✓ does not remove the employee (352ms)
                          when exchange rates are expired
                            ✓ reverts (63ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (471ms)
                            ✓ emits one event per allocated token (300ms)
                            ✓ can be called multiple times between periods of time (977ms)
                            ✓ updates the accrued salary and the last payroll date (368ms)
                            ✓ does not remove the employee (341ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (399ms)
                            ✓ emits one event per allocated token (313ms)
                            ✓ can be called multiple times between periods of time (1006ms)
                            ✓ updates the accrued salary and the last payroll date (367ms)
                            ✓ does not remove the employee (342ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (400ms)
                            ✓ emits one event per allocated token (307ms)
                            ✓ can be called multiple times between periods of time (904ms)
                            ✓ removes the employee (501ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                  when the requested amount is greater than the total owed salary
                    ✓ reverts
                when the employee does not have pending salary
                  when the requested amount is greater than zero
                    ✓ reverts (38ms)
                  when the requested amount is zero
                    ✓ reverts
              when the employee has some accrued salary
                when the employee has some pending salary
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (397ms)
                            ✓ emits one event per allocated token (308ms)
                            ✓ can be called multiple times between periods of time (926ms)
                            ✓ updates the accrued salary and the last payroll date (430ms)
                            ✓ does not remove the employee (350ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (408ms)
                            ✓ emits one event per allocated token (303ms)
                            ✓ can be called multiple times between periods of time (936ms)
                            ✓ updates the accrued salary and the last payroll date (371ms)
                            ✓ does not remove the employee (343ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (451ms)
                            ✓ emits one event per allocated token (316ms)
                            ✓ can be called multiple times between periods of time (963ms)
                            ✓ updates the accrued salary and the last payroll date (366ms)
                            ✓ does not remove the employee (346ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (411ms)
                            ✓ emits one event per allocated token (319ms)
                            ✓ can be called multiple times between periods of time (928ms)
                            ✓ updates the accrued salary and the last payroll date (421ms)
                            ✓ does not remove the employee (356ms)
                          when exchange rates are expired
                            ✓ reverts (56ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (417ms)
                            ✓ emits one event per allocated token (320ms)
                            ✓ can be called multiple times between periods of time (966ms)
                            ✓ updates the accrued salary and the last payroll date (378ms)
                            ✓ does not remove the employee (351ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (610ms)
                            ✓ emits one event per allocated token (320ms)
                            ✓ can be called multiple times between periods of time (988ms)
                            ✓ updates the accrued salary and the last payroll date (687ms)
                            ✓ does not remove the employee (353ms)
                          when exchange rates are expired
                            ✓ reverts (95ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (413ms)
                            ✓ emits one event per allocated token (324ms)
                            ✓ can be called multiple times between periods of time (1036ms)
                            ✓ updates the accrued salary and the last payroll date (423ms)
                            ✓ does not remove the employee (349ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (413ms)
                            ✓ emits one event per allocated token (316ms)
                            ✓ can be called multiple times between periods of time (957ms)
                            ✓ removes the employee (347ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                  when the requested amount is lower than the previous owed salary
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (391ms)
                            ✓ emits one event per allocated token (315ms)
                            ✓ can be called multiple times between periods of time (926ms)
                            ✓ updates the accrued salary and the last payroll date (373ms)
                            ✓ does not remove the employee (340ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (410ms)
                            ✓ emits one event per allocated token (307ms)
                            ✓ can be called multiple times between periods of time (942ms)
                            ✓ updates the accrued salary and the last payroll date (391ms)
                            ✓ does not remove the employee (343ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (398ms)
                            ✓ emits one event per allocated token (312ms)
                            ✓ can be called multiple times between periods of time (1026ms)
                            ✓ updates the accrued salary and the last payroll date (367ms)
                            ✓ does not remove the employee (342ms)
                          when exchange rates are expired
                            ✓ reverts (47ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (410ms)
                            ✓ emits one event per allocated token (306ms)
                            ✓ can be called multiple times between periods of time (960ms)
                            ✓ updates the accrued salary and the last payroll date (371ms)
                            ✓ does not remove the employee (344ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (396ms)
                            ✓ emits one event per allocated token (311ms)
                            ✓ can be called multiple times between periods of time (936ms)
                            ✓ updates the accrued salary and the last payroll date (423ms)
                            ✓ does not remove the employee (366ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (400ms)
                            ✓ emits one event per allocated token (311ms)
                            ✓ can be called multiple times between periods of time (921ms)
                            ✓ updates the accrued salary and the last payroll date (363ms)
                            ✓ does not remove the employee (351ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (403ms)
                            ✓ emits one event per allocated token (332ms)
                            ✓ can be called multiple times between periods of time (1215ms)
                            ✓ updates the accrued salary and the last payroll date (396ms)
                            ✓ does not remove the employee (367ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (426ms)
                            ✓ emits one event per allocated token (316ms)
                            ✓ can be called multiple times between periods of time (1021ms)
                            ✓ updates the accrued salary and the last payroll date (429ms)
                            ✓ does not remove the employee (372ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                  when the requested amount is greater than the previous owed salary but lower than the total owed
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (438ms)
                            ✓ emits one event per allocated token (331ms)
                            ✓ can be called multiple times between periods of time (1004ms)
                            ✓ updates the accrued salary and the last payroll date (412ms)
                            ✓ does not remove the employee (381ms)
                          when exchange rates are expired
                            ✓ reverts (58ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (456ms)
                            ✓ emits one event per allocated token (348ms)
                            ✓ can be called multiple times between periods of time (1278ms)
                            ✓ updates the accrued salary and the last payroll date (395ms)
                            ✓ does not remove the employee (362ms)
                          when exchange rates are expired
                            ✓ reverts (102ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (434ms)
                            ✓ emits one event per allocated token (321ms)
                            ✓ can be called multiple times between periods of time (927ms)
                            ✓ updates the accrued salary and the last payroll date (373ms)
                            ✓ does not remove the employee (365ms)
                          when exchange rates are expired
                            ✓ reverts (56ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (420ms)
                            ✓ emits one event per allocated token (348ms)
                            ✓ can be called multiple times between periods of time (1014ms)
                            ✓ updates the accrued salary and the last payroll date (440ms)
                            ✓ does not remove the employee (408ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (441ms)
                            ✓ emits one event per allocated token (595ms)
                            ✓ can be called multiple times between periods of time (994ms)
                            ✓ updates the accrued salary and the last payroll date (392ms)
                            ✓ does not remove the employee (370ms)
                          when exchange rates are expired
                            ✓ reverts (49ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (485ms)
                            ✓ emits one event per allocated token (339ms)
                            ✓ can be called multiple times between periods of time (985ms)
                            ✓ updates the accrued salary and the last payroll date (403ms)
                            ✓ does not remove the employee (379ms)
                          when exchange rates are expired
                            ✓ reverts (54ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (432ms)
                            ✓ emits one event per allocated token (355ms)
                            ✓ can be called multiple times between periods of time (999ms)
                            ✓ updates the accrued salary and the last payroll date (470ms)
                            ✓ does not remove the employee (448ms)
                          when exchange rates are expired
                            ✓ reverts (57ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (505ms)
                            ✓ emits one event per allocated token (397ms)
                            ✓ can be called multiple times between periods of time (1163ms)
                            ✓ updates the accrued salary and the last payroll date (456ms)
                            ✓ does not remove the employee (389ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                  when the requested amount is equal to the total owed salary
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (451ms)
                            ✓ emits one event per allocated token (348ms)
                            ✓ can be called multiple times between periods of time (1019ms)
                            ✓ updates the accrued salary and the last payroll date (434ms)
                            ✓ does not remove the employee (395ms)
                          when exchange rates are expired
                            ✓ reverts (63ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (446ms)
                            ✓ emits one event per allocated token (339ms)
                            ✓ can be called multiple times between periods of time (1098ms)
                            ✓ updates the accrued salary and the last payroll date (401ms)
                            ✓ does not remove the employee (376ms)
                          when exchange rates are expired
                            ✓ reverts (59ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (425ms)
                            ✓ emits one event per allocated token (333ms)
                            ✓ can be called multiple times between periods of time (1008ms)
                            ✓ updates the accrued salary and the last payroll date (392ms)
                            ✓ does not remove the employee (358ms)
                          when exchange rates are expired
                            ✓ reverts (54ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (442ms)
                            ✓ emits one event per allocated token (1100ms)
                            ✓ can be called multiple times between periods of time (1016ms)
                            ✓ updates the accrued salary and the last payroll date (405ms)
                            ✓ does not remove the employee (361ms)
                          when exchange rates are expired
                            ✓ reverts (59ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (425ms)
                            ✓ emits one event per allocated token (388ms)
                            ✓ can be called multiple times between periods of time (1002ms)
                            ✓ updates the accrued salary and the last payroll date (423ms)
                            ✓ does not remove the employee (380ms)
                          when exchange rates are expired
                            ✓ reverts (56ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (514ms)
                            ✓ emits one event per allocated token (323ms)
                            ✓ can be called multiple times between periods of time (944ms)
                            ✓ updates the accrued salary and the last payroll date (430ms)
                            ✓ does not remove the employee (401ms)
                          when exchange rates are expired
                            ✓ reverts (58ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (459ms)
                            ✓ emits one event per allocated token (344ms)
                            ✓ can be called multiple times between periods of time (1089ms)
                            ✓ updates the accrued salary and the last payroll date (483ms)
                            ✓ does not remove the employee (381ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (877ms)
                            ✓ emits one event per allocated token (418ms)
                            ✓ can be called multiple times between periods of time (1077ms)
                            ✓ removes the employee (378ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                  when the requested amount is greater than the total owed salary
                    ✓ reverts (41ms)
                when the employee does not have pending salary
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (450ms)
                            ✓ emits one event per allocated token (338ms)
                            ✓ can be called multiple times between periods of time (1040ms)
                            ✓ updates the accrued salary and the last payroll date (412ms)
                            ✓ does not remove the employee (395ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (458ms)
                            ✓ emits one event per allocated token (358ms)
                            ✓ can be called multiple times between periods of time (1225ms)
                            ✓ updates the accrued salary and the last payroll date (440ms)
                            ✓ does not remove the employee (382ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (450ms)
                            ✓ emits one event per allocated token (339ms)
                            ✓ can be called multiple times between periods of time (1022ms)
                            ✓ updates the accrued salary and the last payroll date (407ms)
                            ✓ does not remove the employee (363ms)
                          when exchange rates are expired
                            ✓ reverts (48ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (441ms)
                            ✓ emits one event per allocated token (337ms)
                            ✓ can be called multiple times between periods of time (1005ms)
                            ✓ updates the accrued salary and the last payroll date (397ms)
                            ✓ does not remove the employee (364ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (431ms)
                            ✓ emits one event per allocated token (340ms)
                            ✓ can be called multiple times between periods of time (1010ms)
                            ✓ updates the accrued salary and the last payroll date (424ms)
                            ✓ does not remove the employee (381ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (438ms)
                            ✓ emits one event per allocated token (393ms)
                            ✓ can be called multiple times between periods of time (997ms)
                            ✓ updates the accrued salary and the last payroll date (403ms)
                            ✓ does not remove the employee (369ms)
                          when exchange rates are expired
                            ✓ reverts (54ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (462ms)
                            ✓ emits one event per allocated token (345ms)
                            ✓ can be called multiple times between periods of time (2293ms)
                            ✓ updates the accrued salary and the last payroll date (387ms)
                            ✓ does not remove the employee (373ms)
                          when exchange rates are expired
                            ✓ reverts (48ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (428ms)
                            ✓ emits one event per allocated token (390ms)
                            ✓ can be called multiple times between periods of time (1005ms)
                            ✓ removes the employee (387ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                  when the requested amount is lower than the previous owed salary
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (431ms)
                            ✓ emits one event per allocated token (392ms)
                            ✓ can be called multiple times between periods of time (1036ms)
                            ✓ updates the accrued salary and the last payroll date (411ms)
                            ✓ does not remove the employee (391ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (446ms)
                            ✓ emits one event per allocated token (334ms)
                            ✓ can be called multiple times between periods of time (1000ms)
                            ✓ updates the accrued salary and the last payroll date (405ms)
                            ✓ does not remove the employee (368ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (430ms)
                            ✓ emits one event per allocated token (342ms)
                            ✓ can be called multiple times between periods of time (994ms)
                            ✓ updates the accrued salary and the last payroll date (404ms)
                            ✓ does not remove the employee (375ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (443ms)
                            ✓ emits one event per allocated token (342ms)
                            ✓ can be called multiple times between periods of time (1049ms)
                            ✓ updates the accrued salary and the last payroll date (402ms)
                            ✓ does not remove the employee (406ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (457ms)
                            ✓ emits one event per allocated token (342ms)
                            ✓ can be called multiple times between periods of time (1037ms)
                            ✓ updates the accrued salary and the last payroll date (611ms)
                            ✓ does not remove the employee (374ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (450ms)
                            ✓ emits one event per allocated token (372ms)
                            ✓ can be called multiple times between periods of time (1062ms)
                            ✓ updates the accrued salary and the last payroll date (423ms)
                            ✓ does not remove the employee (378ms)
                          when exchange rates are expired
                            ✓ reverts (51ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (438ms)
                            ✓ emits one event per allocated token (340ms)
                            ✓ can be called multiple times between periods of time (1008ms)
                            ✓ updates the accrued salary and the last payroll date (410ms)
                            ✓ does not remove the employee (383ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (490ms)
                            ✓ emits one event per allocated token (1542ms)
                            ✓ can be called multiple times between periods of time (1073ms)
                            ✓ updates the accrued salary and the last payroll date (427ms)
                            ✓ does not remove the employee (401ms)
                          when exchange rates are expired
                            ✓ reverts (56ms)
                  when the requested amount is equal to the previous owed salary
                    when the employee has some pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (522ms)
                            ✓ emits one event per allocated token (386ms)
                            ✓ can be called multiple times between periods of time (1143ms)
                            ✓ updates the accrued salary and the last payroll date (440ms)
                            ✓ does not remove the employee (392ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (1611ms)
                            ✓ emits one event per allocated token (341ms)
                            ✓ can be called multiple times between periods of time (1016ms)
                            ✓ updates the accrued salary and the last payroll date (462ms)
                            ✓ does not remove the employee (372ms)
                          when exchange rates are expired
                            ✓ reverts (50ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (435ms)
                            ✓ emits one event per allocated token (343ms)
                            ✓ can be called multiple times between periods of time (1048ms)
                            ✓ updates the accrued salary and the last payroll date (433ms)
                            ✓ does not remove the employee (393ms)
                          when exchange rates are expired
                            ✓ reverts (56ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (585ms)
                            ✓ emits one event per allocated token (386ms)
                            ✓ can be called multiple times between periods of time (1081ms)
                            ✓ updates the accrued salary and the last payroll date (422ms)
                            ✓ does not remove the employee (387ms)
                          when exchange rates are expired
                            ✓ reverts (55ms)
                    when the employee does not have pending reimbursements
                      when the employee has a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (439ms)
                            ✓ emits one event per allocated token (345ms)
                            ✓ can be called multiple times between periods of time (1030ms)
                            ✓ updates the accrued salary and the last payroll date (419ms)
                            ✓ does not remove the employee (391ms)
                          when exchange rates are expired
                            ✓ reverts (77ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (413ms)
                            ✓ emits one event per allocated token (336ms)
                            ✓ can be called multiple times between periods of time (1006ms)
                            ✓ updates the accrued salary and the last payroll date (413ms)
                            ✓ does not remove the employee (446ms)
                          when exchange rates are expired
                            ✓ reverts (53ms)
                      when the employee does not have a pending bonus
                        when the employee is not terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (439ms)
                            ✓ emits one event per allocated token (365ms)
                            ✓ can be called multiple times between periods of time (1051ms)
                            ✓ updates the accrued salary and the last payroll date (427ms)
                            ✓ does not remove the employee (376ms)
                          when exchange rates are expired
                            ✓ reverts (58ms)
                        when the employee is terminated
                          when exchange rates are not expired
                            ✓ transfers the requested salary amount (473ms)
                            ✓ emits one event per allocated token (402ms)
                            ✓ can be called multiple times between periods of time (1111ms)
                            ✓ removes the employee (426ms)
                          when exchange rates are expired
                            ✓ reverts (52ms)
                  when the requested amount is greater than the previous owed salary
                    ✓ reverts (41ms)
            when the employee did not set any token allocations yet
              when the employee has some pending salary
                when the requested amount is lower than the total owed salary
                  ✓ reverts (51ms)
                when the requested amount is equal to the total owed salary
                  ✓ reverts (47ms)
              when the employee does not have pending salary
                when the requested amount is greater than zero
                  ✓ reverts (40ms)
                when the requested amount is zero
                  ✓ reverts (636ms)
          when the employee does not have a reasonable salary
            when the employee has a zero salary
              when the employee has already set some token allocations
                when the employee has some pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (69ms)
                        when exchange rates are expired
                          ✓ reverts (56ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (50ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (44ms)
                        when exchange rates are expired
                          ✓ reverts (42ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts (43ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts (41ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts (40ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts (38ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts (40ms)
                when the employee does not have pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (41ms)
                        when exchange rates are expired
                          ✓ reverts (42ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts (58ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (41ms)
                        when exchange rates are expired
                          ✓ reverts (43ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (42ms)
                        when exchange rates are expired
                          ✓ reverts (88ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (44ms)
                        when exchange rates are expired
                          ✓ reverts
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (42ms)
                        when exchange rates are expired
                          ✓ reverts (38ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (78ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts
              when the employee did not set any token allocations yet
                when the employee has some pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (43ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (78ms)
                        when exchange rates are expired
                          ✓ reverts (41ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts (44ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (42ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (41ms)
                        when exchange rates are expired
                          ✓ reverts (45ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (50ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (53ms)
                        when exchange rates are expired
                          ✓ reverts (43ms)
                when the employee does not have pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (43ms)
                        when exchange rates are expired
                          ✓ reverts (44ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (57ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (56ms)
                        when exchange rates are expired
                          ✓ reverts (81ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (50ms)
                        when exchange rates are expired
                          ✓ reverts (43ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts (39ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (38ms)
                        when exchange rates are expired
                          ✓ reverts (39ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (39ms)
            when the employee has a huge salary
              when the employee has already set some token allocations
                when the employee has some pending salary
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (54ms)
                        when exchange rates are expired
                          ✓ reverts (65ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (53ms)
                        when exchange rates are expired
                          ✓ reverts (59ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (105ms)
                        when exchange rates are expired
                          ✓ reverts (57ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (56ms)
                        when exchange rates are expired
                          ✓ reverts (53ms)
                  when the requested amount is lower than the total owed salary
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ transfers the requested salary amount (545ms)
                          ✓ emits one event per allocated token (404ms)
                          ✓ can be called multiple times between periods of time (2132ms)
                          ✓ updates the last payroll date (736ms)
                          ✓ does not remove the employee (1553ms)
                        when exchange rates are expired
                          ✓ reverts (62ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ transfers the requested salary amount (486ms)
                          ✓ emits one event per allocated token (358ms)
                          ✓ can be called multiple times between periods of time (979ms)
                          ✓ updates the last payroll date (408ms)
                          ✓ does not remove the employee (377ms)
                        when exchange rates are expired
                          ✓ reverts (59ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ transfers the requested salary amount (456ms)
                          ✓ emits one event per allocated token (337ms)
                          ✓ can be called multiple times between periods of time (1022ms)
                          ✓ updates the last payroll date (424ms)
                          ✓ does not remove the employee (411ms)
                        when exchange rates are expired
                          ✓ reverts (61ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ transfers the requested salary amount (475ms)
                          ✓ emits one event per allocated token (378ms)
                          ✓ can be called multiple times between periods of time (1093ms)
                          ✓ updates the last payroll date (460ms)
                          ✓ does not remove the employee (494ms)
                        when exchange rates are expired
                          ✓ reverts (63ms)
                  when the requested amount is equal to the total owed salary
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (59ms)
                        when exchange rates are expired
                          ✓ reverts (76ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (64ms)
                        when exchange rates are expired
                          ✓ reverts (60ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (57ms)
                        when exchange rates are expired
                          ✓ reverts (50ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (317ms)
                        when exchange rates are expired
                          ✓ reverts (51ms)
                when the employee does not have pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (38ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (41ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (38ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (38ms)
                        when exchange rates are expired
                          ✓ reverts (39ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (38ms)
                        when exchange rates are expired
                          ✓ reverts (52ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (42ms)
                        when exchange rates are expired
                          ✓ reverts (39ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (40ms)
              when the employee did not set any token allocations yet
                when the employee has some pending salary
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (44ms)
                        when exchange rates are expired
                          ✓ reverts (44ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (43ms)
                        when exchange rates are expired
                          ✓ reverts (42ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (43ms)
                        when exchange rates are expired
                          ✓ reverts (41ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (42ms)
                        when exchange rates are expired
                          ✓ reverts (42ms)
                  when the requested amount is lower than the total owed salary
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (41ms)
                        when exchange rates are expired
                          ✓ reverts (44ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (47ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (51ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (48ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                  when the requested amount is equal to the total owed salary
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (51ms)
                        when exchange rates are expired
                          ✓ reverts (48ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (52ms)
                        when exchange rates are expired
                          ✓ reverts (47ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (47ms)
                        when exchange rates are expired
                          ✓ reverts (50ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (48ms)
                        when exchange rates are expired
                          ✓ reverts (45ms)
                when the employee does not have pending salary
                  when the requested amount is greater than zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts (52ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (47ms)
                        when exchange rates are expired
                          ✓ reverts (43ms)
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts (42ms)
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts (39ms)
                  when the requested amount is zero
                    when the employee has some pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts (39ms)
                        when exchange rates are expired
                          ✓ reverts
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts
                    when the employee does not have pending reimbursements
                      when the employee is not terminated
                        when exchange rates are not expired
                          ✓ reverts
                        when exchange rates are expired
                          ✓ reverts
                      when the employee is terminated
                        when exchange rates are not expired
                          ✓ reverts (40ms)
                        when exchange rates are expired
                          ✓ reverts
        when the sender is not an employee
          when the requested amount is greater than zero
            ✓ reverts
          when the requested amount is zero
            ✓ reverts
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll rates handling,
    when the denomination token is USD
      when the employee requests only ETH
        ✓ receives the expected amount of ETH (627ms)
      when the employee requests only ANT
        ✓ receives the expected amount of ANT (622ms)
      when the employee requests multiple tokens
        ✓ receives the expected amount of tokens (824ms)
    when the denomination token is ETH
      when the employee requests only ETH
        ✓ receives the expected amount of ETH (601ms)
      when the employee requests only ANT
        ✓ receives the expected amount of ANT (832ms)
      when the employee requests multiple tokens
        ✓ receives the expected amount of tokens (1598ms)
    when the denomination token is DAI
      when the employee requests only ETH
        ✓ receives the expected amount of ETH (1065ms)
      when the employee requests only ANT
        ✓ receives the expected amount of ANT (923ms)
      when the employee requests multiple tokens
        ✓ receives the expected amount of tokens (1133ms)
    when the denomination token is ANT
      when the employee requests only ETH
        ✓ receives the expected amount of ETH (852ms)
      when the employee requests only ANT
        ✓ receives the expected amount of ANT (864ms)
      when the employee requests multiple tokens
        ✓ receives the expected amount of tokens (1157ms)

  Contract: Payroll reentrancy guards
    reentrancy guards
      determineAllocation
        ✓ reverts (186ms)
      changeAddressByEmployee
        ✓ reverts (171ms)
      payday
        ✓ reverts (173ms)

  Contract: Payroll reimbursements
    addReimbursement
      when it has already been initialized
        when the sender has permissions
          when the given employee exists
            when the given employee is active
              when the given reimbursement greater than zero
                ✓ adds requested reimbursement (109ms)
                ✓ emits an event (77ms)
              when the given reimbursement is zero
                ✓ adds requested reimbursement (105ms)
                ✓ emits an event (78ms)
              when the given reimbursement way greater than zero
                ✓ reverts (136ms)
            when the given employee is not active
              ✓ reverts (66ms)
          when the given employee does not exist
            ✓ reverts (60ms)
        when the sender does not have permissions
          ✓ reverts (65ms)
      when it has not been initialized yet
        ✓ reverts (38ms)
    reimbursements payday
      when it has already been initialized
        when the sender is an employee
          when the employee has already set some token allocations
            when the employee has some pending reimbursements
              when the requested amount is zero
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (409ms)
                      ✓ emits one event per allocated token (325ms)
                      ✓ does not remove the employee and resets the reimbursements (415ms)
                    when exchange rates are expired
                      ✓ reverts (50ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (486ms)
                      ✓ emits one event per allocated token (342ms)
                      ✓ does not remove the employee and resets the reimbursements (400ms)
                    when exchange rates are expired
                      ✓ reverts (52ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (441ms)
                      ✓ emits one event per allocated token (361ms)
                      ✓ does not remove the employee and resets the reimbursements (430ms)
                    when exchange rates are expired
                      ✓ reverts (52ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (450ms)
                      ✓ emits one event per allocated token (360ms)
                      ✓ removes the employee (456ms)
                    when exchange rates are expired
                      ✓ reverts (50ms)
              when the requested amount is less than the total reimbursements amount
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (448ms)
                      ✓ emits one event per allocated token (349ms)
                      ✓ does not remove the employee and resets the reimbursements (450ms)
                    when exchange rates are expired
                      ✓ reverts (54ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (540ms)
                      ✓ emits one event per allocated token (488ms)
                      ✓ does not remove the employee and resets the reimbursements (523ms)
                    when exchange rates are expired
                      ✓ reverts (64ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (536ms)
                      ✓ emits one event per allocated token (983ms)
                      ✓ does not remove the employee and resets the reimbursements (470ms)
                    when exchange rates are expired
                      ✓ reverts (57ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (521ms)
                      ✓ emits one event per allocated token (453ms)
                      ✓ does not remove the employee and resets the reimbursements (550ms)
                    when exchange rates are expired
                      ✓ reverts (60ms)
              when the requested amount is equal to the total reimbursements amount
                when the employee has some pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (475ms)
                      ✓ emits one event per allocated token (366ms)
                      ✓ does not remove the employee and resets the reimbursements (420ms)
                    when exchange rates are expired
                      ✓ reverts (54ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (494ms)
                      ✓ emits one event per allocated token (606ms)
                      ✓ does not remove the employee and resets the reimbursements (458ms)
                    when exchange rates are expired
                      ✓ reverts (55ms)
                when the employee does not have pending salary
                  when the employee is not terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (564ms)
                      ✓ emits one event per allocated token (367ms)
                      ✓ does not remove the employee and resets the reimbursements (450ms)
                    when exchange rates are expired
                      ✓ reverts (53ms)
                  when the employee is terminated
                    when exchange rates are not expired
                      ✓ transfers all the pending reimbursements (700ms)
                      ✓ emits one event per allocated token (358ms)
                      ✓ removes the employee (406ms)
                    when exchange rates are expired
                      ✓ reverts (50ms)
              when the requested amount is greater than the total reimbursements amount
                ✓ reverts (40ms)
            when the employee does not have pending reimbursements
              when the requested amount is greater than zero
                ✓ reverts
              when the requested amount is zero
                ✓ reverts
          when the employee did not set any token allocations yet
            when the employee has some pending reimbursements
              when the requested amount is zero
                ✓ reverts (39ms)
              when the requested amount is less than the total reimbursements amount
                ✓ reverts (43ms)
              when the requested amount is equal to the total reimbursements amount
                ✓ reverts (41ms)
              when the requested amount is greater than the total reimbursements amount
                ✓ reverts (40ms)
            when the employee does not have pending reimbursements
              when the requested amount is greater than zero
                ✓ reverts (39ms)
              when the requested amount is zero
                ✓ reverts (44ms)
        when the sender is not an employee
          when the requested amount is greater than zero
            ✓ reverts (40ms)
          when the requested amount is zero
            ✓ reverts
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll settings
    setPriceFeed
      when it has already been initialized
        when the sender has permissions
          when the given address is a contract
            ✓ updates the feed address (113ms)
            ✓ emits an event (82ms)
          when the given address is not a contract
            ✓ reverts (70ms)
          when the given address is the zero address
            ✓ reverts (65ms)
        when the sender does not have permissions
          ✓ reverts (67ms)
      when it has not been initialized yet
        ✓ reverts (40ms)
    setRateExpiryTime
      when it has already been initialized
        when the sender has permissions
          when the given expiration time is one minute
            ✓ updates the expiration time (109ms)
            ✓ emits an event (79ms)
          when the given expiration time is greater than one minute
            ✓ updates the expiration time (109ms)
            ✓ emits an event (78ms)
          when the given expiration time is less than one minute
            ✓ reverts (64ms)
        when the sender does not have permissions
          ✓ reverts (66ms)
      when it has not been initialized yet
        ✓ reverts

  Contract: Payroll employees termination
    terminateEmployee
      when it has already been initialized
        when the given employee id exists
          when the sender has permissions to terminate employees
            when the employee was not terminated
              when the given end date is in the future
                ✓ sets the end date of the employee (109ms)
                ✓ emits an event (75ms)
                ✓ does not reset the owed salary nor the reimbursements of the employee (865ms)
                ✓ can re-add a removed employee (811ms)
              when the given end date is in the past
                ✓ reverts (66ms)
            when the employee end date was already set
              when the previous end date was not reached yet
                ✓ changes the employee end date (146ms)
              when the previous end date was reached
                ✓ reverts (102ms)
          when the sender does not have permissions to terminate employees
            ✓ reverts (90ms)
        when the given employee id does not exist
          ✓ reverts (95ms)
      when it has not been initialized yet
        ✓ reverts (51ms)

  Contract: Payroll token allocations
    determineAllocation
      when it has already been initialized
        when the employee exists
          when the employee is active
            when the amount of tokens and allocations match
              when the given list is not empty
                when all the given tokens are allowed
                  when the allocations add up to 100
                    when the allocation list does not include zero values
                      when there was no previous allocation
                        ✓ persists requested allocation (187ms)
                      when there was a previous allocation
                        ✓ replaces previous allocation for the requested one (187ms)
                    when the allocation list includes zero values
                      when there was no previous allocation
                        ✓ persists requested allocation (189ms)
                      when there was a previous allocation
                        ✓ replaces previous allocation for the requested one (189ms)
                  when the allocations add up less than 100
                    ✓ reverts (57ms)
                  when the allocations add up more than 100
                    ✓ reverts (53ms)
                when at least one token of the list is not allowed
                  ✓ reverts (61ms)
              when the given list is empty
                ✓ reverts (48ms)
            when the amount of tokens and allocations do not match
              ✓ reverts (41ms)
          when the employee is not active
            when the amount of tokens and allocations match
              when the given list is not empty
                when all the given tokens are allowed
                  when the allocations add up to 100
                    when the allocation list does not include zero values
                      when there was no previous allocation
                        ✓ persists requested allocation (538ms)
                      when there was a previous allocation
                        ✓ replaces previous allocation for the requested one (198ms)
                    when the allocation list includes zero values
                      when there was no previous allocation
                        ✓ persists requested allocation (207ms)
                      when there was a previous allocation
                        ✓ replaces previous allocation for the requested one (198ms)
                  when the allocations add up less than 100
                    ✓ reverts (87ms)
                  when the allocations add up more than 100
                    ✓ reverts (69ms)
                when at least one token of the list is not allowed
                  ✓ reverts (76ms)
              when the given list is empty
                ✓ reverts (60ms)
            when the amount of tokens and allocations do not match
              ✓ reverts (68ms)
        when the employee does not exist
          ✓ reverts (52ms)
      when it has not been initialized yet
        ✓ reverts (57ms)
    getAllocation
      when it has already been initialized
        when the employee exists
          when the employee is active
            when the given token is not the zero address
              when the given token was allowed
                when the given token was picked by the employee
                  ✓ tells its corresponding allocation (42ms)
                when the given token was not picked by the employee
                  ✓ returns 0 (42ms)
              when the given token was not allowed
                ✓ returns 0 (40ms)
            when the given token is the zero address
              when the given token was allowed
                when the given token was picked by the employee
                  ✓ tells its corresponding allocation (40ms)
                when the given token was not picked by the employee
                  ✓ returns 0
              when the given token was not allowed
                ✓ returns 0
          when the employee is not active
            when the given token is not the zero address
              when the given token was allowed
                when the given token was picked by the employee
                  ✓ tells its corresponding allocation
                when the given token was not picked by the employee
                  ✓ returns 0
              when the given token was not allowed
                ✓ returns 0
            when the given token is the zero address
              when the given token was allowed
                when the given token was picked by the employee
                  ✓ tells its corresponding allocation
                when the given token was not picked by the employee
                  ✓ returns 0
              when the given token was not allowed
                ✓ returns 0
        when the employee does not exist
          ✓ reverts
      when it has not been initialized yet
        ✓ reverts


  934 passing (36m)
```

## Coverage

```console
$ npm run coverage:payroll

> @aragon/monorepo-apps@1.0.0 coverage:payroll /home/daniel/Development/github.com/ConsenSys/aragon-payroll-audit-internal-2019-06/code/payroll
> lerna run --scope=@aragon/future-apps-payroll --concurrency=1 --stream coverage

@aragon/future-apps-payroll: > @aragon/future-apps-payroll@0.0.1 coverage /home/daniel/Development/github.com/ConsenSys/aragon-payroll-audit-internal-2019-06/code/payroll/future-apps/payroll
@aragon/future-apps-payroll: > SOLIDITY_COVERAGE=true npm run ganache-cli:test
@aragon/future-apps-payroll: > @aragon/future-apps-payroll@0.0.1 ganache-cli:test /home/daniel/Development/github.com/ConsenSys/aragon-payroll-audit-internal-2019-06/code/payroll/future-apps/payroll
@aragon/future-apps-payroll: > ./node_modules/@aragon/test-helpers/ganache-cli.sh
@aragon/future-apps-payroll: Starting testrpc-sc...
@aragon/future-apps-payroll: Running testrpc-sc with pid 13961 in port 8555
@aragon/future-apps-payroll: Measuring coverage...
@aragon/future-apps-payroll: Generating coverage environment
@aragon/future-apps-payroll: Running: truffle compile --network coverage 
@aragon/future-apps-payroll: (this can take a few seconds)...
@aragon/future-apps-payroll: Compiling ./contracts/Payroll.sol...
@aragon/future-apps-payroll: Compiling ./contracts/PayrollKit.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/TestImports.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/ExecutionTarget.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/MaliciousEmployee.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PayrollMock.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PriceFeedMock.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-finance/contracts/Finance.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-migrations/contracts/Migrations.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-vault/contracts/Vault.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACLOracle.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/APMNamehash.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/Repo.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AragonApp.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Autopetrified.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IForwarder.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Initializable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IsContract.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Petrifiable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/SafeERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/TimeHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/DAOFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/IKernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/Kernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/ENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath8.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/token/ERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/PPF.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/open-zeppelin/ECRecovery.sol...
@aragon/future-apps-payroll: Compiling @aragon/test-helpers/contracts/TimeHelpersMock.sol...
@aragon/future-apps-payroll: Compilation warnings encountered:
@aragon/future-apps-payroll: @aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function Controlled()  public { controller = msg.sender;}
@aragon/future-apps-payroll:     ^-------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function MiniMeToken(
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceFrom = balanceOfAt(_from, block.number);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceTo = balanceOfAt(_to, block.number);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:22:48: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (records[node].owner != msg.sender) throw;
@aragon/future-apps-payroll:                                                ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function ENS() public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:         ^---------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:44: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (ens.owner(node) != msg.sender) throw;
@aragon/future-apps-payroll:                                            ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function PublicResolver(AbstractENS ensAddr) public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var record = records[node];
@aragon/future-apps-payroll:         ^--------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:53: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (((contentType - 1) & contentType) != 0) throw;
@aragon/future-apps-payroll:                                                     ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setOwner(bytes32 node, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                     ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public constant returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                                           ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public constant returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setResolver(bytes32 node, address resolver) only_owner(node) public {
@aragon/future-apps-payroll:                                        ^--------------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function resolver(bytes32 node) public constant returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
@aragon/future-apps-payroll:                                   ^--------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function ttl(bytes32 node) public constant returns (uint64) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setAddr(bytes32 node, address addr) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function addr(bytes32 node) public constant returns (address ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setName(bytes32 node, string name) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^---------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function name(bytes32 node) public constant returns (string ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function hasPermission(address who, address where, bytes32 what, bytes how) public view returns (bool);
@aragon/future-apps-payroll:     ^-----------------------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function getScriptExecutor(bytes script) public view returns (IEVMScriptExecutor);
@aragon/future-apps-payroll:     ^--------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public view returns (bool);
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function forward(bytes evmCallScript) public;
@aragon/future-apps-payroll:     ^-------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_from, _to, _amount);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Approval(msg.sender, _spender, _amount);
@aragon/future-apps-payroll:         ^-------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewCloneToken(address(cloneToken), snapshot);
@aragon/future-apps-payroll:         ^------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(0, _owner, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_owner, 0, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
@aragon/future-apps-payroll:             controller.transfer(this.balance);
@aragon/future-apps-payroll:                                 ^----------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ClaimedTokens(_token, controller, balance);
@aragon/future-apps-payroll:         ^----------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function owner(bytes32 _node) public constant returns (address);
@aragon/future-apps-payroll:     ^--------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function resolver(bytes32 _node) public constant returns (address);
@aragon/future-apps-payroll:     ^-----------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function ttl(bytes32 _node) public constant returns (uint64);
@aragon/future-apps-payroll:     ^-----------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setOwner(bytes32 _node, address _owner) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setResolver(bytes32 _node, address _resolver) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setTTL(bytes32 _node, uint64 _ttl) public;
@aragon/future-apps-payroll:     ^-------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
@aragon/future-apps-payroll:         records[0].owner = msg.sender;
@aragon/future-apps-payroll:                 ^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(node, owner);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:                       ^--------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewOwner(node, label, owner);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewResolver(node, resolver);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewTTL(node, ttl);
@aragon/future-apps-payroll:         ^---------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         AddrChanged(node, addr);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ContentChanged(node, hash);
@aragon/future-apps-payroll:         ^------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NameChanged(node, name);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ABIChanged(node, contentType);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         PubkeyChanged(node, x, y);
@aragon/future-apps-payroll:         ^-----------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         TextChanged(node, key, key);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/VaultRecoverable.sol:49:34: Warning: Unused function parameter. Remove or comment out the variable name to silence this warning.
@aragon/future-apps-payroll:     function allowRecoverability(address token) public view returns (bool) {
@aragon/future-apps-payroll:                                  ^-----------^
@aragon/future-apps-payroll: ,@aragon/apps-finance/contracts/Finance.sol:840:5: Warning: Function state mutability can be restricted to pure
@aragon/future-apps-payroll:     function getMaxPeriodTransitions() internal view returns (uint64) { return MAX_UINT64; }
@aragon/future-apps-payroll:     ^--------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: Writing artifacts to ./build/contracts
@aragon/future-apps-payroll: Instrumenting  ./coverageEnv/contracts/Payroll.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/PayrollKit.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/test/mocks/ExecutionTarget.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/test/mocks/MaliciousEmployee.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/test/mocks/PayrollMock.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/test/mocks/PriceFeedMock.sol
@aragon/future-apps-payroll: Skipping instrumentation of  ./coverageEnv/contracts/test/TestImports.sol
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/@aragon/os/contracts/common/SafeERC20.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/eth-gas-reporter/mock/contracts/EtherRouter/EtherRouter.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/eth-gas-reporter/mock/contracts/Wallets/Wallet.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/eth-gas-reporter/node_modules/truffle/build/AssertAddressPayableArray.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/eth-gas-reporter/node_modules/truffle/build/NewSafeSend.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/solium/node_modules/solparse/test/doc_examples.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/solium/test/lib/rules/double-quotes/accept/double-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/solium/test/lib/rules/double-quotes/reject/single-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/solium/test/lib/rules/quotes/double-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/apps-vault/node_modules/solium/test/lib/rules/quotes/single-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/@aragon/os/contracts/common/SafeERC20.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/eth-gas-reporter/mock/contracts/EtherRouter/EtherRouter.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/eth-gas-reporter/mock/contracts/Wallets/Wallet.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/eth-gas-reporter/node_modules/truffle/build/AssertAddressPayableArray.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/eth-gas-reporter/node_modules/truffle/build/NewSafeSend.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/solium/node_modules/solparse/test/doc_examples.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/solium/test/lib/rules/double-quotes/accept/double-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/solium/test/lib/rules/double-quotes/reject/single-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/solium/test/lib/rules/quotes/double-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/apps-finance/node_modules/solium/test/lib/rules/quotes/single-quoted.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Warning: The file at ./coverageEnv/node_modules/@aragon/os/contracts/common/SafeERC20.sol was identified as a Solidity Contract, but did not parse correctly. You may ignore this warning if it is not a Solidity file, or your project does not use it
@aragon/future-apps-payroll: Running: truffle compile --network coverage 
@aragon/future-apps-payroll: (this can take a few seconds)...
@aragon/future-apps-payroll: Compiling ./contracts/Payroll.sol...
@aragon/future-apps-payroll: Compiling ./contracts/PayrollKit.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/TestImports.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/ExecutionTarget.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/MaliciousEmployee.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PayrollMock.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PriceFeedMock.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-finance/contracts/Finance.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-migrations/contracts/Migrations.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-vault/contracts/Vault.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACLOracle.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/APMNamehash.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/Repo.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AragonApp.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Autopetrified.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IForwarder.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Initializable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IsContract.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Petrifiable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/SafeERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/TimeHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/DAOFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/IKernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/Kernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/ENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath8.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/token/ERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/PPF.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/open-zeppelin/ECRecovery.sol...
@aragon/future-apps-payroll: Compiling @aragon/test-helpers/contracts/TimeHelpersMock.sol...
@aragon/future-apps-payroll: Compilation warnings encountered:
@aragon/future-apps-payroll: @aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function Controlled()  public { controller = msg.sender;}
@aragon/future-apps-payroll:     ^-------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function MiniMeToken(
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceFrom = balanceOfAt(_from, block.number);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceTo = balanceOfAt(_to, block.number);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:22:49: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (records[node].owner != msg.sender) {throw;}
@aragon/future-apps-payroll:                                                 ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function ENS() public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:         ^---------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:45: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (ens.owner(node) != msg.sender) {throw;}
@aragon/future-apps-payroll:                                             ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function PublicResolver(AbstractENS ensAddr) public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var record = records[node];
@aragon/future-apps-payroll:         ^--------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:54: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (((contentType - 1) & contentType) != 0) {throw;}
@aragon/future-apps-payroll:                                                      ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setOwner(bytes32 node, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                     ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                                           ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setResolver(bytes32 node, address resolver) only_owner(node) public {
@aragon/future-apps-payroll:                                        ^--------------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function resolver(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
@aragon/future-apps-payroll:                                   ^--------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function ttl(bytes32 node) public  returns (uint64) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setAddr(bytes32 node, address addr) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function addr(bytes32 node) public  returns (address ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setName(bytes32 node, string name) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^---------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function name(bytes32 node) public  returns (string ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function hasPermission(address who, address where, bytes32 what, bytes how) public  returns (bool);
@aragon/future-apps-payroll:     ^-------------------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function getScriptExecutor(bytes script) public  returns (IEVMScriptExecutor);
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function forward(bytes evmCallScript) public;
@aragon/future-apps-payroll:     ^-------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_from, _to, _amount);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Approval(msg.sender, _spender, _amount);
@aragon/future-apps-payroll:         ^-------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewCloneToken(address(cloneToken), snapshot);
@aragon/future-apps-payroll:         ^------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(0, _owner, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_owner, 0, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
@aragon/future-apps-payroll:             controller.transfer(this.balance);
@aragon/future-apps-payroll:                                 ^----------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ClaimedTokens(_token, controller, balance);
@aragon/future-apps-payroll:         ^----------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function owner(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function resolver(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^---------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function ttl(bytes32 _node) public  returns (uint64);
@aragon/future-apps-payroll:     ^---------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setOwner(bytes32 _node, address _owner) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setResolver(bytes32 _node, address _resolver) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setTTL(bytes32 _node, uint64 _ttl) public;
@aragon/future-apps-payroll:     ^-------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
@aragon/future-apps-payroll:         records[0].owner = msg.sender;
@aragon/future-apps-payroll:                 ^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(node, owner);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:                       ^--------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewOwner(node, label, owner);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewResolver(node, resolver);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewTTL(node, ttl);
@aragon/future-apps-payroll:         ^---------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         AddrChanged(node, addr);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ContentChanged(node, hash);
@aragon/future-apps-payroll:         ^------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NameChanged(node, name);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ABIChanged(node, contentType);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         PubkeyChanged(node, x, y);
@aragon/future-apps-payroll:         ^-----------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         TextChanged(node, key, key);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: @aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function Controlled()  public { controller = msg.sender;}
@aragon/future-apps-payroll:     ^-------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function MiniMeToken(
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceFrom = balanceOfAt(_from, block.number);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceTo = balanceOfAt(_to, block.number);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:22:49: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (records[node].owner != msg.sender) {throw;}
@aragon/future-apps-payroll:                                                 ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function ENS() public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:         ^---------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:45: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (ens.owner(node) != msg.sender) {throw;}
@aragon/future-apps-payroll:                                             ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function PublicResolver(AbstractENS ensAddr) public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var record = records[node];
@aragon/future-apps-payroll:         ^--------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:54: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (((contentType - 1) & contentType) != 0) {throw;}
@aragon/future-apps-payroll:                                                      ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setOwner(bytes32 node, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                     ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                                           ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setResolver(bytes32 node, address resolver) only_owner(node) public {
@aragon/future-apps-payroll:                                        ^--------------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function resolver(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
@aragon/future-apps-payroll:                                   ^--------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function ttl(bytes32 node) public  returns (uint64) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setAddr(bytes32 node, address addr) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function addr(bytes32 node) public  returns (address ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setName(bytes32 node, string name) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^---------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function name(bytes32 node) public  returns (string ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function hasPermission(address who, address where, bytes32 what, bytes how) public  returns (bool);
@aragon/future-apps-payroll:     ^-------------------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function getScriptExecutor(bytes script) public  returns (IEVMScriptExecutor);
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function forward(bytes evmCallScript) public;
@aragon/future-apps-payroll:     ^-------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_from, _to, _amount);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Approval(msg.sender, _spender, _amount);
@aragon/future-apps-payroll:         ^-------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewCloneToken(address(cloneToken), snapshot);
@aragon/future-apps-payroll:         ^------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(0, _owner, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_owner, 0, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
@aragon/future-apps-payroll:             controller.transfer(this.balance);
@aragon/future-apps-payroll:                                 ^----------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ClaimedTokens(_token, controller, balance);
@aragon/future-apps-payroll:         ^----------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function owner(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function resolver(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^---------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function ttl(bytes32 _node) public  returns (uint64);
@aragon/future-apps-payroll:     ^---------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setOwner(bytes32 _node, address _owner) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setResolver(bytes32 _node, address _resolver) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setTTL(bytes32 _node, uint64 _ttl) public;
@aragon/future-apps-payroll:     ^-------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
@aragon/future-apps-payroll:         records[0].owner = msg.sender;
@aragon/future-apps-payroll:                 ^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(node, owner);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:                       ^--------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewOwner(node, label, owner);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewResolver(node, resolver);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewTTL(node, ttl);
@aragon/future-apps-payroll:         ^---------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         AddrChanged(node, addr);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ContentChanged(node, hash);
@aragon/future-apps-payroll:         ^------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NameChanged(node, name);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ABIChanged(node, contentType);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         PubkeyChanged(node, x, y);
@aragon/future-apps-payroll:         ^-----------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         TextChanged(node, key, key);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-token-manager/contracts/TokenManager.sol:327:5: TypeError: Overriding function changes state mutability from "nonpayable" to "view".
@aragon/future-apps-payroll:     function allowRecoverability(address _token) public view returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/os/contracts/common/VaultRecoverable.sol:49:5: Overriden function is here:
@aragon/future-apps-payroll:     function allowRecoverability(address token) public  returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-token-manager/contracts/TokenManager.sol:227:5: TypeError: Overriding function changes state mutability from "nonpayable" to "view".
@aragon/future-apps-payroll:     function canForward(address _sender, bytes) public view returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/os/contracts/common/IForwarder.sol:13:5: Overriden function is here:
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,/home/daniel/Development/github.com/ConsenSys/aragon-payroll-audit-internal-2019-06/code/payroll/future-apps/payroll/coverageEnv/contracts/PayrollKit.sol:21:3: TypeError: Overriding function changes state mutability from "view" to "nonpayable".
@aragon/future-apps-payroll:   function get(address, address) external  returns (uint128 xrt, uint64 when) {
@aragon/future-apps-payroll:   ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/ppf-contracts/contracts/IFeed.sol:4:5: Overriden function is here:
@aragon/future-apps-payroll:     function get(address base, address quote) external view returns (uint128 xrt, uint64 when);
@aragon/future-apps-payroll:     ^-----------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: [31mCompilation failed. See above.[39m
@aragon/future-apps-payroll: Running: truffle test --network coverage 
@aragon/future-apps-payroll: (this can take a few seconds)...
@aragon/future-apps-payroll: Compiling ./contracts/Payroll.sol...
@aragon/future-apps-payroll: Compiling ./contracts/PayrollKit.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/TestImports.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/ExecutionTarget.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/MaliciousEmployee.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PayrollMock.sol...
@aragon/future-apps-payroll: Compiling ./contracts/test/mocks/PriceFeedMock.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-finance/contracts/Finance.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-migrations/contracts/Migrations.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/ITokenController.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-shared-minime/contracts/MiniMeToken.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-token-manager/contracts/TokenManager.sol...
@aragon/future-apps-payroll: Compiling @aragon/apps-vault/contracts/Vault.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/ACLSyntaxSugar.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACL.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/acl/IACLOracle.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/APMNamehash.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apm/Repo.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyBase.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyPinned.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppProxyUpgradeable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AppStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/apps/AragonApp.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Autopetrified.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ConversionHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableDelegateProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/DepositableStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/EtherTokenConstant.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IForwarder.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IVaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Initializable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/IsContract.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Petrifiable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/ReentrancyGuard.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/SafeERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/TimeHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/Uint256Helpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/UnstructuredStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/common/VaultRecoverable.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/EVMScriptRunner.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/IEVMScriptRegistry.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/ScriptHelpers.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/BaseEVMScriptExecutor.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/evmscript/executors/CallsScript.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/AppProxyFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/DAOFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/factory/EVMScriptRegistryFactory.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/IKernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/Kernel.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelConstants.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/kernel/KernelStorage.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/AbstractENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/ENS.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/ens/PublicResolver.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath64.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/math/SafeMath8.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/misc/ERCProxy.sol...
@aragon/future-apps-payroll: Compiling @aragon/os/contracts/lib/token/ERC20.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/IFeed.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/PPF.sol...
@aragon/future-apps-payroll: Compiling @aragon/ppf-contracts/contracts/open-zeppelin/ECRecovery.sol...
@aragon/future-apps-payroll: Compiling @aragon/test-helpers/contracts/TimeHelpersMock.sol...
@aragon/future-apps-payroll: Compilation warnings encountered:
@aragon/future-apps-payroll: @aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function Controlled()  public { controller = msg.sender;}
@aragon/future-apps-payroll:     ^-------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function MiniMeToken(
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceFrom = balanceOfAt(_from, block.number);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceTo = balanceOfAt(_to, block.number);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:22:49: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (records[node].owner != msg.sender) {throw;}
@aragon/future-apps-payroll:                                                 ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function ENS() public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:         ^---------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:45: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (ens.owner(node) != msg.sender) {throw;}
@aragon/future-apps-payroll:                                             ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function PublicResolver(AbstractENS ensAddr) public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var record = records[node];
@aragon/future-apps-payroll:         ^--------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:54: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (((contentType - 1) & contentType) != 0) {throw;}
@aragon/future-apps-payroll:                                                      ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setOwner(bytes32 node, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                     ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                                           ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setResolver(bytes32 node, address resolver) only_owner(node) public {
@aragon/future-apps-payroll:                                        ^--------------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function resolver(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
@aragon/future-apps-payroll:                                   ^--------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function ttl(bytes32 node) public  returns (uint64) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setAddr(bytes32 node, address addr) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function addr(bytes32 node) public  returns (address ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setName(bytes32 node, string name) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^---------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function name(bytes32 node) public  returns (string ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function hasPermission(address who, address where, bytes32 what, bytes how) public  returns (bool);
@aragon/future-apps-payroll:     ^-------------------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function getScriptExecutor(bytes script) public  returns (IEVMScriptExecutor);
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function forward(bytes evmCallScript) public;
@aragon/future-apps-payroll:     ^-------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_from, _to, _amount);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Approval(msg.sender, _spender, _amount);
@aragon/future-apps-payroll:         ^-------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewCloneToken(address(cloneToken), snapshot);
@aragon/future-apps-payroll:         ^------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(0, _owner, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_owner, 0, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
@aragon/future-apps-payroll:             controller.transfer(this.balance);
@aragon/future-apps-payroll:                                 ^----------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ClaimedTokens(_token, controller, balance);
@aragon/future-apps-payroll:         ^----------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function owner(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function resolver(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^---------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function ttl(bytes32 _node) public  returns (uint64);
@aragon/future-apps-payroll:     ^---------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setOwner(bytes32 _node, address _owner) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setResolver(bytes32 _node, address _resolver) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setTTL(bytes32 _node, uint64 _ttl) public;
@aragon/future-apps-payroll:     ^-------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
@aragon/future-apps-payroll:         records[0].owner = msg.sender;
@aragon/future-apps-payroll:                 ^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(node, owner);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:                       ^--------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewOwner(node, label, owner);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewResolver(node, resolver);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewTTL(node, ttl);
@aragon/future-apps-payroll:         ^---------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         AddrChanged(node, addr);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ContentChanged(node, hash);
@aragon/future-apps-payroll:         ^------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NameChanged(node, name);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ABIChanged(node, contentType);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         PubkeyChanged(node, x, y);
@aragon/future-apps-payroll:         ^-----------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         TextChanged(node, key, key);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: @aragon/apps-shared-minime/contracts/MiniMeToken.sol:37:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function Controlled()  public { controller = msg.sender;}
@aragon/future-apps-payroll:     ^-------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:123:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function MiniMeToken(
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:195:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceFrom = balanceOfAt(_from, block.number);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:209:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var previousBalanceTo = balanceOfAt(_to, block.number);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:22:49: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (records[node].owner != msg.sender) {throw;}
@aragon/future-apps-payroll:                                                 ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:29:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function ENS() public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:         ^---------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:45:45: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (ens.owner(node) != msg.sender) {throw;}
@aragon/future-apps-payroll:                                             ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:53:5: Warning: Defining constructors as functions with the same name as the contract is deprecated. Use "constructor(...) { ... }" instead.
@aragon/future-apps-payroll:     function PublicResolver(AbstractENS ensAddr) public {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:146:9: Warning: Use of the "var" keyword is deprecated.
@aragon/future-apps-payroll:         var record = records[node];
@aragon/future-apps-payroll:         ^--------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:166:54: Warning: "throw" is deprecated in favour of "revert()", "require()" and "assert()".
@aragon/future-apps-payroll:         if (((contentType - 1) & contentType) != 0) {throw;}
@aragon/future-apps-payroll:                                                      ^---^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:60:37: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setOwner(bytes32 node, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                     ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:72:59: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 node, bytes32 label, address owner) only_owner(node) public {
@aragon/future-apps-payroll:                                                           ^-----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:36:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function owner(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:83:40: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setResolver(bytes32 node, address resolver) only_owner(node) public {
@aragon/future-apps-payroll:                                        ^--------------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:43:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function resolver(bytes32 node) public  returns (address) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:93:35: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setTTL(bytes32 node, uint64 ttl) only_owner(node) public {
@aragon/future-apps-payroll:                                   ^--------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/ENS.sol:50:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function ttl(bytes32 node) public  returns (uint64) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:87:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setAddr(bytes32 node, address addr) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^----------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:77:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function addr(bytes32 node) public  returns (address ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:132:36: Warning: This declaration shadows an existing declaration.
@aragon/future-apps-payroll:     function setName(bytes32 node, string name) only_owner(node) public {
@aragon/future-apps-payroll:                                    ^---------^
@aragon/future-apps-payroll: @aragon/os/contracts/lib/ens/PublicResolver.sol:122:5: The shadowed declaration is here:
@aragon/future-apps-payroll:     function name(bytes32 node) public  returns (string ret) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/os/contracts/acl/IACL.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function hasPermission(address who, address where, bytes32 what, bytes how) public  returns (bool);
@aragon/future-apps-payroll:     ^-------------------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/evmscript/IEVMScriptRegistry.sol:24:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function getScriptExecutor(bytes script) public  returns (IEVMScriptExecutor);
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/common/IForwarder.sol:17:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function forward(bytes evmCallScript) public;
@aragon/future-apps-payroll:     ^-------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:213:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_from, _to, _amount);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:245:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Approval(msg.sender, _spender, _amount);
@aragon/future-apps-payroll:         ^-------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:373:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewCloneToken(address(cloneToken), snapshot);
@aragon/future-apps-payroll:         ^------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:392:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(0, _owner, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:408:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(_owner, 0, _amount);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:509:33: Warning: Using contract member "balance" inherited from the address type is deprecated. Convert the contract to "address" type to access the member, for example use "address(contract).balance" instead.
@aragon/future-apps-payroll:             controller.transfer(this.balance);
@aragon/future-apps-payroll:                                 ^----------^
@aragon/future-apps-payroll: ,@aragon/apps-shared-minime/contracts/MiniMeToken.sol:516:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ClaimedTokens(_token, controller, balance);
@aragon/future-apps-payroll:         ^----------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:7:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function owner(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:8:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function resolver(bytes32 _node) public  returns (address);
@aragon/future-apps-payroll:     ^---------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:9:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function ttl(bytes32 _node) public  returns (uint64);
@aragon/future-apps-payroll:     ^---------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:10:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setOwner(bytes32 _node, address _owner) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:11:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setSubnodeOwner(bytes32 _node, bytes32 label, address _owner) public;
@aragon/future-apps-payroll:     ^----------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:12:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setResolver(bytes32 _node, address _resolver) public;
@aragon/future-apps-payroll:     ^------------------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/AbstractENS.sol:13:5: Warning: Functions in interfaces should be declared external.
@aragon/future-apps-payroll:     function setTTL(bytes32 _node, uint64 _ttl) public;
@aragon/future-apps-payroll:     ^-------------------------------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:30:17: Warning: Decimal literal assigned to bytesXX variable will be left-aligned. Use an explicit conversion to silence this warning.
@aragon/future-apps-payroll:         records[0].owner = msg.sender;
@aragon/future-apps-payroll:                 ^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:61:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         Transfer(node, owner);
@aragon/future-apps-payroll:         ^-------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:73:23: Warning: This function only accepts a single "bytes" argument. Please use "abi.encodePacked(...)" or a similar function to encode the data.
@aragon/future-apps-payroll:         var subnode = keccak256(node, label);
@aragon/future-apps-payroll:                       ^--------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:74:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewOwner(node, label, owner);
@aragon/future-apps-payroll:         ^--------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:84:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewResolver(node, resolver);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/ENS.sol:94:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NewTTL(node, ttl);
@aragon/future-apps-payroll:         ^---------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:89:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         AddrChanged(node, addr);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:113:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ContentChanged(node, hash);
@aragon/future-apps-payroll:         ^------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:134:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         NameChanged(node, name);
@aragon/future-apps-payroll:         ^---------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:169:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         ABIChanged(node, contentType);
@aragon/future-apps-payroll:         ^---------------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:190:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         PubkeyChanged(node, x, y);
@aragon/future-apps-payroll:         ^-----------------------^
@aragon/future-apps-payroll: ,@aragon/os/contracts/lib/ens/PublicResolver.sol:212:9: Warning: Invoking events without "emit" prefix is deprecated.
@aragon/future-apps-payroll:         TextChanged(node, key, key);
@aragon/future-apps-payroll:         ^-------------------------^
@aragon/future-apps-payroll: ,@aragon/apps-token-manager/contracts/TokenManager.sol:327:5: TypeError: Overriding function changes state mutability from "nonpayable" to "view".
@aragon/future-apps-payroll:     function allowRecoverability(address _token) public view returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/os/contracts/common/VaultRecoverable.sol:49:5: Overriden function is here:
@aragon/future-apps-payroll:     function allowRecoverability(address token) public  returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: ,@aragon/apps-token-manager/contracts/TokenManager.sol:227:5: TypeError: Overriding function changes state mutability from "nonpayable" to "view".
@aragon/future-apps-payroll:     function canForward(address _sender, bytes) public view returns (bool) {
@aragon/future-apps-payroll:     ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/os/contracts/common/IForwarder.sol:13:5: Overriden function is here:
@aragon/future-apps-payroll:     function canForward(address sender, bytes evmCallScript) public  returns (bool);
@aragon/future-apps-payroll:     ^------------------------------------------------------------------------------^
@aragon/future-apps-payroll: ,/home/daniel/Development/github.com/ConsenSys/aragon-payroll-audit-internal-2019-06/code/payroll/future-apps/payroll/coverageEnv/contracts/PayrollKit.sol:21:3: TypeError: Overriding function changes state mutability from "view" to "nonpayable".
@aragon/future-apps-payroll:   function get(address, address) external  returns (uint128 xrt, uint64 when) {
@aragon/future-apps-payroll:   ^ (Relevant source part starts here and spans across multiple lines).
@aragon/future-apps-payroll: @aragon/ppf-contracts/contracts/IFeed.sol:4:5: Overriden function is here:
@aragon/future-apps-payroll:     function get(address base, address quote) external view returns (uint128 xrt, uint64 when);
@aragon/future-apps-payroll:     ^-----------------------------------------------------------------------------------------^
@aragon/future-apps-payroll: [31mCompilation failed. See above.[39m
@aragon/future-apps-payroll: Cleaning up...
@aragon/future-apps-payroll: Event trace could not be read.
@aragon/future-apps-payroll: Error: ENOENT: no such file or directory, open './allFiredEvents'
@aragon/future-apps-payroll: Exiting without generating coverage...
```