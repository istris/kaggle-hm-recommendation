# Kaggle H&M Personalized Fashion Recommendations

Kaggle竞赛项目：H&M时尚商品个性化推荐

## 项目结构
    ├── data/               # 数据文件（gitignore）
    ├── notebooks/          # Jupyter Notebook
    ├── src/               # 源代码
    │   ├── preprocessing.py  # 数据预处理
    │   ├── models.py        # 模型定义
    │   └── evaluation.py    # 评估指标
    ├── outputs/           # 模型输出（gitignore）
    └── docs/              # 文档


## 数据理解
见 [docs/data_dictionary.md](docs/data_dictionary.md)

## 运行环境
- Python 3.9+
- PyTorch 1.12+
- pandas, numpy, scikit-learn

## 进度记录
- [x] Day 1: 环境准备 + 数据下载 + 数据理解
- [ ] Day 2-7: EDA + Baseline + SVD++
- [ ] Day 8-14: Two-Tower + 优化 + 提交

## 竞赛链接
https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations
EOF

# 提交到GitHub
git add .
git commit -m "Day 1: init project structure and data dictionary"