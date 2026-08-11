# zgocloud VPS价格：年付低至$9.9起,多机房三网优化任你选

每次想租一台 VPS，我都会陷入同一个困境：便宜的怕跑路，贵的又下不去手。尤其当需求落在"既想要 CN2 GIA 三网优化、又想要原生 IP、还想年付不超过 50 美元"这种叠加 buff 的场景时，市面上真能同时满足的商家其实不多。

前段时间重新梳理了下手头的几台机器，把 ZgoCloud（也写作 ZgoVPS）这套价格体系从头到尾翻了一遍，发现它家 2026 年这一波的套餐排布，恰好就是按"价格敏感度 + 线路需求"两条轴在切——便宜的能便宜到年付 9.9 美元，贵的也能给你上 12 核 VDS 装 Windows。下面就把这套价格表拆开聊一聊，看看到底哪一档适合你。

## 一、先说 ZgoCloud 是个什么底子

ZgoCloud 是 2021 年在美国特拉华州注册的主机商，自己持有 AS197767 网络，是 ARIN 和 RIPE 成员，跟 NTT、Orange SA、Cogent 这些 Tier 1 都有直连。机房分布在洛杉矶、香港、东京、大阪、德国法尔肯施泰因，硬件清一色 AMD EPYC 7002/7003/9004 Genoa、Ryzen 9 7950X、Intel Xeon Platinum 8452Y 这种当代主力，搭配 DDR4/DDR5 + PCIe 4.0 NVMe，洛杉矶还入驻了 Equinix 机房。

简单说就是：硬件不抠门，线路也不含糊。洛杉矶走 CN2 GIA + AS9929 + CMIN2 三网优化；日本大阪主推 IIJ 软银线路；香港是三网直连。这套配置放在 2026 年的低价 VPS 市场里，属于"性能过剩"那一档。

## 二、ZgoCloud VPS 价格全景：从 $9.9/年 到 VDS 全覆盖

### 洛杉矶 Global 国际线路——价格屠夫档

这是 ZgoCloud 全家桶里最便宜的一条线，AMD EPYC 7002 + DDR4 + 1Gbps 带宽，走国际线路（不专门做三网优化），适合做跳板、出海业务、跑一些对国内访问速度不敏感的服务。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Lite | 1 核 EPYC 7002 | 512MB DDR4 | 15GB | 1TB | 1Gbps | $9.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=91) |
| Specials-Basic | 1 核 EPYC 7002 | 768MB DDR4 | 18GB | 1.5TB | 1Gbps | $12.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=92) |
| Specials-Starter | 1 核 EPYC 7002 | 1GB DDR4 | 20GB | 2TB | 1Gbps | $15/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=93) |
| Specials-Standard | 2 核 EPYC 7002 | 2GB DDR4 | 40GB | 4TB | 1Gbps | $25/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=94) |
| Specials-Pro | 3 核 EPYC 7002 | 4GB DDR4 | 60GB | 6TB | 1Gbps | $45/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=95) |
| Starter（季付） | 1 核 EPYC 7002 | 1GB DDR4 | 20GB | 2TB | 1Gbps | $8/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=84) |
| Standard（季付） | 2 核 EPYC 7002 | 2GB DDR4 | 40GB | 4TB | 1Gbps | $12/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=85) |
| Pro（季付） | 3 核 EPYC 7002 | 4GB DDR4 | 60GB | 6TB | 1Gbps | $20/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=86) |
| Premium（季付） | 4 核 EPYC 7002 | 6GB DDR4 | 80GB | 8TB | 1Gbps | $28/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=87) |

年付 9.9 美元起步，折合月均不到 1 美元，512MB 内存 + 1TB 流量，跑个轻量代理或者小型监控脚本绰绰有余。如果嫌 512MB 太挤，多花 5 美元就能升到 1GB 内存 + 2TB 流量的 Starter 档，性价比反而更高。👉 [想直接看 Global 套餐完整列表的，可以从这里进](https://bit.ly/ZgoVps)。

### 洛杉矶 AMD EPYC 7003 优化线路——三网党首选

电信走联通 CUII/AS9929，移动走自家 CMIN2/AS58807，原生美国 IP，带宽提到 200~300Mbps。这一档是大多数国内用户真正关心的"性价比甜点位"。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Lite | 1 核 | 1GB DDR4 | 20GB | 600GB | 200Mbps | $25/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=65) |
| Specials-Starter | 1 核 | 2GB DDR4 | 30GB | 1TB | 300Mbps | $36/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=115) |
| Specials-Standard | 2 核 | 3GB DDR4 | 50GB | 2TB | 300Mbps | $66/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=67) |
| Starter（季付） | 1 核 | 2GB DDR4 | 30GB | 1TB | 300Mbps | $16/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=68) |
| Standard（季付） | 2 核 | 3GB DDR4 | 50GB | 2TB | 300Mbps | $24/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=69) |
| Pro（季付） | 3 核 | 4GB DDR4 | 80GB | 2TB | 300Mbps | $32/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=72) |
| Premium（季付） | 4 核 | 6GB DDR4 | 100GB | 2TB | 300Mbps | $40/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=73) |

