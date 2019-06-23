# Solium / Ethlint result

## Payroll

```
future-apps/payroll/contracts/Payroll.sol
  827:10    error    Only use indent of 8 spaces.    indentation

future-apps/payroll/contracts/PayrollKit.sol
  21:2      error      Only use indent of 4 spaces.                       indentation
  23:20     warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members
  24:0      error      Only use indent of 4 spaces.                       indentation
  220:50    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members
  234:54    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members
  235:54    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members
  236:54    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members
  237:54    warning    Avoid using 'now' (alias to 'block.timestamp').    security/no-block-members

future-apps/payroll/contracts/test/mocks/MaliciousEmployee.sol
  77:8    warning    Provide an error message for require().    error-reason
  84:8    warning    Provide an error message for require().    error-reason
  85:8    warning    Provide an error message for require().    error-reason
  96:8    warning    Provide an error message for require().    error-reason
  97:8    warning    Provide an error message for require().    error-reason
  98:8    warning    Provide an error message for require().    error-reason

future-apps/payroll/contracts/test/mocks/PriceFeedMock.sol
  26:8    warning    Provide an error message for require().    error-reason
  27:8    warning    Provide an error message for require().    error-reason
  30:8    warning    Provide an error message for require().    error-reason

✖ 3 errors, 15 warnings found.
```


## ppf-contract

```
ppf-contracts/packages/ppf-contracts/contracts/PPF.sol
  96:12    error    Avoid using Inline Assembly.    security/no-inline-assembly

ppf-contracts/packages/ppf-contracts/contracts/misc/Migrations.sol
  4:2     error    Only use indent of 4 spaces.    indentation
  5:2     error    Only use indent of 4 spaces.    indentation
  7:2     error    Only use indent of 4 spaces.    indentation
  9:0     error    Only use indent of 4 spaces.    indentation
  11:2    error    Only use indent of 4 spaces.    indentation
  13:0    error    Only use indent of 4 spaces.    indentation
  15:2    error    Only use indent of 4 spaces.    indentation
  17:0    error    Only use indent of 4 spaces.    indentation
  19:2    error    Only use indent of 4 spaces.    indentation
  22:0    error    Only use indent of 4 spaces.    indentation

ppf-contracts/packages/ppf-contracts/contracts/open-zeppelin/ECRecovery.sol
  12:2     error    Only use indent of 4 spaces.    indentation
  14:0     error    Only use indent of 4 spaces.    indentation
  21:2     error    Only use indent of 4 spaces.    indentation
  28:6     error    Only use indent of 8 spaces.    indentation
  32:4     error    Avoid using Inline Assembly.    security/no-inline-assembly
  40:6     error    Only use indent of 8 spaces.    indentation
  45:6     error    Only use indent of 8 spaces.    indentation
  47:6     error    Only use indent of 8 spaces.    indentation
  49:0     error    Only use indent of 4 spaces.    indentation
  56:2     error    Only use indent of 4 spaces.    indentation
  63:21    error    Only use indent of 8 spaces.    indentation
  67:0     error    Only use indent of 4 spaces.    indentation

✖ 23 errors found.
```