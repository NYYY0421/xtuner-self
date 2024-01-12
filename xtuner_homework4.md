### 基础作业 微调自己的小助手
1. 自己名字的小助手

环境：xtuner0.1.9
数据格式
![Alt text](image-1.png)
训练：
![Alt text](image.png)
训练后的pth格式参数转Hugging Face格式  
![Alt text](image-2.png)
Merge模型参数
![Alt text](image-3.png)
输出是本人的小助手：
![Alt text](1704979261667.png)

2. 自定义微调
```bash
ft-medqa/work_dirs/internlm_chat_7b_qlora_medqa2019_e3/internlm_chat_7b_qlora_medqa2019_e3.py
```
转换为huggingface模型
![Alt text](image-4.png)
merge 
![Alt text](image-5.png)
测试一下微调效果：
![Alt text](image-6.png)
msagent:
拷贝配置文件
![Alt text](image-7.png)
运行：
![Alt text](image-8.png)
*最后的结果和视频中类似，都是没有成功调用到api*

### 进阶作业
#### 上传自己的权重文件到huggingface
*参考了https://huggingface.co/docs/huggingface_hub/guides/cli#specify-a-token 的上传教程*
1. 安装huggingface_hub
```bash
pip install huggingface_hub
```
2. 登录，（我使用了clash代理）
```bash
huggingface-cli login
```
![Alt text](image-9.png)
3. 上传文件
![Alt text](image-14.png)
上传成功：   
地址https://huggingface.co/NYYY0421/mymodel/tree/main
![Alt text](image-15.png)
