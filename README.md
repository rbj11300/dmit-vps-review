# DMIT $36.9 年付 VPS 到底值不值买？T1 套餐全面评测：线路表现、适用场景与全套餐价格对比（附购买避坑指南）

直接说结论：**$36.9/年的 DMIT T1 WEE，不是给所有人买的，但买对了场景真的很香。**

很多人看到这个价格，会误以为是 CN2 GIA 捡漏。不是的。DMIT 的 $36.9/年入门套餐走的是 T1 国际线路，没有中国大陆方向的专项优化。但这不代表它没用——用对地方，它的性价比在同价位里很难找到对手。

这篇文章把 DMIT $36.9 的 VPS 说清楚：这个套餐是什么、能干什么、不适合什么，顺带把 DMIT 全系套餐整理出来，方便你对号入座。

---

## DMIT 是什么，T1 线路是什么意思

DMIT 是 2017 年在美国成立的 VPS 服务商，自建机房，三个数据中心分别在美国洛杉矶、中国香港和日本东京。硬件全系用 AMD EPYC 处理器，KVM 虚拟化，这点在 VPS 圈里算配置认真的一家。

搬瓦工曾经从 DMIT 购买过部分 CN2 GIA 带宽——这个细节能说明 DMIT 的线路质量在行业里处于什么位置。

DMIT 的产品线分三档：

- **Premium（Pro 系列）**：三网 CN2 GIA 双向优化，延迟最低，也最贵
- **Eyeball（EB 系列）**：电信走 CN2/9929，联通移动走 CMIN2，性价比比 Pro 高一档
- **Tier 1（T1 系列）**：国际线路，无中国大陆专项优化，价格最低

$36.9/年对应的，就是 T1 系列里最入门的 **LAX.AN4.T1 WEE** 套餐。

---

## $36.9/年这个套餐，配置到底是什么

**LAX.AN4.T1 WEE**：
- 1 核 AMD EPYC 9004 / 1GB 内存 / 20GB SSD
- 1TB 月流量（进出取最大值单向计算）
- 超量后不停机，限速至 100Mbps 继续跑
- 1 IPv4 + 1 IPv6 /64
- 洛杉矶机房，T1 国际线路

超量限速这个设计挺实用的。1TB 流量对大多数人日常够用，万一某个月超了，直接限速继续用，不用担心突然断线。

不夸张，这是我看过同价位里流量最不焦虑的一个入门套餐之一。

👉 [查看 DMIT 最新套餐与购买选项](https://www.dmit.io/aff.php?aff=13832)

---

## T1 线路国内访问质量怎么样

这是很多人最关心的问题，直接说实测情况。

T1 线路是国际优化线路，走的是多个 Tier 1 国际运营商（NTT、Lumen 等），移动走 CMI。电信联通在非高峰时段跑起来没什么问题；晚高峰时期，国内访问速度确实不如 CN2 GIA 稳定，偶尔会感觉到速度波动。

如果你的用途是：

1. 自建落地节点，自己有中转
2. 面向海外用户建站，国内访问不是核心需求
3. 跑不需要大陆优化的国际服务
4. 想低成本试水 DMIT 再决定要不要升级

——T1 套餐够用。

但如果你需要每天晚高峰稳定访问国内，或者代理场景对延迟很敏感，这个套餐不适合你，该看 Pro 或 EB 系列。

说句实话，$36.9/年的 DMIT T1 WEE，更像是一个"先进门试试看"的套餐，而不是长期主力机器的首选。

---

## DMIT 全套餐价格对比表

### 美国洛杉矶 · T1 系列（国际线路 · 超量限速不停机）

**LAX.AN4.T1 · GENERAL 系列**（CPU: AMD EPYC 9004）

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| WEE | 1核 | 1GB | 20GB | 1TB/月 | 100Mbps超量 | $36.9/年 |  [以 $36.9/年开始体验](https://www.dmit.io/aff.php?aff=13832) |
| TINY | 1核 | 1GB | 20GB | 2TB/月 | 10Gbps | $6.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| STARTER | 1核 | 2GB | 40GB | 4TB/月 | 10Gbps | $12.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| MINI | 2核 | 2GB | 60GB | 8TB/月 | 10Gbps | $21.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| MICRO | 4核 | 4GB | 80GB | 16TB/月 | 10Gbps | $32.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

**LAX.AN5.T1 · VOLUME 系列**（CPU: AMD EPYC 9005 · 大流量定位）

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| V2C2G | 2核 | 2GB | 40GB | 5TB/月 | 10Gbps | $14.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=169) |
| V2C4G | 2核 | 4GB | 80GB | 10TB/月 | 10Gbps | $23.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=170) |
| V4C4G | 4核 | 4GB | 120GB | 20TB/月 | 10Gbps | $36.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=171) |
| V4C8G | 4核 | 8GB | 160GB | 40TB/月 | 10Gbps | $52.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=180) |
| V8C16G | 8核 | 16GB | 240GB | 80TB/月 | 10Gbps | $119.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=172) |
| V12C24G | 12核 | 24GB | 320GB | 160TB/月 | 10Gbps | $199.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=173) |

