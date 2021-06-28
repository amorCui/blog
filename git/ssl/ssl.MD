问题描述：
使用SmartGit工具clone项目时，弹出框提示信息为“XXXX，SSL certificate problem: self signed certificate”

问题分析：
提示信息为SSL认证失败，可以关闭SSL的认证

解决方案：
1.在windows的命令行窗口执行指令：
  set GIT_SSL_NO_VERIFY=true git clone
2.在windows的命令行中，进入到git命令所在的磁盘位置，执行下面的git命令：
  git config --global http.sslVerify false
