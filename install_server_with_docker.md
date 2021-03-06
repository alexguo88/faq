# 阿卡信服务器快速搭建教程

## 两行命令拥有阿卡信服务器

通过我们发布的Docker镜像，可以最快速的完成服务器搭建工作，整个过程只需两行命令。

> 如果你没有Docker环境，请看下面的Docker一键安装教程。

````shell
# 请认准我们的官方镜像，无毒无害实时更新
docker pull registry.cn-qingdao.aliyuncs.com/akaxin/openzaly:latest

# hostBaseDir需要更改成你本地的绝对目录，服务器的日志、图片、数据库将存储在这个位置
docker run -tid -v hostBaseDir:/akaxin -p 2021:2021 registry.cn-qingdao.aliyuncs.com/akaxin/openzaly:latest

````

通过上面的两行命令安装完成后

````shell
docker ps -l
````

看到镜像，处于运行中，代表镜像运行成功，可以通过app访问站点。


## 一键安装Docker教程

快速安装基于Docker，以下是Docker的一键安装教程，**如果你已经拥有Docker环境，请跳过**。

* [Linux](<demo.md>)
    * 直接通过yum、apt安装即可。
    * 或者访问：https://www.docker.com/community-edition#/download
* [Mac OSX](<https://store.docker.com/editions/community/docker-ce-desktop-mac>)
* [Windows Pro\Server](<https://store.docker.com/editions/community/docker-ce-desktop-windows>)


----

使用过程若有任何问题，欢迎联系我们 hi@akaxin.xyz
