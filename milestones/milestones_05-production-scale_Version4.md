# 05 Production Scale（生产级可扩展与可靠性）

目标
- 构建高可用、可扩展、可演进的推理平台与发布机制，做好成本治理与合规。

交付物
- 自动扩缩容与灰度/A-B 实验方案
- 性能工程报告（TPS/延迟/成本曲线、容量规划）
- 合规与负责 AI 清单（数据来源、隐私、偏差）

验收标准
- [ ] K8s + 推理服务（Triton/自研）可水平扩展
- [ ] 灰度发布/特性开关 + 线上 A/B 评估指标
- [ ] 成本治理：GPU/CPU 成本对比、批量/并行/量化收益
- [ ] 可靠性：SLO/SLI、降级策略、熔断与限流
- [ ] 合规：数据许可证/隐私、模型偏差评估与审计可追踪

任务清单
- [ ] Triton/ONNX/TensorRT 优化（可选）
- [ ] KEDA/HPA 自动扩缩容、节点亲和与资源配额
- [ ] 金丝雀/蓝绿发布；回滚与版本冻结
- [ ] 成本/性能监控仪表与预警
- [ ] 风险与合规清单落地（审批/审计记录）

参考资料
- [NVIDIA Triton Inference Server](https://github.com/triton-inference-server/server)
- [TensorRT](https://developer.nvidia.com/tensorrt)