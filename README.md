## 环境

python3

## 运行

```bash
cp app.config.example app.config

pipenv install
```
配置 app.config

```bash
pipenv run python main.py
```

## python-docx
读取docx内容
- Document对象，表示一个word文档。
- Paragraph对象，表示word文档中的一个段落
- Paragraph对象的text属性，表示段落中的文本内容。
- Table对象，表示word文档中的一个表格
> Table包含rows，每个row包含cells,cell.text表示表格中某一个单元格的内容

## 命名实体分析

### Hanlp
- 本地库，同步调用，识别速度快
- 识别精度有限

https://github.com/hankcs/HanLP

## 百度词法分析
- 识别准确度更高
- 有QPS限制 ( QPS（query per second）指每秒向服务发送的请求数量峰值，相当于每个API每秒可以允许请求的最大上限数量)
> 解决限流问题可以使用 ratelimiter

https://ai.baidu.com/docs#/NLP-Python-SDK/top