
# LightGBM 安装


## 在 Windows 下的安装


1.下载源代码

```
git clone --recursive https://github.com/Microsoft/LightGBM
```

2.编译 DLL

进入`LightGBM` 目录，用 VS2015（或者更高的版本）打开 `windows/LightGBM.sln`，选择 DLL 和 x64，按 `Ctrl+Shift+B` 进行编译，dll文件就会在`windows/x64/DLL/`目录里。注意，一定要是 VS2015 以上的，如果没有 VS2015，可以参考下[官网的其它方法](http://lightgbm.apachecn.org/cn/latest/Installation-Guide.html)，写的还是很清楚的。

<p align="center">
    <img width="70%" height="70%" src="http://images.iterate.site/blog/image/180729/cLIi3FLFIf.png?imageslim">
</p>

3.安装 python 包

进入目录`python-package`  执行命令：


```
python setup.py install
```


4.测试一下

进入`examples\python-guide` 执行样例：


```
python .\simple_example.py
```

如果没有报错，那就说明安装成功了。





# 相关

1. [ LightGBM 中文文档](http://lightgbm.apachecn.org/cn/latest/index.html)
2. [在 Windows 下安装 LightGBM 的 python 包](https://blog.csdn.net/jiaqiangbandongg/article/details/53814663)
