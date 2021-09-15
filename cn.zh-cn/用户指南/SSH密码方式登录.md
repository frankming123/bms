# SSH密码方式登录<a name="zh-cn_topic_0053537015"></a>

## 操作场景<a name="section17306435184815"></a>

本节操作介绍在Windows和Linux环境中使用SSH密码方式登录Linux裸金属服务器的操作步骤。

## 前提条件<a name="section33044631113942"></a>

-   裸金属服务器状态必须为“运行中”。
-   裸金属服务器已经绑定弹性公网IP，绑定方式请参见[绑定弹性公网IP至服务器](绑定弹性公网IP至服务器.md)。
-   已配置安全组入方向的访问规则，配置方式请参见[添加安全组规则](添加安全组规则.md)。
-   使用的登录工具（如PuTTY）与待登录的裸金属服务器之间网络连通。例如，默认的22端口没有被防火墙屏蔽。

>![](public_sys-resources/icon-note.gif) **说明：** 
>密钥登录方式创建的Linux裸金属服务器，如需使用用户名和密码方式登录，请先使用[远程登录方式](远程登录方式.md)登录裸金属服务器，开启SSH密码登录权限，具体操作请参见[如何设置SSH服务配置项](https://support.huaweicloud.com/bms_faq/bms_faq_0040.html)。

## 本地使用Windows操作系统<a name="section62238598113942"></a>

如果本地使用Windows操作系统的计算机，您可以按照下面方式登录Linux裸金属服务器（以PuTTY工具为例）。

>![](public_sys-resources/icon-note.gif) **说明：** 
>PuTTY工具下载地址：[https://www.chiark.greenend.org.uk/\~sgtatham/putty/latest.html](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

1.  运行PuTTY。
2.  在左侧目录中选择“Session”，在“Host Name \(or IP address\)”下的输入框中输入裸金属服务器的弹性公网IP地址，连接方式选择SSH。
3.  在左侧目录中选择“Windows \> Translation”，在“Received data assumed to be in which character set:”下拉框中选择“UTF-8”。
4.  单击“Open”。
5.  输入用户名“root”和创建裸金属服务器时设置的密码，登录裸金属服务器。

## 本地使用Linux操作系统<a name="section6934158113942"></a>

如果本地使用Linux操作系统的计算机，您可以在计算机的命令行中运行如下命令，登录Linux裸金属服务器。

**ssh** _裸金属服务器__的弹性公网IP地址_

