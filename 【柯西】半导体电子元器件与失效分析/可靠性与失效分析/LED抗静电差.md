---
schema: failure_case_kg
schema_version: "1.1"
case_id: FC-LED-ESD-WEAK-001
source_title: LED抗静电差(ESD)失效分析
source_publish_date: 2026-10-11
extract_date: 2026-10-11
keywords: [LED, ESD, 抗静电, 静电敏感, PN结, 死灯]
---

# 失效案例知识图谱：LED抗静电差（ESD敏感）

## 1. 元信息
| 字段 | 值 |
|---|---|
| 失效对象 | LED芯片 |
| 失效模式 | 静电损伤→漏电/死灯 |
| 根因 | 芯片对ESD敏感 |

## 2. 机理
- 静电高压→近界面/薄氧化物击穿
- 损伤边缘漏电→光衰/死灯
- 无内置ESD保护更敏感

## 3. 检测
- ESD模型测试分级、漏电测试、电致发光定位

## 4. 改进
- 加Zener/内置ESD、产线防静电、选用抗ESD型号

## 5. 知识要点
- 抗静电差=芯片ESD敏感→击穿死灯；内置保护+防静电工艺。