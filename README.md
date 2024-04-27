# Smart Contract Security Audit Report

This repository contains the audit report of the `StorageVictim` smart contract, along with the corrected and updated version of the contract, `StorageSecured`

## Description

The StorageVictim smart contract was written in Solidity and contains 1 critical vulnerability, 1 medium vulnerability, and 2 informational vulnerabilities. The audit report provides a detailed explanation of these vulnerabilities and their fixes. The updated and corrected version of the StorageVictim contract is available in the src folder.

## Audit Findings

- **Critical Vulnerabilities:** These are severe issues that can lead to significant security risks. For example, the contract had an uninitialized pointer vulnerability, where the Storage pointer str was not initialized, leading to potential security issues. The fix involved initializing `str` to Storage memory str; in the `store` and `getStore` functions.

- **Medium Vulnerabilities:** These are moderate issues that can potentially lead to security risks. For instance, the contract used an outdated version of the Solidity compiler, which could introduce vulnerabilities and compatibility issues. The fix involved updating the Solidity compiler version to a more recent one.

- **Informational Vulnerabilities:** These are issues that, while not severe, should be addressed for better code quality and readability. For example, the contract lacked a SPDX-License-Identifier, which could cause issues in certain development environments. The fix involved adding a specified License identifier.

## Full Audit Report

The full audit report is available here, `./AuditReport`

## Demo Video

https://www.loom.com/share/836289c9156d4415abd38c2100c93523?sid=d009440f-83b6-4f9d-91d1-13e9a77fad10

## Author

Ugo Mars
[@metacraftersio](https://github.com/UgoMars)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
