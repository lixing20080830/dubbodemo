# dubbodemo run

1 启动zookeeper<br>
2 启动tomcat，运行dubbo-admin<br>
3  dubbodemo项目dubboprovider的applicationContext.xml文件修改<br>
![Image text](https://github.com/lixing20080830/dubbodemo/raw/master/images-folder/1.png)<br>

4 启动Provider<br>
![Image text](https://github.com/lixing20080830/dubbodemo/raw/master/images-folder/2.png)<br>

5 启动Consumer<br>
![Image text](https://github.com/lixing20080830/dubbodemo/raw/master/images-folder/3.png)<br>

6 打开http://localhost:8888/dubbo-admin-2.6.0 查看providers<br>
![Image text](https://github.com/lixing20080830/dubbodemo/raw/master/images-folder/4.png)<br>


tips注册中心只负责服务注册和目录发布，安全授权，实际的服务访问仍然是两个组件之间的点对点连接完成，这种方式下整个架构下获取更高的性能，同时服务管理平台也不容易成为大并发服务访问下的单点瓶颈
![Image text](https://github.com/lixing20080830/dubbodemo/raw/master/images-folder/5.png)<br>
