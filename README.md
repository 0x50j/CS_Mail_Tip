Cobalt Strike主机上线邮件提醒插件

食用说明

0x01:
将`Aggressor_mail.jar`和`Aggressor_email_gui.cna`这两个文件移动到Cobalt Strike的目录下

0x02:
修改`Aggressor_email_gui.cna`文件的34 ~ 37 行的代码内容

    %defaults["smtp"] = "发件服务器地址";
    %defaults["myEmailAccount"]  = "邮箱账号";
    %defaults["myEmailPassword"] = "邮箱密码";
    %defaults["Sender"] = "CS New Host Online";
    %defaults["Recipients"] = "收件邮箱";

0x03:
然后使用CS自带的agscript工具启动,启动命令参数如下:
`agscript <host> <port> <user> <pass> </file/Aggressor_email_gui.cna>`

<img src='https://resource.0x50j.com/Aggressor_01.png' />

0x04:
最后在客户端界面加载`Aggressor_email_gui.cna`插件即可
