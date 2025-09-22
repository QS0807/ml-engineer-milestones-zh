# 参考架构与落地建议

传统 ML（CTR/评分/分类）
- 数据：批处理（Spark/BigQuery）+ 版本化（Lakehouse）
- 训练：MLflow 追踪 + 自动重训 DAG（Airflow/Prefect）
- 服务：FastAPI/gRPC + ONNX/Triton（可选）+ K8s
- 监控：Prometheus/Grafana（延迟/吞吐/错误率）+ Evidently（漂移）

LLM/RAG
- 索引：分块 + Embedding（OpenAI/本地）+ 向量库（Faiss/PGVector/Weaviate）
- 检索：召回 + 精排（BM25/ColBERT 可选）
- 生成：LLM（API/本地）+ 策略（缓存、函数调用、工具编排）
- 评测：离线指标 + 线上反馈闭环（日志/回放）
- 安全：越狱/敏感信息检测、内容过滤与审计

与你现有技术栈的结合（Java Spring/NestJS/GraphQL）
- 网关：统一鉴权/配额/审计；对接 ML/LLM 服务
- 协议：REST + GraphQL（Schema 统一、联邦）
- DevOps：GitHub Actions + 多模块构建与集成测试