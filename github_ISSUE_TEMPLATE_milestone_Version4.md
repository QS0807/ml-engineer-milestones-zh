name: Milestone
description: 跟踪一个里程碑的完成情况与证据
title: "[Milestone] <阶段>-<主题>"
labels: ["milestone"]
body:
  - type: textarea
    id: goal
    attributes:
      label: 目标
      description: 本里程碑要达成的目标
      placeholder: 例如：完成可复现的训练与评估，并上线一个基础推理服务
  - type: checkboxes
    id: acceptance
    attributes:
      label: 验收标准
      options:
        - label: 交付物齐全（代码/报告/文档）
        - label: 指标达成并有对比基线
        - label: 可复现（环境/数据/随机种子）
        - label: 有自动化测试与CI
        - label: 有部署与运行说明
  - type: textarea
    id: deliverables
    attributes:
      label: 交付物与证据链接
      description: 代码仓库、PR、Demo、报告、截图等
  - type: textarea
    id: notes
    attributes:
      label: 复盘与改进
      description: 决策、权衡、问题与后续计划