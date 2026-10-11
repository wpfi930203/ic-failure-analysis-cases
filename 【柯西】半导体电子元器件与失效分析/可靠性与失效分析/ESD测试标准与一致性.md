---
id: KG-ESD-TEST-RELIABILITY-001
source_title: AEC-Q系列ESD测试 + 两次ESD结果差异（iST）
extract_date: 2026-10-11
keywords: [ESD, HBM, MM, CDM, JS-001, JS-002, AEC-Q100, ISO10605, Latch-Up, 校准]
---

# 可靠性知识图谱：ESD原理/标准/测试一致性

## 1. ESD基础
- ESD=静电荷积累后瞬间放电；约40%集成电路失效由ESD引起

## 2. 三模型
| 模型 | 参数 |
|---|---|
| HBM | 1.5kΩ+100pF |
| MM | 0Ω+200pF |
| CDM | 自身充电 |

## 3. AEC-Q依据
- Q100系用JS-001(HBM)/JS-002(CDM)
- Q200用ISO10605(2000Ω/150pF)

## 4. 测试一致性
- 供电差0.01V→Latch-Up结果相反
- 设备无输出→误通过
- 校准频率低→失真

## 5. 措施
- 月度校准、波形日志、FA复核

## 6. 知识要点
- 两差异多在测试仪/校准而非样品，用波形日志+FA复核。