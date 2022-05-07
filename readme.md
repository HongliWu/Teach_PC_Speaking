# 教电脑说人话！
**讲解视频：**

**参考程序：https://github.com/lturing/tacotronv2_wavernn_chinese**

**执行步骤：**

1、新建一个空的文件夹，这里以Teach_PC_Speaking为例。

2、在文件夹中打开终端，并执行 
```bash
git clone https://github.com/lturing/tacotronv2_wavernn_chinese.git
```
3、创建新的隔离环境，
```bash
conda creat -n speak python=3.6
```

4、修改requirement文件，改成和本项目中的requirement文件一致。
```bash
cd tacotronv2_wavernn_chinese
vim requirements.txt
```

5、切换到新建的独立环境并安装依赖包(使用豆瓣镜像进行加速)
```bash
conda activate speak
pip install -r requirements.txt -i https://pypi.douban.com/simple/
```

6、使用 python tacotron_synthesize.py 即可生成男声。

7、修改或替换tacotron_synthesize.py文件，将本项目中训练好的权重放进去。

8、使用 python tacotron_synthesize.py 即可生成金克斯的语音。