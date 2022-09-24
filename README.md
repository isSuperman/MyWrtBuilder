# MyWrtBuilder
使用 OpenWrt ImageBuilder 快速构建可定制化的 OpenWrt 固件。

### 这是什么？

在尝试了网上流行的各种乱七八糟的 OpenWrt 固件之后，我始终没能找到一个最适合自己用的固件。

最终，我选择了一个最接近自己的期望的固件上游：[ImmortalWrt](https://github.com/immortalwrt/immortalwrt)，选择这个固件的原因有纯净的使用体验以及足够丰富的软件源等等。但是纯净的固件仍然不能开箱即用，于是我决定使用 ImmortalWrt 提供的 Image Builder 自定义自己的固件，于是便有了这个项目。

### 本项目特点

* 使用 ImageBuilder 构建固件，省时省力，构建一次最多只需要不到半个小时。
* 集成了(我自己)日常会用到的 Luci 软件包，更换了 Argon 主题，开箱即用。
* 只需简单修改 build.sh 即可二次构建属于你自己的固件，方便定制。
* ~~更换了好看的登录页面背景~~

### 固件截图

登录界面：

![](https://raw.githubusercontent.com/Revincx/MyWrtBuilder/main/img/login.png)

内置组件：

![](https://raw.githubusercontent.com/Revincx/MyWrtBuilder/main/img/apps.png)

主界面：

![](https://raw.githubusercontent.com/Revincx/MyWrtBuilder/main/img/main_status.png)

### 食用方法

如果你对上图中我内置的组件感到满意，可以直接在 Release 页面下载编译完成的固件刷入使用。

如果你想添加或删除其他内置组件，只需 Fork 本仓库，修改 build.sh 然后进入 Actions 编译即可。

### 计划中的想法

由于修改 build.sh 进行定制的方法仍然不够人性化，所以我在考虑设计一个图形化的界面以生成自定义的组件组件列表。只需自助勾选所需要的组件然后即可一键生成构建配置文件，然后上传配置文件到 GitHub 仓库中即可开始构建。

不过这个目前只是想法罢了，做出来的话可能还得鸽很长一段时间（

### 鸣谢

[OpenWrt](https://github.com/openwrt/openwrt/)

[ImmortalWrt](https://github.com/immortalwrt/immortalwrt)

[GitHub Actions](https://github.com/features/actions)
