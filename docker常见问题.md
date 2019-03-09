##  docker常见问题

#### 1.IDEA docker控制台中文乱码的解决方式

	参考: 
[IDEA docker控制台中文乱码的解决方式](https://wangyaozheng.top/article/21)

	问题如下图:
  ![](img/b1.png)

	解决方法:
	查看其环境配置语言是否是C.UTF-8
  ![](img/b2.png)
	可是还是有乱码，查看IDEA file encoding默认编码是不是UTF-8
	如果设置的没问题，显示还是有乱码，那么请把下边的代码-Dfile.encoding=UTF-8复制到
  ![](img/b3.png)
	这两个文件的末尾
  ![](img/b4.png)
	再次启动docker 部署
  ![](img/b5.png)