# 里程碑总览与依赖关系

阶段列表
1. Foundations（基础）
2. ML Service（模型服务化）
3. MLOps Basics（流水线与治理）
4. LLM/RAG（大模型应用）
5. Production Scale（生产级可扩展与可靠性）
6. Portfolio & Interview（作品集与面试准备）

依赖关系（建议）
- 01 → 02 → 03 是主线
- 04 可与 03 并行，但依赖 02 的服务化基础
- 05 依赖 02/03（也可对 04 的系统做升级）
- 06 贯穿所有阶段的沉淀与总结

进度追踪（示例）
- [ ] 01 Foundations
- [ ] 02 ML Service
- [ ] 03 MLOps Basics
- [ ] 04 LLM/RAG
- [ ] 05 Production Scale
- [ ] 06 Portfolio & Interview

可复用成果建议
- 通用特征工程与评测脚本
- 模型服务模板（FastAPI/gRPC + Docker）
- CI/CD 模板（GitHub Actions）
- 监控/漂移报告模板（Prometheus/Evidently）
- LLM/RAG 评测集与指标基线