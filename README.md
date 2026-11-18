# mini-cs-framework

基于 Socket 的客户端 / 服务端骨架。服务端收消息、分发命令、维持会话；客户端发请求并挂上自己的动作回调。

写于 2020 年，用来把一套可复用的 C/S 通信壳从业务里拆出来。

## 里面有什么

- `Server`：监听、线程池、临时会话和正式会话
- `Client`：读配置、连接、`sentRequest` 发请求
- `CommandDistributor`：按命令把消息分出去
- `@ActionMethod`、`@ActionPara`、`@HasActionMethod`：把方法和网络动作标出来

源码在 `clientserver简单实现/src`，核心包 `com.mec.CS_Frame_Work`。目录是当时的 Eclipse 工程，没有 Maven 或 Gradle。

## 状态

学习代码，源码按最初上传的样子保留。仓库曾用名 `easyCSFrameWork`，旧地址会重定向到这里。
