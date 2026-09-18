# BuyBench

**Celo Agents at Work Hackathon — Track 5: Best Feedback for buy**

## Project Overview

BuyBench tested the buyer-side experience of the Buy marketplace by completing a real Google Cloud VM purchase through the Buy protocol on Celo mainnet.

## Test Environment

- **Buy CLI**: v0.5.0
- **Node.js**: v22.22.1
- **Operating System**: Windows with WSL Ubuntu
- **Network**: Celo mainnet

## Environment Findings

- **Windows Schannel certificate-revocation error**: Prevented direct Buy CLI usage on native Windows; diagnosed with `--ssl-no-revoke` flag
- **WSL Ubuntu**: Successfully resolved HTTPS/DNS issues for Buy operations
- **Conclusion**: WSL environment provides stable Buy CLI functionality on Windows hosts

## Test Execution

### Purchase Details

- **Service**: Google Cloud VM
- **Machine Type**: e2-micro
- **Rental Duration**: 1 hour
- **Zone**: us-west1-a
- **Quote/Payment**: 0.016753 USDT (~$0.017 USD)

### Transaction Information

- **Transaction Hash**: `0xf96a64dc18f173ca59c9ca7f63aec252f571c4027fd32374e7a11b9c058a22e1`
- **VM Instance**: cpay-f96a64dc18f1
- **Token**: USDT

### Script Execution

- **Script**: `echo test`
- **Result**: `test`
- **Payment-to-Result Time**: ~15 seconds

## ERC-8004 Agent Information

- **Agent ID**: 9770

## Public Feedback

Track 5 feedback filed to celo-org/buy-skill repository:
https://github.com/celo-org/buy-skill/issues/28

## Conclusion

The Buy marketplace was successfully tested end-to-end, demonstrating functional buyer-side VM rental, payment settlement, and script execution through the Buy protocol on Celo mainnet. The test confirmed both the technical feasibility of the service and provided valuable environment feedback for Windows/WSL users.