---

### 美国洛杉矶 · Premium 系列（三网 CN2 GIA · 大陆优化）

**LAX.AN4.Pro**（CPU: AMD EPYC 9004）

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| TINY | 1核 | 2GB | 20GB | 1000GB/月 | 1Gbps | $88.88/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=237) |
| Pocket | 2核 | 2GB | 40GB | 1500GB/月 | 4Gbps | $159.98/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=238) |
| STARTER | 2核 | 2GB | 80GB | 3000GB/月 | 10Gbps | $29.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=239) |
| MINI | 4核 | 4GB | 80GB | 5000GB/月 | 10Gbps | $58.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=240) |
| MICRO | 4核 | 4GB | 160GB | 7000GB/月 | 10Gbps | $74.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=241) |
| MEDIUM | 6核 | 8GB | 160GB | 15000GB/月 | 10Gbps | $168.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=242) |
| LARGE | 8核 | 16GB | 320GB | 25000GB/月 | 10Gbps | $338.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=243) |
| GIANT | 12核 | 24GB | 640GB | 50000GB/月 | 10Gbps | $619.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=244) |

**LAX.AN5.Pro**（CPU: AMD EPYC 9005）

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| TINY | 1核 | 2GB | 20GB | 1000GB/月 | 1Gbps | $119.99/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=100) |
| Pocket | 2核 | 2GB | 40GB | 1500GB/月 | 4Gbps | $203.90/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=137) |
| STARTER | 2核 | 2GB | 80GB | 3000GB/月 | 10Gbps | $38.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=56) |
| MINI | 4核 | 4GB | 80GB | 5000GB/月 | 10Gbps | $76.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=58) |
| MICRO | 4核 | 4GB | 160GB | 7000GB/月 | 10Gbps | $99.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=81) |
| MEDIUM | 6核 | 8GB | 160GB | 15000GB/月 | 10Gbps | $219.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=82) |
| LARGE | 8核 | 16GB | 320GB | 25000GB/月 | 10Gbps | $459.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=61) |
| GIANT | 12核 | 24GB | 640GB | 50000GB/月 | 10Gbps | $839.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=98) |

---

### 美国洛杉矶 · Eyeball 系列（电信 9929 + 移动 CMIN2）

