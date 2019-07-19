## 环境

python3

## 运行

```bash
pipenv install
 
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

## 百度词法分析
- 识别准确度更高
- 有qps限制
> 解决限流问题可以使用 ratelimiter