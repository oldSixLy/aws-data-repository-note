## IaaS层服务

### VPC - Virtual Private Cloud(虚拟私有云，虚拟局域网)
通俗来说，就是在AWS云平台内，为你创建一个虚拟的局域网环境，你的所有AWS资源均可定义在这个VPC内，从而实现和其他资源的逻辑隔离，以及实现VPC内高速网络带宽的访问。

#### VPC控制面板
![AWS-VPC-控制面板](/static/module-02/VPC.jpg)

#### 您的VPC
每个账户默认有个default的VPC。
![default-VPC](/static/module-02/您的VPC.jpg)

作为局域网是可以划分多个子网的.
![子网](/static/module-02/子网.jpg)

对于网络内部是需要路由控制.
![路由](/static/module-02/路由.jpg)

像网关，弹性IP，安全组等都通过VPC控制面板可以设置，其中：
弹性IP分配后可以关联我们的EC2实例还有VPC内的网络接口等。
安全组可以设置出入站规则，可以限制IP和端口。

### AWS Direct Connect
Direct Connect是一款专线服务，可以提供直通AWS云的专线服务。
日常和云服务的通讯是走公网的，日常开发没问题，但如果有大量本地内容需要和云服务通讯，传输效率会受到公网带宽的限制。
通过Direct Connect可以拉专线到AWS数据中心。**很贵**


**[回到导航栏](/README.md)**