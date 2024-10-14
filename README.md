# Debian

#### 显示模式配置
切换到集成显卡 (Intel 或者 AMD):

`sudo envycontrol -s integrated`

切换到混合模式，平衡性能和功耗:

`sudo envycontrol -s hybrid --rtd3`

切换到 NVIDIA 独立显卡模式，:

`sudo envycontrol -s nvidia --force-comp`

---

`/home/m2joy/.local/share/plasma/desktoptheme` 这是存放`plasma`主题 

`/home/m2joy/.local/share/plasma/look-and-feel/` 存放全局主题 

`/home/m2joy/.local/share/plasma/plasmoids/` 存放插件 

以上目录如果没有就自行创建。

#### 扩容swap分区方法
![](./img/swap.jpg)

# Arch

#### 解决因nvidia驱动原因导致的无法休眠问题
![](./img/hibernate.jpg)