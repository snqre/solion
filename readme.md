# Solion
## A Type-Safe Solidity Compiler
```ts
Compiler().compile({
    language: "Solidity",
    sources: {
        "counter": {
            content: `
                /// ...
            `
        },
    },
    settings: {
        optimizer: {
            enabled: true,
            runs: 200
        },
        evmVersion: "istanbul",
        outputSelection: {
            "*": {
                "*": [
                    "abi",
                    "ast",
                    "evm.bytecode.object",
                ],
            },
        },
    }
})
```