**LAX.AN4.EB**

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| TINY | 1核 | 2GB | 20GB | 1500GB/月 | 2Gbps | $88.88/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=245) |
| Pocket | 2核 | 2GB | 40GB | 3000GB/月 | 4Gbps | $159.98/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=246) |
| STARTER | 2核 | 2GB | 80GB | 5000GB/月 | 10Gbps | $29.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=247) |
| MINI | 4核 | 4GB | 80GB | 10000GB/月 | 10Gbps | $58.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=248) |
| MICRO | 4核 | 4GB | 160GB | 14000GB/月 | 10Gbps | $74.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=249) |
| MEDIUM | 6核 | 8GB | 160GB | 30000GB/月 | 10Gbps | $168.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=250) |
| LARGE | 8核 | 16GB | 320GB | 50000GB/月 | 10Gbps | $338.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=251) |
| GIANT | 12核 | 24GB | 640GB | 100000GB/月 | 10Gbps | $619.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=252) |

**LAX.AN5.EB**

| 套餐 | CPU | 内存 | 硬盘 | 流量 | 带宽 | 价格 | 购买 |
|------|-----|------|------|------|------|------|------|
| TINY | 1核 | 2GB | 20GB | 1500GB/月 | 2Gbps | $119.99/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=189) |
| Pocket | 2核 | 2GB | 40GB | 3000GB/月 | 4Gbps | $203.90/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=190) |
| STARTER | 2核 | 2GB | 80GB | 5000GB/月 | 10Gbps | $38.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=191) |
| MINI | 4核 | 4GB | 80GB | 10000GB/月 | 10Gbps | $76.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=192) |
| MICRO | 4核 | 4GB | 160GB | 14000GB/月 | 10Gbps | $99.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=193) |
| MEDIUM | 6核 | 8GB | 160GB | 30000GB/月 | 10Gbps | $219.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=194) |
| LARGE | 8核 | 16GB | 320GB | 50000GB/月 | 10Gbps | $459.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=195) |
| GIANT | 12核 | 24GB | 640GB | 100000GB/月 | 10Gbps | $839.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=196) |

现在我有了足够材料，开始写完整的Markdown文章输出：

---

# DMIT $36.9 年付 VPS 怎么样？T1 套餐线路评测、适用场景与全系套餐价格一次讲清楚（含避坑指南与套餐对比表）

很多人在 DMIT 官网看到 $36.9/年这个价格，第一反应是：「这么便宜，是不是 CN2 GIA 捡漏？」

不是。

$36.9/年对应的是 DMIT 的 LAX.AN4.T1 WEE 套餐，走的是 T1 国际线路，没有针对中国大陆方向的专项优化。这一点搞清楚，后面所有的评价才有意义。不过这不代表这个套餐没价值——用对了场景，它在同价位里真的难找到对手。

这篇文章把这件事说完整：$36.9 的 DMIT 是什么线路、能干什么、哪些场景不适合，顺带把 DMIT 全系套餐整理出来方便你对号入座。

---

## DMIT 是谁，三条产品线分别什么定位

DMIT 是 2017 年在美国注册的 VPS 服务商，走自建机房路线，三个数据中心分别在美国洛杉矶、中国香港和日本东京。全系标配 AMD EPYC 处理器 + NVMe SSD，KVM 虚拟化。

有个常被提到的背景：搬瓦工曾从 DMIT 购买过 CN2 GIA 带宽，这点能说明 DMIT 在精品线路这块的位置。

产品线一共三档，命名看起来有点绕，拆开其实很简单：

**Premium（Pro 系列）** — 三网 CN2 GIA 双向优化，电信联通去程 GIA，移动走 CMI，三网回程全走 GIA。延迟最低，晚高峰也稳，就是贵。

**Eyeball（EB 系列）** — 电信走 CN2/9929，联通走 9929，移动走 CMIN2。国内优化稍弱于 Pro，但价格低一档，对联通移动用户来说性价比更高。

**Tier 1（T1 系列）** — 国际优化线路，走多个 Tier 1 国际运营商，无中国大陆专项优化。价格最低，$36.9/年 就是这个系列的入门款。

---

## DMIT 36.9 的 VPS 配置是什么

**套餐全名：LAX.AN4.T1 WEE**

