# AI Infra Lab — 从后端架构到AI Infra的实践

15年后端架构经验，系统学习并实践 LLM 推理服务、推理优化、MLOps 平台。
本仓库记录学习过程中的**可复现实验、优化报告、平台demo**。

## 我的方向
AI Infra / 推理服务 / MLOps 平台架构

## 产出索引
| 阶段 | 产出 | 链接 |
|---|---|---|
| 阶段1 | 推理服务部署+压测报告 | [report](reports/stage1_serving_report.md) |
| 阶段2 | 推理优化benchmark（量化/引擎对比/投机解码/TP） | [report](reports/stage2_benchmark_report.md) |
| 阶段3 | 分布式训练实践 | [notes](reports/stage3_training_notes.md) |
| 阶段4 | MLOps平台demo+架构图 | [demo](reports/stage4_mlops_demo.md) |

## 关键结论（TL;DR）
- vLLM + AWQ 在某场景下吞吐提升 X 倍、显存降 Y%
- 引擎选型：场景Z选vLLM，场景W选TRT-LLM，理由是...
- MLOps平台架构：K8s + Argo + MLflow + Prometheus，支撑多模型灰度

## 环境
见 [docs/setup.md](docs/setup.md)，复现见 [docs/reproduce.md](docs/reproduce.md)

## 踩坑记录
见 [docs/pitfalls.md](docs/pitfalls.md)
