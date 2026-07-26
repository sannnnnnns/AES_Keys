这是一个用于解包三角洲的aes_key
---
# DeltaForce_Unpacking 三角洲行动 PAK 查看教程
## 一、软件下载
使用软件：FModel

官网地址： https://fmodel.app
下载方式：点击官网左上角蓝色按钮 Download Now，获取压缩包
解压后得到 FModel.exe，可存放到任意目录

## 二、PAK 读取
启动 FModel，进入主界面后按以下步骤操作：

1. 选择游戏目录
点击左上角菜单栏 Directory -> Selector
2. 设置弹窗参数
Directory：选择《三角洲行动》的 PAK 文件目录
示例：D:\Delta Force\Delta Force\DeltaForce\Content\Paks
UE Versions：搜索并选择 DeltaForce（重要！）
Detected Game：确保自动变为 Paks（否则手动修改）
点击 OK，软件将自动重启。
重启后，FModel.exe 所在目录下会出现 Output 文件夹，左侧会显示 PAK 文件列表。

## 三、AES 加载
获取储存 AES Key 的文件链接
本项目AESkey文件链接为：https://raw.githubusercontent.com/HanKongXingYu/DeltaForce_Unpacking/refs/heads/main/FModel/AES_Keys_1.json
菜单栏点击 Settings → 找到 AES 并点击
在 AES 配置界面：
左侧输入框中填入储存 AES Key 的文件链接，点击 Send
下方显示文件内容后，在右侧输入表达式 $.['MainKey','Keys'] ，点击 Test 测试
右侧出现内容、下方提示变为“通过”后，点击 OK
关闭 Settings 窗口，回到主界面
菜单栏点击 Directory → AES，进入 AES manager 窗口
点击 Refresh 等待加载
向下滚动，确保所有文件都已填入 Key，点击 OK
四、加载 PAK 文件
所有文件亮起（变为可加载状态）后：

单独打开：双击某个 PAK 文件
加载全部：将 LoadingMode 选择为 ALL，点击 Load
加载后会跳转到 Folders 选项卡，即可看到所有 PAK 整合后的文件目录。

后续 FModel 的详细使用请自行搜索。

**本教程仅提供技术学习参考，请遵守相关游戏的使用条款。**

原文作者：![HanKongXingYu](https://github.com/HanKongXingYu) 由于这位大佬提供的key有问题，所以我改了一下
