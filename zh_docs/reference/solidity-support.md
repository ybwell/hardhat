# Solidity 支持

Hardhat 内置网络（Hardhat Network）拥有一流的Solidity支持。它总是知道哪些智能合约正在运行，它们具体做什么，以及它们为什么会失败，这些使开发智能合约更容易。

为了这些支持，Hardhat与Solidity进行了深入整合，这意味着新的Solidity版本并不是自动支持的。

本文档解释了目前支持哪些Solidity版本，以及如果你使用不支持的版本会发生什么。

## 支持的版本

这些是与Hardhat完全兼容的Solidity版本：

- 从 0.5.1 开始的任何 0.5.x 版本
- 任何 0.6.x 版本
- 任何 0.7.x 版本

我们不太建议在较新的、不支持的 Solidity 版本中使用 Hardhat，但如果你需要，请继续阅读。


### 使用不支持的版本

当运行一个不支持的 Solidity 版本时，Hardhat集成的功能可能不起作用，或者运行不正确。

如 Solidity 堆栈跟踪可能停止工作、不正确或不完整。也可能是 `console.log` 停止工作。

尽管这些可能被破坏，但智能合约的实际编译和执行不会受到影响。
合约的实际编译和执行不会受到影响。你仍然可以相信测试结果或部署的智能合约。
只是在此时，你从Hardhat得到的帮助会减少。