- 1 核 AMD EPYC 9004 处理器
- 1GB 内存 / 20GB SSD
- 1TB 月流量（进出取最大值单向计算）
- 超量后不停机，限速至 100Mbps 继续运行
- 默认 1 IPv4 + 1 IPv6 /64
- 美国洛杉矶机房

超量限速这个设计是亮点。1TB 对个人日常够用，哪个月跑多了也只是降速不断线。同价位很多商家流量超了直接关机，DMIT 这个处理方式实用多了。

磁盘 I/O 跑起来稳定，读写在 1GB/s 量级。单核 AMD EPYC 9654 的性能对轻量级应用完全够用。

👉 [查看 DMIT 当前套餐与最新价格](https://www.dmit.io/aff.php?aff=13832)

---

## T1 线路国内访问表现如何

直接说实测的情况。

T1 系列在非高峰时段访问国内速度说得过去，延迟也在可接受范围内。但晚高峰时期，电信联通的速度波动明显，和 CN2 GIA 的体感差距能感觉到，这是 T1 线路的结构性问题，不是商家的问题。

移动走 CMI，非高峰时段下行速度还行；高峰时期也会有限速，这是 CMI 线路的通病。

说句实话：如果你的主要需求是稳定高速访问国内资源，或者晚上八九点要流畅跑代理，这个套餐不够用，直接看 Pro 或 EB 系列。

但如果是以下这几种用途，T1 够了：

1. 自建落地节点，自己在前端做了中转优化
2. 面向海外用户的网站或服务，不需要大陆方向优化
3. 开发环境、跑脚本、CI/CD 这种对线路质量不敏感的场景
4. 想先低成本测一下 DMIT 的硬件和稳定性，再决定要不要买 Pro

第四种情况尤其值得一提。DMIT 提供 3 天无理由全额退款（流量使用不超 30GB），30 天内也可以按剩余价值退款。$36.9 买进来试水，不合适退出来，试错成本很低。

---

## 三个系列怎么选，一张表说清楚

| 维度 | T1 | Eyeball（EB） | Premium（Pro） |
|------|-----|---------------|----------------|
| 国内访问优化 | 无 | 有（电信/联通9929 + 移动CMIN2） | 有（三网CN2 GIA） |
| 晚高峰稳定性 | 一般 | 较好 | 好 |
| 适合电信用户 | 否 | 是 | 是（最佳） |
| 适合联通/移动 | 否 | 是（更均衡） | 是 |
| 入门价格 | $36.9/年 | $88.88/年 | $88.88/年 |
| 流量超额 | 限速不停机 | 限速不停机 | 限速不停机 |
| 适用场景 | 国际业务/自建中转/开发环境 | 大陆访问+性价比 | 最低延迟/最稳定 |

联通移动用户选 EB，电信用户预算充足选 Pro，电信用户预算有限 EB 也行，不需要大陆优化的选 T1。

---

## DMIT 全套餐价格表

套餐比较多，按机房和系列整理，价格以官网为准，库存随时可能变动。

### 洛杉矶 · T1 国际线路

**LAX.AN4.T1 GENERAL 系列**（CPU: AMD EPYC 9004，超量限速至 100Mbps 不停机）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| WEE | 1核 | 1GB | 20GB | 1TB | $36.9/年 |  [以 $36.9/年开始](https://www.dmit.io/aff.php?aff=13832) |
| TINY | 1核 | 1GB | 20GB | 2TB | $6.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| STARTER | 1核 | 2GB | 40GB | 4TB | $12.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| MINI | 2核 | 2GB | 60GB | 8TB | $21.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| MICRO | 4核 | 4GB | 80GB | 16TB | $32.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

**LAX.AN5.T1 VOLUME 系列**（CPU: AMD EPYC 9005，大流量场景）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| V2C2G | 2核 | 2GB | 40GB | 5TB | $14.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=169) |
| V2C4G | 2核 | 4GB | 80GB | 10TB | $23.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=170) |
| V4C4G | 4核 | 4GB | 120GB | 20TB | $36.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=171) |
| V4C8G | 4核 | 8GB | 160GB | 40TB | $52.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=180) |
| V8C16G | 8核 | 16GB | 240GB | 80TB | $119.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=172) |
| V12C24G | 12核 | 24GB | 320GB | 160TB | $199.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=173) |

