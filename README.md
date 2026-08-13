# WorldHorde

Minecraft Java Edition **1.12.2** 世界级动态尸潮与感染生态插件。

当前版本：**2.1.0**

## 仓库说明

本仓库参考 YXLand 的版本归档方式维护 WorldHorde。每个版本独立保留版本说明、测试报告、变更记录、SHA256、源码清单与可恢复源码，不用新版本覆盖旧版本。

```text
versions/
└── 2.1.0/
    ├── README.md
    ├── CHANGELOG.md
    ├── TEST_REPORT.md
    ├── SHA256SUMS.txt
    └── SOURCE_MANIFEST.txt

bootstrap/
├── README.md
└── 2.1.0/
    ├── source.part00.b64
    ├── source.part01.b64
    └── ...

assets/
└── README.md
```

由于当前 GitHub 连接器不能可靠直传大型二进制 ZIP/JAR，源码采用与 YXLand 已有 bootstrap 相同的 **Base64 分片 + XZ 压缩 TAR** 归档方式；恢复后得到完整 Java/YAML/文档等文本源码。恢复方法见 [`bootstrap/README.md`](bootstrap/README.md)。

PNG / OGG 等客户端二进制资源会在 `SOURCE_MANIFEST.txt` 中保留完整路径与大小索引；后续通过支持二进制直传的发布通道继续归档到 `assets/<版本>/`。

## 2.1.0 核心能力

- World Director 世界级动态尸潮
- 血月、感染度、动态袭击与游荡尸群
- 多类型特殊感染者、远距离追猎与末尾猎杀
- A/B/C 世界攻城、结构耐久、集中突破与自动修复
- YXClientEngine 沉浸 GUI / HUD / BGM / 粒子 / World Marker
- 智能仇恨导演：多人概率索敌、软集火限制、追击失败换目标
- 尸潮余孽 / 威胁债务：上一场未清剿会强化下一场，但有硬上限与恢复机制
- 协同攻城：同一突破口多感染者协作拆墙，2/3/4/5+ 攻击者约 1.8× / 2.5× / 3.1× / 3.5× 总效率
- Minecraft 1.12.2 / Java 8，重点兼容 CatServer 类混合服务端

## 当前版本

详细说明：[`versions/2.1.0/README.md`](versions/2.1.0/README.md)

完整变更：[`CHANGELOG.md`](CHANGELOG.md)
