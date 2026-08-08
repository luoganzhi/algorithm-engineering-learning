# 项目一：学生学习风险预测

## 目标

基于学生的家庭背景、学习投入、缺勤和生活习惯等可在学期早期获得的信息，预测学生最终是否存在不及格风险。

风险标签定义：最终成绩 `G3 < 10` 记为 `1`（at risk），否则记为 `0`。

## 数据

使用 UCI Machine Learning Repository 的 [Student Performance](https://archive.ics.uci.edu/dataset/320/student%2Bperformance) 数据集。本项目先使用数学课程数据 `student-mat.csv`，共 395 条学生记录。

引用：Cortez, P. (2008). Student Performance [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5TG7T.

## 重要边界：防止目标泄漏

`G1`、`G2` 分别是第一、第二阶段成绩，`G3` 是最终成绩。由于项目目标是早期风险预警，特征中必须排除 `G1`、`G2`、`G3`：

- `G3` 用来构造标签，绝不能作为特征。
- `G1`、`G2` 与最终成绩高度相关，在真正的“早期预警”时尚不可获得；保留它们会得到虚高但不实用的结果。

## 项目结构

```text
data/raw/        原始公开数据
notebooks/       探索、建模与评估过程
docs/            结论与复现说明
```

## 计划

1. 数据理解与任务定义
2. 数据清洗、特征处理与训练/验证/测试划分
3. 逻辑回归、随机森林、XGBoost 的交叉验证比较
4. 风险阈值、错误案例与可解释性分析
5. 最终测试、README 结论与复现说明