Specials-Lite 这款年付 25 美元、200Mbps 带宽 + 600GB 流量，是三网优化里的入门门票；如果跑 WordPress 或者中转站，建议直接上 Specials-Starter，2GB DDR4 + 1TB 流量 + 300Mbps，年付 36 美元，月均 3 美元，比 Lite 多花 11 美元换来的体验差距相当明显。

### 洛杉矶 Intel Xeon Platinum 8452Y 优化线路——DDR5 党

跟上面那档线路完全一样，差别只在 CPU 换成 Intel Xeon Platinum 8452Y，内存升级到 DDR5，硬盘走 PCIe 4.0 NVMe。适合对单核性能敏感、跑数据库或编译型工作负载的场景。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Lite | 1 核 8452Y | 768MB DDR5 | 15GB | 600GB | 200Mbps | $30/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=39) |
| Specials-Starter | 1 核 8452Y | 1GB DDR5 | 20GB | 1TB | 300Mbps | $42/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=32) |
| Specials-Standard | 2 核 8452Y | 2GB DDR5 | 40GB | 2TB | 300Mbps | $88/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=31) |
| Starter（季付） | 1 核 8452Y | 1GB DDR5 | 20GB | 1TB | 300Mbps | $16/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=26) |
| Standard（季付） | 2 核 8452Y | 2GB DDR5 | 40GB | 2TB | 300Mbps | $24/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=27) |
| Pro（季付） | 3 核 8452Y | 4GB DDR5 | 80GB | 2TB | 300Mbps | $32/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=28) |
| Premium（季付） | 4 核 8452Y | 6GB DDR5 | 100GB | 2TB | 300Mbps | $40/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=29) |

季付档的 Starter 跟 AMD 那边同价（16 美元/季），但内存是 DDR5、CPU 是 Intel 旗舰，单核跑分更高，对 PHP、Node.js 这类单线程敏感的应用友好不少。

### 洛杉矶 AMD Ryzen 9 7950X 三网优化（CN2 GIA + 9929 + CMIN2）

这是 ZgoCloud 洛杉矶线路里最顶的一档，CPU 直接上了 Ryzen 9 7950X，主频 5.7GHz，Geekbench 6 单核能跑 3000+，比 EPYC 7003 单核性能强一截。带宽也拉到 500Mbps。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Lite | 1 核 7950X | 512MB DDR5 | 15GB | 500GB | 200Mbps | $38.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=101) |
| Specials-Starter | 1 核 7950X | 1GB DDR5 | 25GB | 1TB | 500Mbps | $58.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=60) |
| Starter（季付） | 1 核 7950X | 1GB DDR5 | 25GB | 1TB | 500Mbps | $18/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=58) |
| Standard（季付） | 2 核 7950X | 2GB DDR5 | 40GB | 2TB | 500Mbps | $28/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=59) |

Ryzen 9 这档明显是为"既要 CN2 GIA 三网直连、又想要单核炸裂"的玩家准备的，跑 WordPress、Typecho、Ghost 这种动态站点，响应速度会比 EPYC 那档快一截。👉 [对单核性能有执念的，直接看这里](https://bit.ly/ZgoVps)。

### 日本大阪 IIJ 线路——亚太低延迟党

ZgoCloud 在日本大阪走的是 IIJ 主流线路，CPU 上了 EPYC 9354P 和 Ryzen 9 7950X 两套，带宽从 400Mbps 起跳，最高 800Mbps。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| EPYC 9354P Specials-Starter | 1 核 | 1GB DDR4 | 20GB | 1TB | 400Mbps | $12/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=43) |
| EPYC 9354P Specials-Standard | 2 核 | 2GB DDR4 | 40GB | 1TB | 800Mbps | $17/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=44) |
| EPYC 9354P Specials-Pro | 3 核 | 4GB DDR4 | 80GB | 1TB | 800Mbps | $24/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=45) |
| Ryzen 9 Specials-Lite | 1 核 7950X | 512MB DDR5 | 15GB | 700GB | 400Mbps | $28/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=19) |
| Ryzen 9 Specials-Starter | 1 核 7950X | 1GB DDR5 | 20GB | 1TB | 800Mbps | $38/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=20) |
| Ryzen 9 Starter（季付） | 1 核 7950X | 1GB DDR5 | 20GB | 1TB | 800Mbps | $15/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=18) |
| Ryzen 9 Standard（季付） | 2 核 7950X | 2GB DDR5 | 40GB | 2TB | 800Mbps | $25/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=21) |

