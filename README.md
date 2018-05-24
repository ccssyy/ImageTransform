# ImageTransform
StyleTransform
1.先从http://download.tensorflow.org/models/vgg_16_2016_08_28.tar.gz 上下载
vgg16 模型，在项目根目录下创建pretrained 文件夹，将上述vgg16 模型解压得
到的.ckpt 文件存放在pretrained 文件夹下。
2. 训练是用COCO 数据集， 下载链接
http://msvocds.blob.core.windows.net/coco2014/train2014.zip ， 将解压得到的
train2014 文件夹拷贝到项目根目录下。
3.可在命令行下输入命令：
python train.py --conf conf/wave.yml
训练相应的风格。模型保存在models/wave/下。
4.使用模型：将models/wave/下的模型拷贝到models/下，扩展名命名为.ckpt-done，运行
web.py，在浏览器中打开地址http://127.0.0.1:5000/显示web 界面。
