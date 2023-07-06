# Klipper

## 目前我的认知

![img.png](assets/img.png)



Klipper 文档中默认推荐使用 [OctoPi 系统镜像](https://www.klipper3d.org/Installation.html#prepping-an-os-image)，其中预装了 OctoPrint。
这是一个通用的 3d 打印管理系统。
 
但是OctoPi OS 和 OctoPrint 并不是唯一选择。

Voron 文档中还给出另外 [2 个管理系统](https://docs.vorondesign.com/build/software/) ：
- Mainsail
- Fluidd

虽然我已经装好了 OctoPi OS，但还是决定切到 Mainsail OS。

Maimsail 文档比较简单，没有 OctoPi 贴心，这里贴一下系统镜像写入后的操作：

```
Log into your Pi via SSH (it is located at octopi.local if your computer supports bonjour or the IP address assigned by your router), default username is "pi", default password is "raspberry". Run sudo raspi-config. Once that is open:

Change the password via "Change User Password"
Optionally: Change the configured timezone via "Localization Options" > "Timezone".
Optionally: Change the hostname via "Network Options" > "Hostname". Your OctoPi instance will then no longer be reachable under octopi.local but rather the hostname you chose postfixed with .local, so keep that in mind.
You can navigate in the menus using the arrow keys and Enter. To switch to selecting the buttons at the bottom use Tab.

You do not need to expand the filesystem, current versions of OctoPi do this automatically.
```


## 关于固件

目前手里有一个古董 MKS base v1.3 里面刷了 Marlin 固件。 试了一下是可以用 octoprint 控制打印的 (就和以前用电脑软件联机打印一样，只不过现在连的是树莓派）。

尝试了刷入 klipper 固件，固件刷入成功，但是全网都没找到合适的 配置文件。有时间再研究，睡觉。