日本大阪到国内的延迟通常在 50ms 上下，配合 IIJ 软银线路，三网往返都比较稳。Ryzen 9 那档年付 38 美元、800Mbps 带宽 + 1TB 流量，是亚太节点里少见的"高带宽 + 高主频 + 低延迟"组合。

### 香港 AMD EPYC 7002 三网直连

香港机房走三网直连，CPU 是 EPYC 7002，带宽统一 100Mbps（香港带宽贵，这是行业惯例），延迟最低能到 30ms 以内。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Lite | 1 核 | 512MB | 10GB | 300GB | 100Mbps | $36.8/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=123) |
| Specials-Starter | 1 核 | 1GB | 10GB | 500GB | 100Mbps | $45/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=121) |
| Specials-Standard | 2 核 | 2GB | 20GB | 1TB | 100Mbps | $88/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=122) |
| Starter（季付） | 1 核 | 1GB | 10GB | 500GB | 100Mbps | $16/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=117) |
| Standard（季付） | 2 核 | 2GB | 20GB | 1TB | 100Mbps | $30/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=118) |
| Pro（季付） | 3 核 | 3GB | 30GB | 1.5TB | 100Mbps | $45/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=119) |

香港带宽虽然只有 100Mbps，但胜在三网直连延迟低，Specials-Lite 年付 36.8 美元这一款经常被秒空，要入手得盯紧点。

### 德国 Intel Xeon Gold 5412U 国际线路

德国机房走国际线路，1Gbps 大带宽，CPU 是 Intel Xeon Gold 5412U + DDR5，适合做欧美业务落地或者跑大流量中转。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Starter（年付） | 1 核 5412U | 1GB DDR5 | 20GB | 2TB | 1Gbps | $12.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=53) |
| Standard（年付） | 2 核 5412U | 2GB DDR5 | 40GB | 4TB | 1Gbps | $22.9/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=54) |
| Starter（季付） | 1 核 5412U | 1GB DDR5 | 20GB | 2TB | 1Gbps | $6/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=49) |
| Standard（季付） | 2 核 5412U | 2GB DDR5 | 40GB | 4TB | 1Gbps | $10/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=50) |

德国这一档价格跟洛杉矶 Global 几乎打平，但 CPU 是 Intel Xeon Gold + DDR5，单核性能比 EPYC 7002 强，DDR5 也比 DDR4 快一截，跑欧洲业务的性价比相当能打。

### 洛杉矶双 ISP / 家庭 IP VPS——原生住宅 IP 党

这一档的特色是 IP 属性：双 ISP 或者家庭/住宅 IP，适合做流媒体解锁、广告投放、账号注册这类对 IP 纯净度有要求的场景。CPU 是 EPYC 7002，带宽 100~200Mbps。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 特价 VPS-1 | 1 核 | 1GB | 10GB | 500GB | 100Mbps | $58/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=146) |
| 特价 VPS-2 | 2 核 | 2GB | 20GB | 1TB | 100Mbps | $108/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=147) |
| Starter（季付） | 1 核 | 1GB | 10GB | 500GB | 100Mbps | $20/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=148) |
| Standard（季付） | 2 核 | 2GB | 20GB | 1TB | 100Mbps | $38/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=149) |
| Pro（季付） | 3 核 | 3GB | 30GB | 1.5TB | 200Mbps | $56/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=150) |
| Premium（季付） | 4 核 | 4GB | 50GB | 2TB | 200Mbps | $72/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=151) |

