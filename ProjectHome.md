本项目用于解决现网DNS解析的问题，在原有的基础上增加智能解析的功能，并配合PHP页面对DNS记录进行管理。借鉴互联网相关资料，修改并对现有问题进行修改而成. 整个思路是：
  * 通过DNS DLZ将bind的配置写入MYSQL
  * 通过php页面进行管理
  * View是整个方案的关键之一
  * 因为公司域名较少，直接使用了mysql的主主方案

这是一套完整的可用解决方案，实现之前请确保:
  * 基本的编译环境OK
  * 能够自已安装Apache+php+mysql,并调试正常运行。
  * 按照下面的内容进行.<详情请看wiki文档>

目前为了让方案能便更加方便的部署，已编写自动安装脚本，实现一键安装。
  * 访问地址: http://bind-dlz-project.googlecode.com/files/bind-dlz-auto.sh
  * 使用方法如下:
  * # chmod u+x bind-dlz-autoinstall.sh
  * 按照提示完成选择，进行安装

后续将添加APF防火墙denyhost安装