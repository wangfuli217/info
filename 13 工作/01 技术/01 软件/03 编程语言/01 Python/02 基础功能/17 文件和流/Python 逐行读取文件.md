



```py
f = open("foo.txt")               # 返回一个文件对象
line = f.readline()               # 调用文件的 readline()方法
while line:
    print line,                   # 后面跟 ',' 将忽略换行符
    # print(line, end = '')　     # 在 Python 3 中使用
    line = f.readline()
f.close()
```


```py
for line in open("foo.txt"):
    print line
```






```py
f = open("c:\\1.txt","r")
lines = f.readlines()      #读取全部内容 ，并以列表方式返回
for line in lines
    print line
```




# 相关

- [Python逐行读取文件内容的三种方法](https://www.cnblogs.com/dingd/p/5775919.html)