双 ISP 套餐不支持优惠码，价格比普通优化线路贵一些，但 IP 属性值这个差价——纯原生住宅 IP 在解锁 Netflix、ChatGPT、TikTok 这些场景里几乎是刚需。👉 [需要纯净原生 IP 的，可以从这里直接进购买页](https://bit.ly/ZgoVps)。

### 洛杉矶 VDS——可装 Windows 的大块头

VDS 跟 VPS 的区别在于资源独占：VDS 是真独享 CPU 核心、内存、硬盘，可以跑满 CPU（但不准挖矿），还能装 Windows（自备授权）。CPU 是 AMD EPYC 7003，DDR4，带宽 1~2Gbps，流量 10~20TB/月。

| 套餐 | CPU | 内存 | NVMe | 月流量 | 带宽 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Specials-Starter | 2 核 EPYC 7003 | 4GB DDR4 | 60GB | 10TB | 1Gbps | $66/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=125) |
| Specials-Standard | 4 核 EPYC 7003 | 8GB DDR4 | 150GB | 20TB | 1Gbps | $96/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=106) |
| Specials-Pro | 8 核 EPYC 7003 | 16GB DDR4 | 250GB | 20TB | 2Gbps | $166/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=107) |
| Specials-Premium | 12 核 EPYC 7003 | 24GB DDR4 | 500GB | 20TB | 2Gbps | $258/年 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=108) |
| Starter（季付） | 2 核 EPYC 7003 | 4GB DDR4 | 60GB | 10TB | 1Gbps | $24/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=124) |
| Standard（季付） | 4 核 EPYC 7003 | 8GB DDR4 | 150GB | 20TB | 1Gbps | $32/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=103) |
| Premium（季付） | 12 核 EPYC 7003 | 24GB DDR4 | 500GB | 20TB | 2Gbps | $76/季 | [立即购买](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=105) |

VDS 这档年付 96 美元就能拿到 4 核 8GB + 150GB NVMe + 20TB 流量，跑 Windows Server 或者大型站点绰绰有余，价格比同配置的独立服务器便宜一个数量级。

## 三、ZgoCloud 最新优惠码：能省则省

ZgoCloud 当前在售的优惠码有两个，力度和适用范围各有不同：

- **`8NU44CM6LZ`**：9.5 折循环优惠，仅限年付周期，适用于常规洛杉矶 VPS（特价 Specials 套餐除外），有效期至 **2026 年 8 月 31 日**。续费同价，不会第二年涨回原价。
- **`BPZZ1GE8T7`**：8.5 折优惠码，力度更大，适用于季付产品，有效期至 **2026 年 12 月 31 日**，是目前确认可叠加使用的长期码。

使用方法很简单：下单时在结账页面的 "Use promotional code" 一栏填入，点 Submit 即可生效。注意特价 Specials 套餐本身已经是底价，不能再叠加优惠码；双 ISP / 家庭 IP 套餐也不支持优惠码。

## 四、ZgoCloud VPS 价格选购建议

聊完价格表，最后给几句实在话。

**如果你只是想要一台便宜的跳板机**：直接洛杉矶 Global 国际线路 Specials-Lite，年付 9.9 美元，512MB 内存跑代理够用，月均不到 1 美元，丢了也不心疼。👉 [点这里直接下单](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=91)。

**如果你跑 WordPress 或者中转站、对国内速度有要求**：洛杉矶 AMD EPYC 7003 优化线路的 Specials-Starter 是甜点位，年付 36 美元，2GB DDR4 + 300Mbps + 1TB 流量，三网优化到位。预算再充足一点可以上 Ryzen 9 7950X 那档，单核性能更强。👉 [EPYC 7003 优化线路购买入口](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=115)。

**如果你做亚太业务、对延迟敏感**：日本大阪 IIJ 线路是首选，Specials-Starter 季付 12 美元起步，800Mbps 带宽在大阪机房里属于相当激进的配置。👉 [大阪 IIJ 套餐入口](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=43)。

**如果你要解锁流媒体、做账号注册**：直接上洛杉矶双 ISP / 家庭 IP 套餐，原生住宅 IP 是这类场景的硬通货，年付 58 美元起步。👉 [双 ISP 套餐入口](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=146)。

**如果你要装 Windows 或者跑大型站点**：洛杉矶 VDS Specials-Standard，年付 96 美元，4 核 8GB + 150GB NVMe + 20TB 流量，性价比在 VDS 这个品类里相当突出。👉 [VDS 套餐入口](https://clients.zgovps.com/?cmd=cart&action=add&affid=609&id=106)。

下单前提醒一句：ZgoCloud 开了 MaxMind 自动风控，下单时 IP 地址、电话号码、选择的国家这三个字段必须保持一致（不要求真实，但必须对得上），不然会被判 Fraud 拒单。支付方式支持 PayPal 和信用卡（Stripe），国内用户如果用支付宝，部分套餐也支持。

整体看下来，ZgoCloud 这套价格体系的核心思路很清楚：用 Specials 特价档做引流入门，用季付常规档留住长期用户，用 VDS 和双 ISP 档做利润上限。对消费者来说，这种分层意味着你总能在自己预算区间里找到对应的那一档——不至于因为"想升级又差一口气"而纠结半天。👉 [想一次性看全部套餐的，可以从这个入口进](https://bit.ly/ZgoVps)，结账时别忘了填优惠码。
