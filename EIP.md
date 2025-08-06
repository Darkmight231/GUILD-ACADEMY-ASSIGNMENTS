# EIP-9999: Gas Should be returned on all failed transactions
Authors     Sanni Mujeeb(@smoch1037)

Created     2025-08-02
## Table of contents
- Abstract
- Motivation
- Rationale
- Security Considerations
- Copyrights


## Abstract
This proposal identifies a common issue faced by contract creator or message calls when their transaction fails midway, they keep paying gas fee up till where there contract fails, they are no having a successful transaction and they are still loosing money, it shouldnt be so.

## Motivation
In the case of a executing a message call or creating a contract, if the execution halts in a an exceptional fashion then no gas is refunded to the caller and the state is reverted to the point immediately prior to balance transfer


## Rationale
The reason for considering this approach is to make sure gas fee are been refunded to creators of contract or message callers when their transaction revert midway, the usual method of deducting the gas fee up until the point the contract reverted should be abrogated and for every failed transaction, sender should receive their full money.


## Security Considerations
No security considerations

## Copyrights
Copyrights and related rights waived via CCO
