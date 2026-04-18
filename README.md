# RAG Code Assistant (基础版)

基于检索增强生成（RAG）的代码库问答助手。支持将本地代码库索引到向量数据库，并通过智谱AI大模型回答问题。

## 功能
- 索引 Python、Markdown、TXT 等文件
- 根据自然语言问题检索相关代码片段
- 结合大模型生成答案
- 支持多轮对话（历史记忆）

## 安装
1. 克隆仓库
2. 创建虚拟环境：`python -m venv venv`
3. 激活：`.\venv\Scripts\activate`
4. 安装依赖：`pip install -r requirements.txt`
5. 设置环境变量：`$env:ZHIPUAI_API_KEY="你的Key"`
6. 运行索引（仅首次）：`python indexer.py`
7. 启动：`python main.py`

## 技术栈
- Python
- Chroma（向量数据库）
- Sentence-Transformers（嵌入模型）
- 智谱AI（LLM）