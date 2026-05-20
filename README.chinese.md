# **Everyones_nanoGPT 填空笔记教程**

🌐 选择语言 / [日本語 🇯🇵 ](https://github.com/HayatoHongo/Everyones_nanoGPT_ja.git) | [中文 🇨🇳](README.chinese.md)<br>

> 这是为热爱 ChatGPT 并想自己动手搭建专属模型的人准备的完整指南。<br>
> 你输入 “Hello,”，它回复 “今天我能为你做些什么？”<br>
> 当你意识到这一切不过是简单的数学运算时，心跳加速，夜不能寐。<br>
> 欢迎来到深度学习，从此无回头路。<br>
> 我在南北线拥挤的列车上，挤在狭小座位中，写下了这份指南。<br>
> 每当我读到学生们兴奋的评论时，<br>
> 总觉得那段狭小座位里的时光意义非凡。<br>


让我们一起制作 nano-GPT 模型！😎  
本教程提供清晰的讲解和 **100 多道填空题！🫨**  
非常适合想把兴趣转化为实质性成长的早起鸟。  
如果满足先决条件，12–18 小时即可完成。  
所有内容均可在 Google Colab 中运行。本教程基于 [Andrej Karpathy 的 nano-GPT](https://colab.research.google.com/drive/1JMLa53HDuA-i7ZBmqV7ZnA3c_fvtXnx-?usp=sharing)。  
在此特别感谢他的卓越工作。

## 目录
| 章节                             | 预估时间  | 英文 🇺🇸 | 中文 🇨🇳 | 日文 🇯🇵 |
|----------------------------------|----------|---------|---------|---------|
| Chapter 00: 入门教程             | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter00_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter00_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter00_TODO_ja.ipynb) |
| Chapter 01: 数据加载器            | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter01_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter01_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter01_TODO_ja.ipynb) |
| Chapter 02: TokenEmbedding      | 0.5–1 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter02_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter02_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter02_TODO_ja.ipynb) |
| Chapter 03: PositionEmbedding   | 0.5–1 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter03_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter03_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter03_TODO_ja.ipynb) |
| Chapter 04: EmbeddingModule     | 0.5–1 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter04_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter04_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter04_TODO_ja.ipynb) |
| Chapter 05: LayerNorm           | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter05_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter05_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter05_TODO_ja.ipynb) |
| Chapter 06: AttentionHead       | 3–4 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter06_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter06_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter06_TODO_ja.ipynb) |
| Chapter 07: MultiHeadAttention  | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter07_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter07_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter07_TODO_ja.ipynb) |
| Chapter 08: FeedForward         | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter08_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter08_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter08_TODO_ja.ipynb) |
| Chapter 09: TransformerBlock    | 0.5–1 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter09_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter09_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter09_TODO_ja.ipynb) |
| Chapter 10: VocabularyLogits    | 0.5–1 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter10_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter10_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter10_TODO_ja.ipynb) |
| Chapter 11: nanoGPT | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter11_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter11_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter11_TODO_ja.ipynb) |
| Chapter 12: Trainer             | 1–2 小时 | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/Everyones_nanoGPT_colab_Chapter12_TODO.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI/blob/main/Everyones_nanoGPT_TODO/TODO_chinese/Everyones_nanoGPT_colab_Chapter12_TODO_ch.ipynb) | [![在 Colab 中打开](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HayatoHongo/EveryonesAI_ja/blob/main/Everyones_nanoGPT_TODO_ja/Everyones_nanoGPT_colab_Chapter12_TODO_ja.ipynb) |

## **演示输出**
![nanoGPT_demo_output](assets/Everyones_nanoGPT_demo_output.png)

## **张量映射**
**请务必自行完成以下张量映射！** 下面有大量提示，无需担心。  
[在 Canva 查看 nanoGPT 模型的全分辨率张量映射。](https://www.canva.com/design/DAGskS8QP6k/1zs7IklaMrB_LncHn2I8pA/edit?utm_content=DAGskS8QP6k&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)  

![Everyones TensorMap](assets/Everyones_nanoGPT_TensorMap_answer.png)

## **先决条件**

**理解**  
- 理解矩阵乘法与加法  
- 理解均值与方差  
- 理解 ResNet 的残差连接  
- 理解 Word2Vector  
<br><br>

**经验**  
- 使用 PyTorch 构建过 MNIST 手写数字识别模型  
- 在上述模型中使用过交叉熵损失函数  
- 实现过小批量处理和批量归一化  
- 实现过自编码器或 VAE  

我们也在努力于 2025.8.30 前发布面向从未接触过 PyTorch 或编程的新手的有趣入门教程。

## **模型**
本教程使用二元模型（bigram），每个 token 即为一个字符。  
内部结构非常简单。  
训练文本数据集选用莎士比亚作品，因其年代久远，已属公有领域。  

与真正的 GPT-2 相比非常基础，但从这里起步可掌握 GPT 基础。  
在配备 16GB 内存的 PC 上，仅需 2–4 分钟 CPU 训练即可生成类似莎士比亚风格的文本，效果保证惊艳！  

## **开发环境**
为简化配置，建议在 Google Colab 中运行所有示例。  

但 Colab 无法保存复选框状态。  
若想保存进度，请在 VS Code 中操作非常方便。  
尤其适合喜欢 30 分钟短时间集中工作的用户，此时可将仓库 fork 并克隆到本地。  

推荐使用 Python 3.12 和 PyTorch 2.6.0，但大多数版本均可正常运行。  
通常已安装的 PyTorch 即可使用。  
若遇到问题，可使用 `requirements.txt` 创建虚拟环境，或使用随附的 `Dockerfile` 与 Dev Container 扩展以获得更稳定的环境。

## **关于 EveryonesAI 项目**

![EveryonesAI Logo](assets/EveryonesAI_logo.png)  
![EveryonesAI Goal](assets/EveryonesAI_goal.png)  
![EveryonesAI Idea](assets/EveryonesAI_idea.png)  
![EveryonesAI Prerequites](assets/EveryonesAI_prerequites.png)  
![EveryonesAI Plan](assets/EveryonesAI_plan.png)
