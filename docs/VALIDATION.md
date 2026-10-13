# 验证记录

## 已完成

- `scripts/run_tool.py --mode status` 的全部检查项存在，命令帮助正常。
- 在独立副本中，使用 Python 3.11.17 及 `requirements-analysis-tested.txt` 的四项分析依赖成功执行多任务可视化、模块消融可视化和 `--mode all_report`。
- 报告链路中的评分、报告汇总和策略建议均正常退出；保留发布目录原有结果，没有用新生成报告覆盖历史产物。
- 保存了图表、指标 CSV、rank 与重要性日志，以及训练历史 `*_history.csv`；模型下载缓存和训练权重不提交。
- Python 语法、README 图片及本地文档链接、提交清单检查通过。

## 验证边界

没有安装完整训练环境、下载模型/数据集或重新训练。README 指标引用原材料中的验证集结果，不属于本次重跑结果。

`requirements-analysis-tested.txt` 是此次检查通过的直接分析依赖组合；`requirements.txt` 是根据训练源码整理的依赖范围，尚未完整验证，也不是原训练环境锁文件。
