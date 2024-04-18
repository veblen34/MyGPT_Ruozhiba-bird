# SFT&MyGPT

中国人民大学机器学习期中展示代码仓库

包括MyGPT：手动实现小型大语言模型

微调CHatGLM3-6B：完成论文摘要文本二分类任务





## MyGPT

使用了射雕英雄传和弱智吧语料，以此框架可以替换为其他语料



## code (python src_code)

具体的代码使用：

- 准备好语料文件，修改 data_set.py 里面对应的文件名，然后运行 `python data_set.py`
- 再根据自己的实际情况，修改 gpt_model.py 里面的 config 参数，最后运行 `python train.py` 进行模型训练，这里使用的是4层Transformer，使用了sin-cos的位置编码策略。



## 论文文本分类任务

### 采用ChatGLM3-6B与LoRA微调方法



- 本次微调在L20-48GB上进行微调
- 注意peft版本应保持在0.4.0以下，0.7.0以上的版本对浮点数的支持有所变化





## Reference

参考了**JsonBorn7**的框架实现，是非常好的Transformer学习材料。

[https://github.com/JsonBorn7/llm-hero](https:/github.com/JsonBorn7/llm-hero)[JsonBorn7/llm-hero (github.com)](https://github.com/JsonBorn7/llm-hero)



**清华大学and智源AI**的开源预训练模型**CHatGLM3**

git项目地址：

[https://github.com/THUDM/ChatGLM3](https:/github.com/THUDM/ChatGLM3)[THUDM/ChatGLM3: ChatGLM3 series: Open Bilingual Chat LLMs | 开源双语对话语言模型 (github.com)](https://github.com/THUDM/ChatGLM3)