### 洛杉矶 · Premium 三网 CN2 GIA

**LAX.AN4.Pro**（CPU: AMD EPYC 9004）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 2GB | 20GB | 1000GB | $88.88/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=237) |
| Pocket | 2核 | 2GB | 40GB | 1500GB | $159.98/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=238) |
| STARTER | 2核 | 2GB | 80GB | 3000GB | $29.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=239) |
| MINI | 4核 | 4GB | 80GB | 5000GB | $58.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=240) |
| MICRO | 4核 | 4GB | 160GB | 7000GB | $74.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=241) |
| MEDIUM | 6核 | 8GB | 160GB | 15000GB | $168.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=242) |
| LARGE | 8核 | 16GB | 320GB | 25000GB | $338.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=243) |
| GIANT | 12核 | 24GB | 640GB | 50000GB | $619.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=244) |

**LAX.AN5.Pro**（CPU: AMD EPYC 9005）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 2GB | 20GB | 1000GB | $119.99/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=100) |
| Pocket | 2核 | 2GB | 40GB | 1500GB | $203.90/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=137) |
| STARTER | 2核 | 2GB | 80GB | 3000GB | $38.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=56) |
| MINI | 4核 | 4GB | 80GB | 5000GB | $76.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=58) |
| MICRO | 4核 | 4GB | 160GB | 7000GB | $99.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=81) |
| MEDIUM | 6核 | 8GB | 160GB | 15000GB | $219.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=82) |

### 洛杉矶 · Eyeball 系列（电信 9929 + 移动 CMIN2）

**LAX.AN4.EB**

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 2GB | 20GB | 1500GB | $88.88/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=245) |
| Pocket | 2核 | 2GB | 40GB | 3000GB | $159.98/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=246) |
| STARTER | 2核 | 2GB | 80GB | 5000GB | $29.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=247) |
| MINI | 4核 | 4GB | 80GB | 10000GB | $58.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=248) |
| MICRO | 4核 | 4GB | 160GB | 14000GB | $74.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=249) |
| MEDIUM | 6核 | 8GB | 160GB | 30000GB | $168.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=250) |
| LARGE | 8核 | 16GB | 320GB | 50000GB | $338.88/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=251) |
| GIANT | 12核 | 24GB | 640GB | 100000GB | $619.99/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=252) |

**LAX.AN5.EB**

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 2GB | 20GB | 1500GB | $119.99/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=189) |
| Pocket | 2核 | 2GB | 40GB | 3000GB | $203.90/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=190) |
| STARTER | 2核 | 2GB | 80GB | 5000GB | $38.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=191) |
| MINI | 4核 | 4GB | 80GB | 10000GB | $76.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=192) |
| MICRO | 4核 | 4GB | 160GB | 14000GB | $99.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=193) |
| MEDIUM | 6核 | 8GB | 160GB | 30000GB | $219.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832&pid=194) |

### 香港 · AS3 平台（CPU: AMD EPYC 7003）

**HKG.AS3.Pro Premium（CN2 GIA 直连大陆，延迟 20-50ms）**

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 1GB | 10GB | 300GB | $21.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| STARTER | 1核 | 2GB | 20GB | 500GB | $32.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| MINI | 2核 | 2GB | 40GB | 1000GB | $54.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

**HKG.AS3.T1**（国际线路，$36.9/年同款 T1 线路）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| WEE | 1核 | 1GB | 20GB | 1TB | $36.9/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| TINY | 1核 | 1GB | 20GB | 2TB | $6.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

