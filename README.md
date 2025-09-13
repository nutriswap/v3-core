# Nutriswap V3 Core

[![Lint](https://github.com/nutriswap/v3-core/actions/workflows/lint.yml/badge.svg)](https://github.com/nutriswap/v3-core/actions/workflows/lint.yml)
[![Tests](https://github.com/nutriswap/v3-core/actions/workflows/tests.yml/badge.svg)](https://github.com/nutriswap/v3-core/actions/workflows/tests.yml)
[![Fuzz Testing](https://github.com/nutriswap/v3-core/actions/workflows/fuzz-testing.yml/badge.svg)](https://github.com/nutriswap/v3-core/actions/workflows/fuzz-testing.yml)

This repository contains the **core smart contracts** for the **Nutriswap V3 Protocol**.  
For higher level contracts (periphery contracts such as routers), see the [nutriswap-v3-periphery](https://github.com/nutriswap/v3-periphery) repository.

---

## Local deployment

To deploy this code to a local testnet, install the npm package  
`@nutriswap/v3-core` and import the factory bytecode located at:

```typescript
import {
  abi as FACTORY_ABI,
  bytecode as FACTORY_BYTECODE,
} from '@nutriswap/v3-core/artifacts/contracts/UniswapV3Factory.sol/UniswapV3Factory.json'

// deploy the bytecode
