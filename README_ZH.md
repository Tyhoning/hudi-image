<p align="center">
  <h1 align="center">Hudi数据湖架构</h1>
  <p align="center">
    <a href="README.md"><strong>English</strong></a> | <strong>简体中文</strong>
  </p>

## 目录

- [仓库简介](#项目介绍)
- [前置条件](#前置条件)
- [镜像说明](#镜像说明)
- [获取帮助](#获取帮助)
- [如何贡献](#如何贡献)

## 项目介绍
[Apache Hudi](https://github.com/apache/Hudi) 是一种数据湖管理工具。它为数据湖提供了事务支持，能够实现对数据湖中的数据进行插入、更新和删除操作，并且可以跟踪数据的变化，方便进行增量数据处理和分析。

**核心特性：**
1. 数据更新和删除：传统的数据湖通常以不可变的形式存储文件，这使得更新和删除操作变得复杂。Hudi 提供了高效的 upsert（更新或插入）和 delete 操作，从而简化了对数据的修改。
2. 实时数据处理：在需要实时处理数据流的场景中，传统数据湖往往难以满足低延迟需求。Hudi 通过支持流式数据的写入和增量拉取，使得大数据分析可以接近实时进行。
3. 增量数据查询：传统数据湖架构往往需要对整个数据集进行扫描，而 Hudi 允许用户基于增量变化数据进行查询，从而极大提升了查询效率。
4. 数据一致性：Hudi 通过提供 ACID 事务支持，确保在处理更新和删除操作时数据的一致性。这对于那些数据精度要求高的场景（例如金融交易、物联网数据）非常重要。
5. 数据版本管理：Hudi 提供了时间旅行功能，允许用户访问某个历史时间点的数据，方便数据修复、回溯和审计。

**架构设计：**

![](./images/img001.png)


本项目提供的开源镜像商品 [**Hudi数据湖架构**](https://marketplace.huaweicloud.com)，已预先安装 Hudi 软件及其相关运行环境，并提供部署模板。快来参照使用指南，轻松开启“开箱即用”的高效体验吧。

> **系统要求如下：**
> - CPU: 2GHz 或更高
> - RAM: 4GB 或更大
> - Disk: 至少 40GB

## 前置条件
[注册华为账号并开通华为云](https://support.huaweicloud.com/usermanual-account/account_id_001.html)

## 镜像说明

| 镜像规格                                                                                                   | 特性说明                                         | 备注 |
|--------------------------------------------------------------------------------------------------------|----------------------------------------------| --- |
| [Hudi1.0.0-kunpeng-v1.0](https://github.com/HuaweiCloudDeveloper/Hudi-image/tree/Hudi1.0.0-kunpeng-v1.0) | 基于 鲲鹏服务器 + Huawei Cloud EulerOS 2.0 64bit 安装部署 |  |
| [Hudi1.0.0-kunpeng-v1.0](https://github.com/HuaweiCloudDeveloper/Hudi-image/tree/Hudi1.0.0-kunpeng-v1.0)   | 基于 鲲鹏服务器 + Ubuntu24.04 64bit 安装部署         |  |

## 获取帮助
- 更多问题可通过 [issue](https://github.com/HuaweiCloudDeveloper/Hudi-image/issues) 或 华为云云商店指定商品的服务支持 与我们取得联系
- 其他开源镜像可看 [open-source-image-repos](https://github.com/HuaweiCloudDeveloper/open-source-image-repos)

## 如何贡献
- Fork 此存储库并提交合并请求
- 基于您的开源镜像信息同步更新 README.md
