# EEI Tests

Each test case should have:

- wasm bytecode
- account / block / tx state
- expected return or revert data

The following methods must be tested:

- useGas
- getAddress
- getBalance
- getBlockHash
- call
- callDataCopy
- getCallDataSize
- callCode
- callDelegate
- storageStore
- storageLoad
- getCaller
- getCallValue
- codeCopy
- getCodeSize
- getBlockCoinbase
- create
- getBlockDifficulty
- externalCodeCopy
- getExternalCodeSize
- getGasLeft
- getBlockGasLimit
- getTxGasPrice
- log
- getBlockNumber
- getTxOrigin
- return
- selfDestruct
- getBlockTimestamp

I'd suggest to start with return and then the others can use it to return data thus reduce the complexity of checking the test's output.
