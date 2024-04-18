# MyGPT

使用了射雕英雄传和弱智吧语料，以此框架可以替换为其他语料



## code (python src_code)

具体的代码使用：

- 准备好语料文件，修改 data_set.py 里面对应的文件名，然后运行 `python data_set.py`
- 再根据自己的实际情况，修改 gpt_model.py 里面的 config 参数，最后运行 `python train.py` 进行模型训练，这里使用的是4层Transformer，使用了sin-cos的位置编码策略。

### Reference

参考了JsonBorn7的框架实现，是非常好的Transformer学习材料。

[https://github.com/JsonBorn7/llm-hero](https:/github.com/JsonBorn7/llm-hero)[JsonBorn7/llm-hero (github.com)](https://github.com/JsonBorn7/llm-hero)