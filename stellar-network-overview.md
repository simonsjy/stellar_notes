# stellar架构

使用stellar网络可，你可以建立移动钱包、银行工具、用来支付的只能设备等，甚至是任何你可以想到的雨支付相关的东西。虽然stellar是一个复杂的分布式网络，但使用起来却并不复杂。

## API: Horizon {#api-horizon}

Horizon是一个RESTful HTTP API 服务， 绝大多数的应用都通过Horizon与stellar网络进行交互，它提供了一个直接的方式来提交交易、检查账户和订阅事件。因为它是HTTP，所以你可以通过web浏览器、cURL这样的简单命令行工具或者Stellar sdk进行交互。

安装Horizon的方式：[**stellar/quickstart**docker image](https://hub.docker.com/r/stellar/quickstart/)

.Stellar官方维护着JavaSript,Java和GO语言的sdk，Ruby,Python和C\#的sdk由社区维护。

## 网络主干：Stellar Core

每一个Horizon 服务器都会连接一个stellar core.Stellar core 使用[Stellar Consensus Protocol](https://www.stellar.org/developers/guides/concepts/scp.html)\(SCP\)完成与其他core实例对交易状态的验证和一致。stellar网络连接着遍布世界的独立实体。一些实例拥有Horizon使得用户可以访问，而一些实例并没有Horizon，它们的存在是为了提高整个网络的可靠性。

安装Stellar Core的方式：[**stellar/quickstart**docker image](https://hub.docker.com/r/stellar/quickstart/)

.



