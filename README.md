# 算法工程师学习之路 / Algorithm Engineering Learning Journey

这是我从计算机教师转向算法工程师的长期学习记录。项目以“理解原理、亲手实现、形成作品”为主线，持续沉淀数学、机器学习、深度学习与工程实践。

> This repository documents my transition toward algorithm engineering through theory, implementation, and projects.

## 学习路线 / Roadmap

| 阶段 | 内容 | 当前状态 |
| --- | --- | --- |
| 1. 数学基础 | 线性代数、微积分、概率统计 | 已完成第一轮，持续复习 |
| 2. NumPy 从零实现 | 线性回归、逻辑回归、梯度下降 | 已完成 |
| 3. 机器学习基础 | 数据处理、评估、决策树与过拟合 | 学习中 |
| 4. 深度学习 | PyTorch、CNN、Transformer | 待开始 |
| 5. 项目与部署 | 完整项目、服务化、作品集 | 待开始 |

## 已完成的 Notebook / Completed Notebooks

- [R1：线性回归训练循环](notebooks/r1_线性回归训练循环.ipynb)：用 NumPy 手写梯度下降。
- [R1：逻辑回归训练循环](notebooks/r1_逻辑回归训练循环.ipynb)：从二元交叉熵推导到实现。
- [W4：数据处理与数据集划分](notebooks/w4_数据处理与数据集划分.ipynb)：训练/验证/测试划分、标准化、缺失值与类别特征。
- [W5：sklearn 逻辑回归与模型评估](notebooks/w5_sklearn逻辑回归与模型评估.ipynb)：Pipeline、混淆矩阵、ROC 与 AUC。
- [W6：决策树与过拟合](notebooks/w6_决策树与过拟合.ipynb)：待完成当前练习。

完整进度见 [学习档案](notes/算法工程师学习档案.md)。

## 运行方式 / Getting Started

```bash
pip install numpy pandas scikit-learn matplotlib jupyter
jupyter lab
```

在 Jupyter 中打开 `notebooks/` 下对应文件，按顺序运行单元格即可。

## 学习原则 / Learning Principles

- 每个概念都要能解释：**what, why, how**。
- 先理解推导，再亲手写出最小实现。
- 只在训练集上 `fit`，验证集和测试集只做 `transform`，防止 data leakage（数据泄露）。
- 每周记录进度；每个阶段产出可复现的 Notebook 或项目。

## English in Learning

学习笔记会同步积累算法工程常用英语，例如 `feature`（特征）、`gradient`（梯度）、`overfitting`（过拟合）与 `evaluation`（评估）。

