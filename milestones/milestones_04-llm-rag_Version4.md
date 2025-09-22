# 04 LLM/RAG（大模型应用）

目标
- 构建一个小型 RAG 系统，完成评测与安全加固，并提供统一服务入口。

交付物
- RAG 服务（索引构建、检索、重排序、答案生成）
- 向量库与评测数据集，离线/在线评测报告（准确性/覆盖率/成本/延迟）
- 安全与防护策略（越狱/幻觉/隐私）

验收标准
- [ ] 支持多数据源索引；可配置 embedding/检索参数
- [ ] 评测：基准集构造、自动/半自动打分（如 Ragas/DeepEval）
- [ ] 成本与延迟优化：缓存、分段、并行与截断策略
- [ ] 安全评测：越狱/敏感信息检测与拒答策略
- [ ] 统一网关：与 Java Spring/NestJS 网关集成（鉴权/配额/审计）

任务清单
- [ ] 选型：OpenAI/Claude/本地模型 + Faiss/PGVector/Weaviate
- [ ] 索引：分块、embedding、元数据；召回+精排
- [ ] 评测：针对任务构造 Ground Truth 或使用 LLM-as-a-judge（谨慎）
- [ ] 日志与回放：收集真实查询做迭代
- [ ] 安全：提示词注入/越狱对抗、输出过滤

参考资料
- [LlamaIndex](https://www.llamaindex.ai/) / [LangChain](https://www.langchain.com/)
- [RAGAS](https://github.com/explodinggradients/ragas) / [DeepEval](https://github.com/confident-ai/deepeval)