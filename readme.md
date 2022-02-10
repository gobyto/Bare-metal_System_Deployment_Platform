```



wget --no-check-certificate -qO Core_Install.sh 'https://raw.githubusercontent.com/gobyto/Bare-metal_System_Deployment_Platform/main/Core_Install_v3.1.sh' && bash Core_Install.sh -dd 'https://odc.cxthhhhh.com/SyStem/CentOS/CentOS_7.X_NetInstallation_Final_v9.2.vhd.gz'



```
----------------------------------------------------
```


wget --no-check-certificate -qO Core_Install.sh 'https://raw.githubusercontent.com/gobyto/Bare-metal_System_Deployment_Platform/main/Core_Install_v3.1.sh' && bash Core_Install.sh -dd 'https://odc.cxthhhhh.com/SyStem/Bare-metal_System_Deployment_Platform/CXT_Bare-metal_System_Deployment_Platform_v3.6.vhd.gz'




```
CXT裸机系统部署平台（自定义安装任意系统）
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
Bare-metal_System_Deployment_Platform
简介
裸机系统部署平台，是【一键网络重装系统 - 魔改版】的核心组件之一，提供了最大化的自定义系统安装功能。我们从V2.x版本开始提供了本功能，提供了从裸机安装任意系统的可能（手动安装/网络ISO安装/自定义系统等）。支持UEFI+Legacy安装！

相对于一键快速安装模式，裸机系统部署平台使得您可以通过IPIM/KVM/VNC/IDRAC等进行手动安装定制，例如定制分区(RAID)，选择磁盘加密，配合您购买的特定商业ISO安装等高级安装选项。

主要用于高端用户便捷的安装任意系统，即供具有一定的折腾能力的用户使用（有特殊系统安装需求，会IPIM/KVM/VNC/IDRAC等基本操作的用户）。

版本更新
最新版本：跟随【一键网络重装系统 - 魔改版】更新

官方发布：https://www.cxthhhhh.com/bare-metal_system_deployment_platform

Github：Network-Reinstall-System-Modify

文件下载：前往【Open Disk CDN（ODC）】

文件校验（ODC最新数据）
文件名：CXT_Bare-metal_System_Deployment_Platform.vhd.gz

文件大小：53.14MB

MD5：68801a554598a665b21b5bbc4d63cd6e

SHA1：2752195384dcd41e7be8f84701a1ec08590f0a40

SHA256：d9dc2343b3d4c75f0a376ae40677e5c88dbde151295d19ff21d8692117d8b84b

如何安装（任选其一）
1、一键网络重装系统 - 魔改版
1、下载脚本（通过root用户执行）
wget --no-check-certificate -qO ~/Network-Reinstall-System-Modify.sh 'https://www.cxthhhhh.com/CXT-Library/Network-Reinstall-System-Modify/Network-Reinstall-System-Modify.sh' && chmod a+x ~/Network-Reinstall-System-Modify.sh
2、安装 裸机系统部署平台
bash ~/Network-Reinstall-System-Modify.sh -CXT_Bare-metal_System_Deployment_Platform
【合并执行】一键安装裸机系统部署平台（包含下载+执行）：

wget --no-check-certificate -qO ~/Network-Reinstall-System-Modify.sh 'https://www.cxthhhhh.com/CXT-Library/Network-Reinstall-System-Modify/Network-Reinstall-System-Modify.sh' && chmod a+x ~/Network-Reinstall-System-Modify.sh && bash ~/Network-Reinstall-System-Modify.sh -CXT_Bare-metal_System_Deployment_Platform
2、在恢复模式，手动DD镜像
手动DD（示例，按需修改镜像URL和目标磁盘）
wget -qO- 'https://odc.cxthhhhh.com/CXT_Bare-metal_System_Deployment_Platform.vhd.gz' | gunzip -dc | dd of=/dev/sda
wget -qO- 'http://127.0.0.1/CXT_Bare-metal_System_Deployment_Platform.vhd.gz' | gunzip -dc | dd of=/dev/vda
如何使用
1、连接到控制台
在成功通过以上方式安装裸机系统部署平台后，请打开并连接到您的IPIM/KVM/VNC/IDRAC等控制台。
（不会？乖，小白还是去玩一键脚本，裸机系统部署平台不适合你。或者试试自学/付费/红包请群里大佬教学）

【裸机系统部署平台】网启CXT iPXE Shell PXE BOOT安装系统

2、选择平台功能（可按键选择）
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
裸机系统部署平台-VNC演示
3、进入相应的功能（功能演示）
①. CXT_NetInstall_Tools（iPXE+netboot.xyz）
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
CXT_NetInstall_Tools（iPXE+netboot.xyz）
②. CXT_DOS_TOOLS （DOS工具箱）
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
CXT_DOS_TOOLS （DOS工具箱）
③. CXT_FileManager（grub2-filemanager）
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
CXT_FileManager（grub2-filemanager）
④. CXT_TinyCoreLinux
CXT裸机系统部署平台（自定义安装任意系统）-CXT - Enjoy Life | 生活、技术、交友、分享
CXT_TinyCoreLinux（Tiny Core Linux）
⑤. CXT_Windows-PE
即将发布！但远方又似乎飘来了咕咕咕的声音。

恭喜，你已经掌握了平台的安装
可以开始安装您想要的系统了，请随意定制。

常规说明
裸机平台仅适用于高端用户，普通用户请使用传统一键快速安装模式。
使用平台的配置需求：该系统官方要求的安装配置以上+充足的磁盘空间+充足的内存空间（映像文件缓存）。
高级模式的账户和验证密码，允许UEFI启动的安装和高级功能（UserName：root / PassWord：cxthhhhh.com）
使用裸机系统部署平台，将会进行磁盘修改，请备份好您的原始(Old)数据，否则将会造成不可挽回的损失。（您将承担一切的后果和责任）
感谢及包含
本项目中引用或包含了以下的项目的内容（不分先后），对此表示感谢，没有他们就没有裸机系统部署平台：

Grub2、iPXE、netboot.xyz、TinyCoreLinux、grub2-filemanager、Linux、Syslinux、Microsoft、Dos工具箱、Ventoy等（如有遗漏请谅解，请联系我们添加）
