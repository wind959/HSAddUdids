# HSAddUdids
超级签名中最重要的一步：跳过双重认证，自动化脚本添加udid并下载描述文件

<img src="https://raw.githubusercontent.com/HansenCCC/HSAddUdids/master/%E6%95%88%E6%9E%9C%E5%9B%BE.png"  width="400">

## 运行环境
### 编译系统：苹果Mac
### 编译系统版本：MacOS Catalina 10.15.1
### 需要终端环境：：fastlane、ruby、cocoapods 需要安装APP：Xcode
***

## 使用文档
1、cd到当前文档路径

2、修改add_udids.sh文件以下环境变量
   ```
    赋值FASTLANE_MAC_PASSWORD为当前Mac开机密码
    赋值FASTLANE_APPLEID为需要添加的appid账号
    赋值FASTLANE_PASSWORD为需要添加的appid密码
    赋值FASTLANE_APPLE_APPLICATION_SPECIFIC_PASSWORD(进入苹果官网生成的特殊密码APP-SPECIFIC https://appleid.apple.com/account/manage)
    赋值FASTLANE_SESSION(执行fastlane spaceauth -u user@email.com，生成session cookie)
```

3、使用终端执行 sh add_udids.sh 需要添加的udid集合，以空格隔开
    e.g,
```
sh add_udids.sh 6f1b77ce2ff2cd5672734e00facbe97f305f9ddb 6f1b77ce2ff2cd5672734e00facbe97f305f9ddb 6f1b77ce2ff2cd5672734e00facbe97f305f9ddb
```


***
## 参考文档
#### [fastlane官方文档](https://docs.fastlane.tools/ "fastlane官方文档")
#### [关于spaceship工具的简单了解](https://www.jianshu.com/p/1d63bfef1738 "关于spaceship工具的简单了解")
#### [fastlane使用说明书和处理关于开启两步验证如何全自动化问题](https://www.jianshu.com/p/19ae8cc865b0 "fastlane使用说明书和处理关于开启两步验证如何全自动化问题")
#### [使用fastlane创建profile、添加设备、创建推送证书 以及上传蒲公英](https://www.jianshu.com/p/2defceba2761 "使用fastlane创建profile、添加设备、创建推送证书 以及上传蒲公英")
#### [搭建 超级签 详细攻略](https://blog.csdn.net/LiaoQuesg/article/details/101219984  "搭建 超级签 详细攻略")
#### [自动化打包---打包上传App Store Connect](https://www.jianshu.com/p/16e0d9b8e7ca Fastlane "自动化打包---打包上传App Store Connect")
#### [fastlane/spaceship/docs/DeveloperPortal.md](https://github.com/fastlane/fastlane/blob/master/spaceship/docs/DeveloperPortal.md#example-data "fastlane/spaceship/docs/DeveloperPortal.md")
#### [从创建证书到上传到App Store](https://www.jianshu.com/p/db52889f20d0 Fastlane "从创建证书到上传到App Store")
#### [记一次设置Fastlane支持苹果双重认证的过程](https://www.jianshu.com/p/665efd203259 "记一次设置Fastlane支持苹果双重认证的过程")
***



## 我
#### Created by 程恒盛 on 2019/12/3.
#### Copyright © 2019 力王. All rights reserved.
#### QQ:2534550460@qq.com  GitHub:https://github.com/HansenCCC  tel:13767141841
#### copy请标明出处，感谢
