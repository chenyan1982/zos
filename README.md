# zos
体验地址：

http://zos-wwccss.alaudacn.me/

禅道，蝉知和然之的管理员帐号和密码都是：admin 123456 蝉知的后台地址：http://localhost/chanzhi/admin.php

关于我们

ZOS由青岛易软天创网络科技有限公司编译维护。青岛易软天创致力于为天下企业提供专业的管理工具。我们先后以开源的方式发布了禅道项目管理软件、蝉知企业门户系统和然之协同管理系统。

ZOS的背景

在开发维护这几款开源软件的过程中，我们遇到的一个比较棘手的问题就是如何快速简便的让用户安装成功。为此我们做了各种的尝试，这其中包括制作windows的一键安装包，linux的一键安装包，rpm包,deb包等等。

后来我们尝试使用虚机提供ova格式的虚机镜像。但遇到的问题是各种linux发行版本都非常的庞大，完整的镜像做下来就要几百兆，不利于发行和下载。为此我们尝试了各种发行版本，最终选择了根据LFS(linux from scratch)进行编译。

最新版本的ZOS是根据LFS 7.6编译的。在基础的LFS上面，我们又结合BLFS编译了apache, mariadb, php, vim等常见的服务和工具，并内置了我们的三款开源管理软件。

ZOS特点

ZOS主要面向企业内部管理场景，旨在为各种管理软件提供一种罐装的发行方案，以应对越来越复杂的终端场景。
ZOS不是国产操作系统，也不是其他发行版本的精简版本。它根据linux from scratch 7.6进行编译的。
ZOS不是一个通用发行版本，主要内置了apache, php, mysql, openssh, cron, vim, rzsz, phpmyadmin等软件和服务。
ZOS进行了大量的精简，整体的docker镜像只有175M，而使用ubuntu镜像做出来同样的功能的镜像达到了460多M。
ZOS内置了简单的包管理工具(pkg)，可以实现简单的列表，查询，查看，安装，删除等操作。
如何使用

docker pull index.alauda.cn/wwccss/zos:1.1
docker run --name zos -d -p 80:80 zos /bin/start
然后使用浏览器访问主机的ip或者域名就可以看到了。
账户说明

禅道，蝉知和然之的管理员帐号和密码都是：admin 123456 蝉知的后台地址：http://localhost/chanzhi/admin.php

心得

去年的时候我自己做了一个docker的中文社区网站( http://www.docker.org.cn )，翻译了docker的基础入门手册。所以对docker有基本的了解。这次在做镜像的时候主要遇到的几个问题：

如何让镜像作为服务不退出。网上有很多方案了。我最终选择了是用 tail -f 一个文件的取巧的方式来实现。
如何将自己做的ZOS编译为镜像，本来以为很复杂，但其实还是很简单了。主要参考了红帽的一篇文章 http://developerblog.redhat.com/2014/05/15/practical-introduction-to-docker-containers/

* 支持Markdown格式 发表评论
user-logo whopawho   发表于 24 天前
搞定：原来后面要加url和具体tag

sudo docker run --name='zos' -d -p 80:80 index.alauda.cn/wwccss/zos:1.1 /bin/start
 user-logo whopawho   发表于 24 天前
~$ sudo docker run --name zos -d -p 80:80 zos /bin/start
Unable to find image 'zos:latest' locally
运行时候提示找不到镜像

 user-logo whopawho   发表于 24 天前
赞一个，马上试试。禅道在国内还是非常不错的！
