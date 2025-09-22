# 03 MLOps Basics（流水线与治理）

目标
- 建立可复现、可审计的训练与部署过程；增加监控与漂移检测。

交付物
- 训练与评估流水线（Airflow/Prefect）
- 模型追踪与注册（MLflow/W&B）
- 监控仪表（Prometheus/Grafana）与漂移报告（Evidently）

验收标准
- [ ] 数据→训练→评估→注册→部署的流水线打通
- [ ] 关键元数据可追踪：数据版本、代码版本、参数、模型版本
- [ ] 线上指标可见：QPS、延迟、错误率、资源使用
- [ ] 漂移检测：数据分布/概念漂移报告与告警策略
- [ ] CI/CD：构建镜像→运行测试→部署到测试环境

任务清单
- [ ] Airflow/Prefect DAG：定期训练与离线评估
- [ ] MLflow：实验/模型注册、版本回滚
- [ ] Prometheus/Grafana：自定义指标与告警
- [ ] Evidently：数据/模型漂移报告；定义阈值与处理流程
- [ ] GitHub Actions：流水线自动化

参考资料
- [MLflow](https://mlflow.org/)
- [Evidently AI](https://www.evidentlyai.com/)
- [Prefect](https://www.prefect.io/) / [Apache Airflow](https://airflow.apache.org/)