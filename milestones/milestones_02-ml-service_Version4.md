# 02 ML Service（模型服务化）

目标
- 训练并导出一个模型，构建在线推理服务，容器化并提供 API。

交付物
- 模型训练代码与模型工件（joblib/onnx 等）
- 推理服务（FastAPI/gRPC）与 Dockerfile
- 单元与集成测试、负载/延迟基线报告

验收标准
- [ ] 本地训练并导出模型；推理服务加载模型并返回预测
- [ ] 完整测试：数据校验、接口契约、回归测试
- [ ] Docker 镜像可构建/运行；README 有一键启动
- [ ] 性能基线：并发/延迟/吞吐；识别瓶颈与优化点
- [ ] API 文档（OpenAPI/GraphQL Schema）

任务清单
- [ ] FastAPI 实现 REST 推理；或 gRPC（推荐含流式/批处理）
- [ ] 模型优化（批量推理、缓存、简单量化/蒸馏可选）
- [ ] 日志与指标：请求计数、P95 延迟、错误率
- [ ] 与现有后端集成建议：Java Spring/NestJS 作为网关（鉴权/限流）

参考资料
- [FastAPI](https://fastapi.tiangolo.com/)
- [ONNX Runtime](https://onnxruntime.ai/)