# ML 工程师里程碑（Milestones）

本仓库为“机器学习工程师（ML Engineer）”的阶段性里程碑与验收标准清单，覆盖数据-模型-服务-运维的全生命周期，并包含 LLM/RAG 专项。你可以按阶段打勾完成，或将每个里程碑转成 GitHub Issue 追踪。

适用人群
- 希望系统化进阶 ML 工程师的人（含软件工程背景转 AI）
- 需要端到端能力闭环：数据/训练/部署/监控/评测/合规

如何使用
1) 浏览 milestones/ 目录的各阶段文件，选择你当前阶段。
2) 将里程碑内容复制为 Issue（建议使用 .github/ISSUE_TEMPLATE/milestone.md 模板）。
3) 为每个子任务添加勾选与证据链接（Demo、报告、PR、截图）。
4) 完成后在 README 或 00-roadmap 中更新进度。

目录结构
- milestones/
  - 00-roadmap.md（总览与依赖关系）
  - 01-foundations.md（数学/ML 基础与数据技能）
  - 02-ml-service.md（训练一个模型并服务化/容器化）
  - 03-mlops-basics.md（流水线、注册、监控与治理）
  - 04-llm-rag.md（LLM/RAG 应用与评测）
  - 05-production-scale.md（可扩展与可用性、A/B、成本治理）
  - 06-portfolio-interview.md（作品集与面试/系统设计）
- docs/
  - resources.md（精选资料与路线）
  - sample-architectures.md（参考架构与落地建议）
- .github/ISSUE_TEMPLATE/milestone.md（里程碑 Issue 模板）

快速开始（建议顺序）
- [ ] 01 Foundations
- [ ] 02 ML Service
- [ ] 03 MLOps Basics
- [ ] 04 LLM/RAG
- [ ] 05 Production Scale
- [ ] 06 Portfolio & Interview

实践建议
- 每个阶段至少产出一个“可运行、可复现、可展示”的成果（仓库/服务/报告）。
- 将关键环节自动化（数据->训练->评估->部署->监控），打通 CI/CD。
- 对 LLM 项目，重视评测与安全；对传统 ML，重视特征一致性与漂移监控。

许可
- 自由复用/改造，建议保留出处链接以便他人发现改进版本。