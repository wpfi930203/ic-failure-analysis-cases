---
schema: failure_case_kg
schema_version: "1.1"
case_id: FC-PCBA-RECTIFIER-EOS-MISJUDGE-001
source_title: EOS误判失效（整流桥+TVS）分析
source_publish_date: 2026-10-11
extract_date: 2026-10-11
keywords: [EOS, 过电应力, 整流桥, TVS, 误判, 二次回路]
---

# 失效案例知识图谱：EOS误判（整流桥+TVS）

## 1. 元信息
| 字段 | 值 |
|---|---|
| 失效对象 | 整流桥+TVS |
| 失效模式 | 疑似EOS烧毁 |
| 重点 | 分辨真EOS与二次损坏 |

## 2. 分析流程
- EOS判别：大电流弧孔、过热熔化、可双失效
- 微观SEM/金相 看熔融形态/ESD特征
- 二次回路排查是否反向击穿伪装

## 3. 关系
| # | 头 | 关系 | 尾 |
|---|---|---|---|
| R1 | 大电流寡热 | → | 整流桥击穿 |
| R2 | 二次故障 | 冒充 | EOS烧毁 |
| R3 | 微观形态 | 判别 | EOS真伪 |

## 4. 改进
- 加TVS钳位、保护电路、区分真EOS/外因

## 5. 知识要点
- 整流桥配TVS，次级短路反向击回伪装EOS；需微观+回路排查。