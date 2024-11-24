# 西游记佛道倾向研究 - Word2Vec词向量方法

## 研究问题

本研究旨在探索《西游记》中角色与佛教和道教之间的倾向关系。通过使用Word2Vec词向量方法，我们试图量化并比较唐僧、孙悟空、猪八戒和沙和尚这四个主要角色与佛教和道教词汇的接近程度，以揭示他们在宗教文化背景下的定位。

## 主要步骤

1. **数据准备**：
   - 收集《西游记》文本数据，并构建佛教和道教的专业词汇表。

2. **文本清洗**：
   - 使用正则表达式将角色别名统一替换为标准名称，以减少数据的歧义性。
   - 清洗文本，去除不必要的空格和特殊字符，保留关键词汇。

3. **分词与句子构建**：
   - 使用jieba进行中文分词，并将分词结果作为Word2Vec模型的输入。
   - 特别地，以佛教和道教词汇为边界构建句子，以强调这些词汇在模型训练中的重要性。

4. **Word2Vec模型训练**：
   - 使用Gensim库中的Word2Vec模型对清洗后的句子进行训练，生成词向量。

5. **词向量计算与分析**：
   - 计算每个角色与佛教和道教词汇的加权平均距离，以评估角色与两大宗教的接近程度。

6. **结果输出**：
   - 输出每个角色与佛教和道教的加权平均距离，提供直观的比较结果。

## 最终结论

通过Word2Vec词向量方法，我们得出以下结论：

- 角色与佛教和道教的加权平均距离可以作为衡量其宗教倾向的一个指标。
- 唐僧、孙悟空、猪八戒和沙和尚这四个角色在佛教和道教之间的倾向存在差异，这与他们在《西游记》中的性格和行为表现相吻合。
- 该方法为数字文学研究提供了一种新的视角，可以应用于其他文学作品中角色与文化背景关系的分析。

## 使用说明

本项目包含一个Jupyter Notebook文件（`西游记佛道embedding.ipynb`），其中详细记录了数据处理、模型训练和结果分析的全过程。要运行此项目，请确保你的环境中安装有以下包：

- Python 3.9.19
- Jupyter Notebook
- Gensim
- Numpy
- Scikit-learn
- Matplotlib
- Jieba

你可以通过运行Jupyter Notebook来复现我们的分析过程，并根据需要调整参数或扩展研究。

## 贡献与反馈

本项目由人大数字人文研究公众号的技术&应用栏目提供。我们欢迎任何形式的贡献和反馈，包括但不限于代码优化、新功能添加和研究方法改进。如果你有任何建议或问题，请通过GitHub Issues与我们联系。

## 版权声明

《西游记》作为公共领域作品，其文本可用于学术研究和教育目的。本项目中的代码和分析结果遵循MIT License，详情请参阅项目中的LICENSE文件。
