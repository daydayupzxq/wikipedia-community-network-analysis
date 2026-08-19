# 维基百科社团网络分析

围绕维基百科用户—社团网络的数据处理、静态/动态聚类与频繁子图分析。

## 仓库内容

- `notebooks/`：按原文件名保存的 Notebook；为控制仓库体积，已清除嵌入式运行输出，代码和 Markdown 说明均保留。
- `results/`：原项目中可直接展示且小于 10 MB 的图表/汇总结果。
- `requirements.txt`：根据 Notebook import 语句自动整理的依赖候选列表。

## Notebook 索引

| Notebook | 代码单元 | Markdown 单元 | 清理前输出数 |
|---|---:|---:|---:|
| `data_process1.ipynb` | 67 | 15 | 49 |
| `data_process2.ipynb` | 122 | 15 | 122 |
| `Untitled1.ipynb` | 2 | 0 | 1 |
| `总体指标聚类.ipynb` | 20 | 0 | 18 |
| `用户数据整合.ipynb` | 27 | 0 | 17 |
| `聚类三.ipynb` | 27 | 1 | 19 |
| `聚类二_效果最好.ipynb` | 38 | 1 | 24 |
| `聚类二——更改（还可以）.ipynb` | 33 | 2 | 22 |
| `聚类二修改4（暂定版修改）.ipynb` | 37 | 1 | 24 |
| `聚类修改3-暂定.ipynb` | 47 | 1 | 33 |
| `聚类分析_平均值.ipynb` | 21 | 0 | 12 |
| `读取超节点图.ipynb` | 38 | 0 | 31 |
| `静态模型分析.ipynb` | 29 | 4 | 21 |
| `静态聚类.ipynb` | 31 | 3 | 20 |
| `频繁子图挖掘.ipynb` | 67 | 6 | 48 |
| `频繁子图挖掘算法示例.ipynb` | 19 | 0 | 29087 |
| `频繁子图结构统计.ipynb` | 7 | 1 | 2721 |

## 已保留结果

- `results/不同用户类型的分布图.png`
- `results/主题类别图.png`
- `results/用户参与社团的分布图.png`
- `results/用户数量演化趋势图.png`
- `results/用户类型列表数量分布.png`
- `results/示例数据时间图.png`
- `results/重复用户列表数量分布.png`

## 数据说明

原目录包含大量原始和中间 CSV/TXT 数据，部分文件超过 GitHub 100 MB 单文件限制，且行为或用户明细数据可能不适合公开发布。因此本仓库不提交这些数据。运行 Notebook 前，请将合法取得的数据放入本地数据目录，并按 Notebook 中的路径配置进行调整。

## 运行方式

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

建议按 Notebook 中的数据处理顺序运行。由于原始数据未包含在仓库中，完整复现需要自行准备数据并修正本地绝对路径。

## 整理说明

- 未包含 `.ipynb_checkpoints`、IDE 配置和缓存文件。
- 未包含大体积原始/中间数据。
- Notebook 的历史输出已清空，避免仓库过大；关键外部图表保存在 `results/`。
