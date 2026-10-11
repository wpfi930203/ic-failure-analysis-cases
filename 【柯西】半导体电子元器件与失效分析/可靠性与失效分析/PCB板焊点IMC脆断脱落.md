---
schema: failure_case_kg
schema_version: "1.1"
case_id: FC-PCB-SOLDER-IMC-DELAMINATION-001
source_title: PCB板焊点脱落分析（华南检测 ENIG）
source_publish_date: 2025-03-21
extract_date: 2026-10-11
keywords: [焊点脱落, ENIG, IMC, 脆断, PCB侧, 断口SEM]
---

# 失效案例知识图谱：PCB板焊点IMC脆断脱落

## 1. 元信息
| 字段 | 值 |
|---|---|
| 失效对象 | PCB板（ENIG表面处理）右侧焊点 |
| 断裂位置 | PCB侧IMC层（非界面，非黑镍） |
| 根因 | PCB侧IMC层偏厚 → 脆性层 → 外力脆断 |
| 排除 | 焊盘污染、黑镍腐蚀 |

## 2. 证据链
| ID | 手段 | 结果 |
|---|---|---|
| E2 | PCB侧面SEM+EDS | 无腐蚀裂纹→排除污染 |
| E3 | PCB侧切片+SEM | 断裂在PCB侧IMC；无黑镍 |
| E4 | 元件侧切片+SEM | 组件IMC 1.83-2.40μm，PCB侧3.18-3.95μm |
| E5 | 汇总 | 元件上PCB侧3.49-3.92μm；PCB上残余1.32-1.41μm |
| E6 | 结论 | 断裂在PCB侧IMC；偏厚IMC为脆层 |

## 3. 关系
| # | 头 | 关系 | 尾 |
|---|---|---|---|
| R1 | PCB侧IMC过厚 | 成为 | 脆性层 |
| R2 | 脆性层 | 受外力 | 脆断 |
| R3 | PCB侧断裂 | 验证 | IMC过厚主因 |

## 4. 改进
- 适当降低焊接热量避免较厚IMC层

## 5. 知识要点
- IMC厚度半定量判据：PCB侧3.18-3.95μm > 组件1.83-2.40μm，偏厚侧为断裂方向。