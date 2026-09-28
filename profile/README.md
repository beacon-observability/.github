# Beacon Observability

Beacon 是 GuanceCloud 基于 [OpenTelemetry](https://opentelemetry.io/) 维护的多语言应用探针项目。我们按语言独立维护源码、上游同步、测试和发行，同时提供统一的产品入口与公共维护原则。

## 项目入口

| 仓库 | 用途 |
| --- | --- |
| [beacon](https://github.com/beacon-observability/beacon) | 产品介绍、语言入口、维护原则与路线图 |
| [beacon-java](https://github.com/beacon-observability/beacon-java) | Beacon Java 源码、开发文档与发行准备 |
| [beacon-python](https://github.com/beacon-observability/beacon-python) | Beacon Python 源码、开发文档与发行准备 |

## 当前状态

项目仍在持续建设中。各语言的实现方式、能力范围和发行节奏可以不同；源码存在、构建成功或上游支持，不等同于 Beacon 已正式支持。请从 [语言项目](https://github.com/beacon-observability/beacon/blob/main/docs/languages.md) 查看最新状态，并以对应语言仓库的版本文档和发行记录为准。

## 参与项目

- 产品与跨语言文档请在 [beacon](https://github.com/beacon-observability/beacon) 中维护。
- 语言实现、测试和发行问题请前往对应语言仓库。
- 通用修复优先贡献给 OpenTelemetry 上游；Beacon 仅维护经过验证的下游差异。
