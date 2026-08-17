# Awesome 游戏服务器资源大全 with stars

***

### 目录

* [游戏服务器资源大全](#游戏服务器资源大全)
  * [网络](#网络)
  * [协议](#协议)
  * [持久化](#持久化)
  * [缓存与消息队列](#缓存与消息队列)
  * [Log](#log)
  * [游戏AI](#游戏ai)
  * [工具库](#工具库)
  * [开源服务器](#开源服务器)
  * [容器与编排](#容器与编排)
  * [运维](#运维)
  * [学习资源](#学习资源)
  * [其他](#其他)

### 网络

*网络相关的库和工具*

* Java
  * [Netty](https://github.com/netty/netty) ⭐ 35,035 | 🐛 660 | 🌐 Java | 📅 2026-08-17 - Netty是一个高性能、异步事件驱动的NIO框架，它提供了对TCP、UDP和文件传输的支持
  * [Mina](https://github.com/apache/mina) ⭐ 924 | 🐛 5 | 🌐 Java | 📅 2026-08-17 - Apache Mina是一个能够帮助用户开发高性能和高伸缩性网络应用程序的框架
* C++
  * [libuv](https://github.com/libuv/libuv) ⭐ 27,113 | 🐛 228 | 🌐 C | 📅 2026-08-17 - libuv 是 Node 的新跨平台抽象层,用于抽象 Windows 的 IOCP 及 Unix 的 libev
  * [KCP](https://github.com/skywind3000/kcp) ⭐ 16,873 | 🐛 195 | 🌐 C | 📅 2026-06-23 - 快速可靠的 ARQ 协议，比 TCP 浪费带宽换低延迟
  * [muduo](https://github.com/chenshuo/muduo) ⭐ 16,224 | 🐛 86 | 🌐 C++ | 📅 2025-12-23 - 陈硕出品的基于 Reactor 模式的现代 C++ 网络库
  * [asio](https://github.com/chriskohlhoff/asio) ⭐ 6,163 | 🐛 985 | 🌐 C++ | 📅 2026-07-18 - 跨平台 C++ 网络与底层 I/O 库，Boost.Asio 的独立版本
  * [evpp](https://github.com/Qihoo360/evpp) ⭐ 3,774 | 🐛 150 | 🌐 C++ | 📅 2024-04-10 - 360 出品的现代 C++ 高性能网络库
  * [enet](https://github.com/lsalzman/enet) ⭐ 3,251 | 🐛 98 | 🌐 C | 📅 2026-06-23 - 面向游戏的可靠 UDP 网络库
  * [libevent](http://libevent.org/) - libevent是一个轻量级的基于事件驱动的高性能的开源网络库,并且支持多个平台
  * [libev](http://software.schmorp.de/pkg/libev.html) - 较libevent而言，设计更简练，性能更好，但对Windows支持不够好
* Go
  * [gnet](https://github.com/panjf2000/gnet) ⭐ 11,231 | 🐛 1 | 🌐 Go | 📅 2026-07-09 - 高性能、轻量级、非阻塞的事件驱动 Go 网络框架
  * [netpoll](https://github.com/cloudwego/netpoll) ⭐ 4,601 | 🐛 5 | 🌐 Go | 📅 2026-08-06 - 字节跳动开源的高性能 Go 网络库
* Python
  * [Twisted](http://twistedmatrix.com/) - Twisted是用Python实现的基于事件驱动的网络引擎框架
  * [Gevent](http://www.gevent.org/) - Gevent是一种基于协程的Python网络库，它用到Greenlet提供的，封装了libevent事件循环的高层同步API
* Erlang
  * [ranch](https://github.com/ninenines/ranch) ⭐ 1,242 | 🐛 5 | 🌐 Erlang | 📅 2026-07-28 - cowboy 项目下的Tcp网络库
* C#
  * [DotNetty](https://github.com/Azure/DotNetty) ⭐ 4,250 | 🐛 174 | 🌐 C# | 📅 2026-01-12 - netty 的C#版
* Rust
  * [tokio](https://github.com/tokio-rs/tokio) ⭐ 32,943 | 🐛 420 | 🌐 Rust | 📅 2026-08-17 - Rust 异步运行时与网络库事实标准
  * [mio](https://github.com/tokio-rs/mio) ⭐ 7,079 | 🐛 28 | 🌐 Rust | 📅 2026-08-17 - Rust 底层非阻塞 IO 库

### 协议

*协议*

* [protobuf](https://github.com/google/protobuf) ⭐ 71,732 | 🐛 292 | 🌐 C++ | 📅 2026-08-17 - 大家都知道的protobuf
* [FlatBuffers](https://github.com/google/flatbuffers) ⭐ 26,332 | 🐛 264 | 🌐 C++ | 📅 2026-08-11 - Google出品，专门为游戏开发或其他性能敏感的应用程序需求而创建
* [Cap'n Proto](https://github.com/capnproto/capnproto) ⭐ 13,160 | 🐛 330 | 🌐 C++ | 📅 2026-08-17 - 极致性能的序列化协议，零拷贝
* [Thrift](https://github.com/apache/thrift) ⭐ 10,955 | 🐛 13 | 🌐 C++ | 📅 2026-08-17 - Apache 跨语言 RPC 与序列化框架
* [SBE](https://github.com/real-logic/simple-binary-encoding) ⭐ 3,487 | 🐛 43 | 🌐 Java | 📅 2026-08-17 - 面向超低延迟场景的二进制编码
* [Json](http://www.json.org/) - 这个算凑数吗？
* [MessagePack](https://msgpack.org/) - It's like JSON. but fast and small.
* [CBOR](https://cbor.io/) - 二进制对象表示，IETF RFC 8949

### 持久化

*持久化框架*

* Java
  * [druid](https://github.com/alibaba/druid) ⭐ 28,176 | 🐛 2,323 | 🌐 Java | 📅 2026-08-01 - 阿里巴巴出品 数据库连接池
  * [HikariCP](https://github.com/brettwooldridge/HikariCP) ⭐ 21,183 | 🐛 543 | 🌐 Java | 📅 2026-06-14 - 高性能 JDBC 连接池
  * [MyBatis](https://github.com/mybatis/mybatis-3) ⭐ 20,435 | 🐛 206 | 🌐 Java | 📅 2026-08-17 - 一个支持普通SQL查询,存储过程和高级映射的优秀持久层框架
  * [Hibernate](https://github.com/hibernate/hibernate-orm) ⭐ 6,458 | 🐛 166 | 🌐 Java | 📅 2026-08-17 - 老牌 Java ORM 框架
* C#
  * [Dapper](https://github.com/StackExchange/Dapper) ⭐ 18,367 | 🐛 548 | 🌐 C# | 📅 2026-05-16 - 是一款轻量级ORM框架
  * [Entity Framework Core](https://github.com/dotnet/efcore) ⭐ 14,770 | 🐛 2,371 | 🌐 C# | 📅 2026-08-17 - 微软官方 .NET ORM
* Erlang
  * [mysql-otp](https://github.com/mysql-otp/mysql-otp) ⭐ 375 | 🐛 9 | 🌐 Erlang | 📅 2025-06-10 -  MySQL driver for Erlang/OTP
* Golang
  * [gorm](https://github.com/go-gorm/gorm) ⭐ 39,908 | 🐛 518 | 🌐 Go | 📅 2026-06-25 - Go 最流行的 ORM
  * [sqlx](https://github.com/jmoiron/sqlx) ⭐ 17,728 | 🐛 393 | 🌐 Go | 📅 2024-08-15 - database/sql 的扩展
  * [go-sql-driver](https://github.com/go-sql-driver/mysql) ⭐ 15,268 | 🐛 72 | 🌐 Go | 📅 2026-08-14 -  MySQL driver for Golang
  * [xorm](https://gitea.com/xorm/xorm) - 简单强大的 Go ORM
* Python
  * [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy) ⭐ 12,091 | 🐛 213 | 🌐 Python | 📅 2026-08-17 - Python SQL 工具包与 ORM

### 缓存与消息队列

*游戏服常用的缓存与消息中间件*

* [Redis](https://github.com/redis/redis) ⭐ 76,022 | 🐛 2,908 | 🌐 C | 📅 2026-08-17 - 高性能内存数据库，游戏服务器最常用的缓存
* [NSQ](https://github.com/nsqio/nsq) ⭐ 25,768 | 🐛 77 | 🌐 Go | 📅 2026-08-11 - 实时分布式消息平台
* [Redisson](https://github.com/redisson/redisson) ⭐ 24,372 | 🐛 251 | 🌐 Java | 📅 2026-08-17 - Redis 的 Java 客户端，提供分布式对象与服务
* [go-redis](https://github.com/redis/go-redis) ⭐ 22,215 | 🐛 65 | 🌐 Go | 📅 2026-08-17 - Redis 的 Go 客户端
* [NATS](https://github.com/nats-io/nats-server) ⭐ 20,532 | 🐛 544 | 🌐 Go | 📅 2026-08-17 - 高性能云原生消息系统
* [RabbitMQ](https://github.com/rabbitmq/rabbitmq-server) ⭐ 13,782 | 🐛 263 | 🌐 JavaScript | 📅 2026-08-17 - 通用消息中间件
* [KeyDB](https://github.com/Snapchat/KeyDB) ⭐ 12,510 | 🐛 271 | 🌐 C++ | 📅 2024-05-29 - Redis 的多线程分支

### Log

*Log*

* Java
  * [Logback](https://github.com/qos-ch/logback) ⭐ 3,234 | 🐛 334 | 🌐 Java | 📅 2026-08-14 - log4j 作者写的下一代日志框架
  * [Log4j](https://github.com/apache/log4j) ⚠️ Archived - Apache log4j
* C#
  * [Serilog](https://github.com/serilog/serilog) ⭐ 8,028 | 🐛 17 | 🌐 C# | 📅 2026-07-31 - 结构化日志的 .NET 库
  * [NLog](https://github.com/NLog/NLog) ⭐ 6,546 | 🐛 50 | 🌐 C# | 📅 2026-08-16 - 支持多平台的C# log库
* C++
  * [spdlog](https://github.com/gabime/spdlog) ⭐ 29,487 | 🐛 49 | 🌐 C++ | 📅 2026-08-08 - 极快的 C++ 日志库
  * [glog](https://github.com/google/glog) ⚠️ Archived - Google C++ 日志库
* Erlang
  * [Lager](https://github.com/erlang-lager/lager) ⭐ 1,130 | 🐛 52 | 🌐 Erlang | 📅 2025-08-26 - A logging framework for Erlang/OTP
* Golang
  * [logrus](https://github.com/sirupsen/logrus) ⭐ 25,751 | 🐛 44 | 🌐 Go | 📅 2026-08-17 - Structured, pluggable logging for Go
  * [zap](https://github.com/uber-go/zap) ⭐ 24,631 | 🐛 188 | 🌐 Go | 📅 2026-08-05 - Blazing fast, structured, leveled logging in Go
  * [zerolog](https://github.com/rs/zerolog) ⭐ 12,488 | 🐛 145 | 🌐 Go | 📅 2026-08-10 - 零分配 JSON logger
* Python
  * [loguru](https://github.com/Delgan/loguru) ⭐ 24,068 | 🐛 267 | 🌐 Python | 📅 2026-07-01 - 简单易用的 Python 日志库

### 游戏AI

*游戏AI*

* [recastnavigation](https://github.com/recastnavigation/recastnavigation) ⭐ 7,863 | 🐛 133 | 🌐 C++ | 📅 2026-02-27 - 非常高效的寻路系统，和Unity的寻路算法几乎一样
* [Serpent.AI](https://github.com/SerpentAI/SerpentAI) ⚠️ Archived - 游戏代理框架，适合写外挂
* [BehaviorTree.CPP](https://github.com/BehaviorTree/BehaviorTree.CPP) ⭐ 4,161 | 🐛 56 | 🌐 C++ | 📅 2026-08-14 - 现代 C++ 行为树库，机器人/游戏均可用
* [behaviac](https://github.com/Tencent/behaviac/) ⭐ 3,045 | 🐛 100 | 🌐 C# | 📅 2023-07-07 - 腾讯开源的行为树框架
* [gdx-ai](https://github.com/libgdx/gdx-ai) ⭐ 1,301 | 🐛 33 | 🌐 Java | 📅 2024-10-01 - libgdx下的一个ai系统（非常适合参考学习）

### 工具库

*工具库*

* Java
  * [guava](https://github.com/google/guava) ⭐ 51,884 | 🐛 747 | 🌐 Java | 📅 2026-08-17 - Google出品的Java工具库
  * [Hutool](https://github.com/dromara/hutool) ⭐ 30,268 | 🐛 2 | 🌐 Java | 📅 2026-08-13 - 国产小而全的 Java 工具类库
  * [disruptor](https://github.com/LMAX-Exchange/disruptor) ⭐ 18,440 | 🐛 19 | 🌐 Java | 📅 2025-04-02 - 性能高效的线程间通讯库
* C++
  * [folly](https://github.com/facebook/folly) ⭐ 30,496 | 🐛 461 | 🌐 C++ | 📅 2026-08-17 - Facebook 开源的 C++ 基础库
  * [abseil-cpp](https://github.com/abseil/abseil-cpp) ⭐ 18,080 | 🐛 233 | 🌐 C++ | 📅 2026-08-17 - Google 通用 C++ 基础库
* Go
  * [cobra](https://github.com/spf13/cobra) ⭐ 44,455 | 🐛 432 | 🌐 Go | 📅 2026-07-11 - Go 命令行框架
  * [viper](https://github.com/spf13/viper) ⭐ 30,431 | 🐛 132 | 🌐 Go | 📅 2026-01-12 - Go 配置解决方案
  * [ants](https://github.com/panjf2000/ants) ⭐ 14,490 | 🐛 1 | 🌐 Go | 📅 2026-07-04 - 高性能 goroutine 池

### 开源服务器

*各种开源游戏服务器*

* [skynet](https://github.com/cloudwu/skynet) ⭐ 14,122 | 🐛 28 | 🌐 C | 📅 2026-08-05 - 云风大神出品Lua游戏服务器框架
* [Nakama](https://github.com/heroiclabs/nakama) ⭐ 13,176 | 🐛 125 | 🌐 Go | 📅 2026-08-07 - Heroic Labs 出品的开源分布式游戏服务器，Go 编写
* [pomelo](https://github.com/NetEase/pomelo) ⚠️ Archived - 网易出品的Node.js游戏服务器框架
* [TrinityCore](https://github.com/TrinityCore/TrinityCore) ⭐ 10,726 | 🐛 1,523 | 🌐 C++ | 📅 2026-08-17 - MMO游戏服务器框架,开源的魔兽服务器
* [Colyseus](https://github.com/colyseus/colyseus) ⭐ 7,200 | 🐛 24 | 🌐 TypeScript | 📅 2026-08-10 - Node.js / TypeScript 多人游戏服务器框架
* [kbengine](https://github.com/kbengine/kbengine) ⭐ 5,696 | 🐛 176 | 🌐 C | 📅 2022-12-13 - 一款开源的MMOG游戏服务端引擎， 仅Python脚本即可简单高效的完成任何游戏逻辑(支持热更新)
* [leaf](https://github.com/name5566/leaf) ⭐ 5,518 | 🐛 26 | 🌐 Go | 📅 2024-05-23 - 用Golang写的gameserver
* [cuberite](https://github.com/cuberite/cuberite) ⭐ 5,432 | 🐛 579 | 🌐 C++ | 📅 2026-04-25 - 我的世界 的开源服务器
* [NoahGameFrame](https://github.com/ketoo/NoahGameFrame) ⭐ 4,145 | 🐛 25 | 🌐 C++ | 📅 2023-02-25 - 一个支持分布式的C++游戏服务器框架
* [Cellnet](https://github.com/davyxu/cellnet) ⭐ 4,057 | 🐛 7 | 🌐 Go | 📅 2024-03-14 - Go 高性能事件驱动游戏服务器框架
* [nano](https://github.com/lonng/nano) ⭐ 3,223 | 🐛 33 | 🌐 Go | 📅 2026-02-26 - 轻量级、易用、高性能的 Go 游戏服务器框架
* [MaNGOS](https://github.com/mangos/MaNGOS) ⭐ 3,105 | 🐛 2 | 📅 2026-03-06 - 开源的魔兽服务器
* [Pitaya](https://github.com/topfreegames/pitaya) ⭐ 2,824 | 🐛 67 | 🌐 Go | 📅 2026-07-22 - Go 编写的可扩展游戏服务器框架，pomelo 思路延续
* [mqant](https://github.com/liangdas/mqant) ⭐ 2,518 | 🐛 21 | 🌐 Go | 📅 2024-09-09 - mqant是一款基于Golang语言的简洁,高效,高性能的分布式游戏服务器框架
* [NettyGameServer](https://github.com/jwpttcg66/NettyGameServer) ⭐ 1,671 | 🐛 3 | 🌐 Java | 📅 2026-04-14 - 使用netty4.X实现的手机游戏分布式服务器
* [Scut](https://github.com/ScutGame/Scut) ⭐ 1,338 | 🐛 17 | 🌐 C# | 📅 2016-07-02 - support C#/Python/Lua 可惜两年没有更新了
* [gonet](https://github.com/xtaci/gonet) ⚠️ Archived - Go 编写的简洁游戏服务器框架
* [moon](https://github.com/sniper00/moon) ⭐ 972 | 🐛 0 | 🌐 C++ | 📅 2026-08-15 - 基于Actor模型的轻量级游戏服务器框架(Modern C++, Lua)
* [due](https://github.com/dobyte/due) ⭐ 943 | 🐛 28 | 🌐 Go | 📅 2026-08-09 - 一款基于Go语言开发的轻量级分布式游戏服务器框架
* [xingo](https://github.com/viphxin/xingo) ⭐ 862 | 🐛 0 | 🌐 Go | 📅 2026-07-15 - 高性能golang网络库，游戏开发脚手架
* [RockGO](https://github.com/zllangct/RockGO) ⭐ 695 | 🐛 9 | 🌐 Go | 📅 2022-09-07 - 基于ECS，用Golang写的gameserver
* [ryzomcore](https://github.com/ryzom/ryzomcore) ⭐ 451 | 🐛 103 | 🌐 C++ | 📅 2026-08-15 - 分布式的游戏服务器，ryzom 的官方开源
* [Photon Quantum/Server (示例)](https://github.com/exitgames) - 业内常用的实时多人方案，部分组件开源

### 容器与编排

*游戏服上云常用的容器与调度*

* [Kubernetes](https://github.com/kubernetes/kubernetes) ⭐ 124,521 | 🐛 2,934 | 🌐 Go | 📅 2026-08-17 - 容器编排事实标准
* [Agones](https://github.com/googleforgames/agones) ⭐ 6,975 | 🐛 58 | 🌐 Go | 📅 2026-08-17 - 基于 Kubernetes 的专用游戏服编排平台
* [Docker](https://github.com/docker/docker-ce) ⚠️ Archived - 容器化运行时
* [Open Match](https://github.com/googleforgames/open-match) ⭐ 3,423 | 🐛 80 | 🌐 Go | 📅 2026-07-12 - Google 与 Unity 联合开源的可扩展匹配框架

### 运维

*运维工具*

* [Elasticsearch](https://github.com/elastic/elasticsearch) ⭐ 77,805 | 🐛 6,018 | 🌐 Java | 📅 2026-08-17 - 日志检索与分析
* [Grafana](https://github.com/grafana/grafana) ⭐ 76,252 | 🐛 3,359 | 🌐 TypeScript | 📅 2026-08-17 - 通用可视化与监控仪表盘
* [Ansible](https://github.com/ansible/ansible) ⭐ 70,335 | 🐛 830 | 🌐 Python | 📅 2026-08-11 - 无代理的自动化运维工具
* [Prometheus](https://github.com/prometheus/prometheus) ⭐ 65,699 | 🐛 887 | 🌐 Go | 📅 2026-08-17 - 云原生监控与告警系统
* [fabric](https://github.com/fabric/fabric) ⭐ 15,485 | 🐛 507 | 🌐 Python | 📅 2026-04-10 - 远程执行命令
* [supervisor](https://github.com/Supervisor/supervisor) ⭐ 9,103 | 🐛 181 | 🌐 Python | 📅 2025-12-21 - 进程守护管理工具
* [LinuxGSM](https://github.com/GameServerManagers/LinuxGSM) ⭐ 4,888 | 🐛 397 | 🌐 Shell | 📅 2026-08-07 - Linux Game Server Managers

### 学习资源

*学习资源*

* [awesome-cpp](https://github.com/fffaraz/awesome-cpp) ⭐ 72,802 | 🐛 313 | 📅 2026-08-04 - C++ 资源合集，含游戏方向
* [architect-awesome](https://github.com/xingshaocheng/architect-awesome) ⭐ 60,838 | 🐛 63 | 📅 2024-04-11 后端架构师技术图谱
* [game-programmer](https://github.com/miloyip/game-programmer) ⭐ 18,692 | 🐛 31 | 🌐 Python | 📅 2024-03-28 A Study Path for Game Programmer
* [Awesome GameDev](https://github.com/Calinou/awesome-gamedev) ⭐ 3,102 | 🐛 13 | 📅 2026-07-07 - 综合 gamedev 资源合集
* [Game Programming Patterns](http://gameprogrammingpatterns.com/) 游戏编程模式
* [entity-systems](http://entity-systems.wikidot.com/) 实体系统
* [data-oriented-design](http://www.dataorienteddesign.com/dodmain/) 面向数据的设计
* [Client-Server Game Architecture](https://www.gabrielgambetta.com/client-server-game-architecture.html) - 客户端-服务器架构经典系列文章

### 其他

* [awesome-go](https://github.com/avelino/awesome-go) ⭐ 181,322 | 🐛 212 | 🌐 Go | 📅 2026-08-16 - Go 资源合集，找网络/服务器组件常用
* [games](https://github.com/leereilly/games) ⚠️ Archived github上的一个游戏列表
* [awesome-erlang](https://github.com/drobakowski/awesome-erlang) ⭐ 1,708 | 🐛 23 | 📅 2022-11-17 - Erlang 资源合集

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-17._
