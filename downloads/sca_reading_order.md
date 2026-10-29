# 阅读顺序与文件标注说明

更新时间：2026-10-29。

**共54篇独立文献条目：39篇近三年方向候选、8篇基础/综述/经典、7篇数据集与评估。附14篇PDF；另外40篇只有阅读卡和正式入口，尚未附全文。**

## 先理解文件名

- `2025表1区_口径待核` / `2025表2区_口径待核`：匹配用户上传的2025表，但表内没有注明大类/小类，来源也未独立核实；并非已官方认证的大类一区/二区。
- `2025表3区_口径待核`：表中为三区，暂列补充阅读；若CCF A/B等价路线成立，仍可能保留。
- `领域重要来源_等级未核`：依领域重要性纳入，不能直接当成CCF A/B或中科院一区/二区。
- `会议等级待核`：正式来源已记录，会议等级仍待核。
- `经典例外` / `基础综述例外`：基础单列，不受近三年和分区门槛限制；综述不等同于公认经典。

54张阅读卡和14个PDF均已改名。19篇对应用户表一区/二区的论文目前均未附PDF，分区标注在阅读卡文件名中。已有14个PDF来自领域重要来源或经典例外，因此没有给它们虚构分区数字。

## 首轮建议读这12篇

按下面顺序逐步读，不必一口气读完所有目录。F01综述可在遇到陌生概念时作为参考。只读摘要时，不填写未见到的实验细节；没有PDF的条目先通过DOI或学校图书馆取得全文。

| 顺序 | 编号与题名 | 为什么先读 | 全文状态 |
|---:|---|---|---|
| 1 | F02 Correlation Power Analysis with a Leakage Model | CPA：理解泄漏模型、相关性与密钥排名 | 未附PDF，需下载全文 |
| 2 | F04 Deep learning for side-channel analysis and introduction to ASCAD database | ASCAD：理解数据、标签与训练/攻击集划分 | 未附PDF，需下载全文 |
| 3 | F06 Methodology for Efficient CNN Architectures in Profiling Attacks | CNN设计：建立深度学习侧信道攻击基线 | 已附PDF |
| 4 | F08 Pay Attention to Raw Traces: A Deep Learning Architecture for End-to-End Profiling Attacks | 注意力基础：衔接老师的注意力CNN方向 | 已附PDF |
| 5 | A02 On the Instability of Softmax Attention-Based Deep Learning Models in Side-Channel Analysis | 注意力为何不稳定：先理解问题，再堆叠模块 | 未附PDF，需下载全文 |
| 6 | A01 EstraNet: An Efficient Shift-Invariant Transformer Network for Side-Channel Analysis | EstraNet：理解平移不变性与长迹计算成本 | 已附PDF |
| 7 | B01 Being Patient and Persistent: Optimizing An Early Stopping Strategy for Deep Learning in Profiled Attacks | 早停：识别训练策略对攻击结果的影响 | 未附PDF，需下载全文 |
| 8 | B02 HyperSCA: A Comprehensive Hyperparameter Optimization Framework for Deep Learning-based Side Channel Attacks | HyperSCA：学习公平调参与比较方法 | 已附PDF |
| 9 | C01 Side-Channel Attacks Based on Multi-Loss Regularized Denoising AutoEncoder | ML-DAE：进入去噪预处理方向 | 未附PDF，需下载全文 |
| 10 | C02 An Effective Tool for Traces Preprocessing in Side-Channel Analysis: Ridge Energies Extraction From Synchrosqueezing Wavelet Transform | 小波脊能量：对照老师的小波GAN论文 | 未附PDF，需下载全文 |
| 11 | D01 A Second Look at the Portability of Deep Learning Side-Channel Attacks over EM Traces | CrossEM：明确跨设备攻击的实验设定 | 未附PDF，需下载全文 |
| 12 | D02 Ablation Analysis for Multi-Device Deep Learning-Based Physical Side-Channel Analysis | 跨设备消融：分析泛化收益来自哪里 | 未附PDF，需下载全文 |

## 第一轮读完后，选一条支线

- 模型结构：A04 → A03 → A06 → A07。先看消融、训练预算和模型复杂度，再看结构细节。
- 训练策略：B04 → B06 → B07 → B08。区分损失设计、对比学习、集成和自动调参。
- 预处理：F07 → C03 → C06 → C08。C06理论较难，C08证据较少，适合后读。
- 泛化：D03 → D06 → D04 → D05。每篇先确认是否使用目标设备标签、目标迹或微调。
- 数据集与评估按需穿插：E04、E01、E07；E02与E05可以推迟。

## 暂缓作为正式汇报主文献

B05、D07、D08、D09按用户表为三区，先放补充阅读；C04、C05的会议等级仍待核。上述论文并未删除。A10、B03、E02等学习成本较高，也可后读。正式汇报前仍须确认导师采用的分区口径，以及领域重要来源是否获认可。

## 每篇只做一页笔记

记录研究问题、攻击者能力、数据划分、方法变化、关键对照和消融、GE/SR与重复次数、局限，以及与你老师论文的关系。先能讲清楚问题和证据，再深入公式。

## 下载与解压

本次阅读指南和三个PDF包均已更新。建议解压到一个新的空文件夹，避免与旧版A01.pdf等文件形成重复。四个包独立下载，解压到同一父目录即可合并。详细分区证据见2025分区表匹配结果。
