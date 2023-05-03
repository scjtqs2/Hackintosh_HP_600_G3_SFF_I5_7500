# Hackintosh_HP_600_G3_SFF_I5_7500
感谢`悉心研究`大佬 py的 `HP 600G3 SFF`机器。很适合用来折腾，这里提供一个折腾的efi记录。
由于机器自带的 cpu 是 `i3-6100`，不支持 `macos 13（Ventura）`，因此换了个7500来上`macos 13（Ventura）`

### 我的电脑配置：

| 硬件名称 | 型号                |
|------|-------------------|
| CPU  | i507500           |
| 显卡   | HD630             |
| 主板   | hp q270           |
| 内存   | 三星 8g ddr4 （机器自带） |
| 硬盘   | 梅捷(soyo) nvme 1T  |
| 网卡   | Bcm94360cs2       |
| 机箱   | HP 600G3 SFF      |
| 电源   | 自带的180W 铂金80plus  |

### bios 设置：
+ 关闭 传统引导支持，并禁用安全启动。
+ 关闭 快速启动
+ 关闭 vt-d
+ 显存 调整为 512M

### opencore版本：
0.9.1

### macos版本：
macOS Ventura
13.3.1

### 说明
请自行修改/添加 三码

使用 `Hackintool` -> `电源` -> `螺丝刀图标` 来修复电源相关的配置

### Win+Mac双系统解决Win系统时间时差问题

在Windows终端下使用管理员权限运行 
```
Reg add HKLM\SYSTEM\CurrentControlSet\Control\TimeZoneInformation /v RealTimeIsUniversal /t REG_DWORD /d 1
```

### 设置默认启动项

    多系统在启动选择界面，先使用键盘移动到要启动的项，然后按Ctrl+Enter(回车键)进入系统，下次重启后默认就选中该项了


