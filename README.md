##	机型信息
- Intel i5-1035G4
- Intel Iris Plus Graphics G4
- LPDDR4X 3200MHz 16GB
- Intel AX201
- Conexant CX8400

## 安装的是Big Sur(11.4)
## Catalina(10.15.7)开启HIDPI依旧会闪屏

## 已知问题
- 开机闪屏
- 内置麦克风为`Intel Smart Sound Technology`英特尔智音技术，未能驱动(和联想小新Pro13同样的问题)
- 官方驱动中移除了HDMI驱动，机身HDMI不能使用，需要使用type-c转接

## BIOS设置
- 设置硬盘模式为AHCI
- 禁用FastBoot

## 可选
- 设置`DVMT Pre-Allocated`为`04(128M)`或`05(160M)`，图中修改为05后不能进BIOS应该是其他问题，重置NVRAM后正常
- 禁用CFG Lock
- 开启HIDPI

### 修改BIOS设置
#### 修改有风险，请谨慎操作
#### 在1.08上测试正常，不保证其他版本没有问题
1.先打开`WDFInst.exe`，再打开`H2OUVE-W-GUIx64.exe`

2.点击`File->Load runtime`

3.点击左侧绿色`Variable`

4.执行下面的修改

  - DVMT Pre-Allocated
  ![image](https://github.com/Jarvay/Acer-Swift3-SF313-52/blob/master/images/Change%20DVMT%20Pre-Allocated.png)

  - 禁用CFG Lock
  ![image](https://github.com/Jarvay/Acer-Swift3-SF313-52/blob/master/images/Disable%20CFG%20Lock.png)
  
5.点击File下的图标保存，重启

[工具下载](https://wwa.lanzous.com/iTECYn6dlcf)

参考文章(https://zhuanlan.zhihu.com/p/266400995)
更多修改可参考工具中的txt文件