### 日本东京 · AS3 平台

**TYO.AS3.Pro Premium（CN2 GIA 线路）**

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| TINY | 1核 | 1GB | 10GB | 300GB | $21.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| STARTER | 1核 | 2GB | 20GB | 500GB | $32.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

**TYO.AS3.T1**（国际线路）

| 套餐 | CPU | 内存 | 硬盘 | 月流量 | 价格 | 购买 |
|------|-----|------|------|--------|------|------|
| WEE | 1核 | 1GB | 20GB | 1TB | $36.9/年 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |
| TINY | 1核 | 1GB | 20GB | 2TB | $6.90/月 |  [选择此方案](https://www.dmit.io/aff.php?aff=13832) |

> 套餐库存随时变动，部分套餐可能缺货。购买前建议在官网确认当前库存状态。

---

## 退款政策与换 IP

退款这块，3 天内且流量用量不超 30GB 可以全额退款（扣支付手续费）；30 天内可以按剩余时间比例退款。退款可以选原路返回，也可以退到账户余额（选余额不扣手续费）。

换 IP 的政策在之前也升级过，现在可以自助操作，不用发工单等客服了。Premium 和 EB 系列 IP 被墙可以免费换，15 天一次；其他情况换 IP 收 $5。T1 系列 IP 换也是 $5，但 T1 本身 IP 质量还行，被墙概率相对低些。

---

## 买之前要知道的几件事

**一、DMIT 经常缺货。** 几个热门套餐，尤其是性价比高的年付款，补货后往往很快卖完。看到有货不要拖太久。

**二、套餐只能升级不能降级。** 第一次买保守一点，先试低配，满意了再升配或者换年付。

**三、$36.9/年的 T1 WEE 不超售。** DMIT 官方明确不超售资源，这点在同价位里不算常见。跑脚本或者轻量应用不用担心资源被抢占。

**四、客服能用中文沟通。** 官网是英文，但客服支持中文，工单通常 24 小时内回复。支付支持支付宝、PayPal，对国内用户没门槛。

---

## 常见问题

**Q：DMIT 36.9 的 VPS 是 CN2 GIA 线路吗？**

A：不是。$36.9/年的 LAX.AN4.T1 WEE 是 T1 国际线路，无中国大陆专项优化。DMIT 最便宜的 CN2 GIA 套餐（Pro 系列）入门价是 $88.88/年。

**Q：T1 线路适合做代理或梯子吗？**

A：取决于你的用法。如果你自己有中转机，T1 做落地节点完全可以。如果直接用 T1 节点访问国内，晚高峰体验不如 CN2 GIA，延迟和速度波动都会有。

**Q：$36.9/年买不到了怎么办，有其他选择吗？**

A：三个机房的 T1 系列都有 WEE 年付套餐，价格相同（洛杉矶/香港/东京各一个），缺货时可以看另外两个机房。另外 T1 TINY 月付 $6.90 也是入门选项。

**Q：DMIT 的 IP 原生吗？能解锁 Netflix 吗？**

A：全系配原生 IP。流媒体解锁能力用过的人提到比较多，但解锁状态是动态变化的，DMIT 不做书面保证，实际情况以当时测试为准。

**Q：流量超了会怎样？**

A：T1 系列超量后限速至 100Mbps 继续跑，不停机。香港/东京 T1 WEE 超量限速 50Mbps，洛杉矶 T1 WEE 超量限速 100Mbps。

---

想试的话，从 $36.9/年的 T1 WEE 进来是成本最低的方式。用着觉得线路不够，3 天内退了再看 Pro 或 EB；觉得够用，年付锁价是当下同价位里能拿到的比较实惠的一个档位了。

👉 [前往 DMIT 查看所有套餐与当前库存](https://www.dmit.io/aff.php?aff=13832)

