## Arch Linux 15分钟脚本

#### 功能：
* 配置分区
* 安装基本系统
* 安装显卡驱动（支持Intel/Nvidia双显卡）
* 安装配置蓝牙
* 建立用户
* 安装必要软件
* 支持选择安装主流桌面

#### 使用方法：
1. 键盘布局
# ls /usr/share/kbd/keymaps/**/*.map.gz
# loadkeys us
2. 设置字体
# setfont /usr/share/kbd/consolefonts/LatGrkCyr-12x22.psfu.gz
3. 网络 dhcpd/wifi-menu
4. 时间 timedatectl set-ntp true (使用 timedatectl status 检查服务状态)
5. 进入live系统连接网络后执行：
```
wget https://github.com/ittooo/arch/raw/master/live.sh
bash live.sh
```

*注意查看带有颜色的提示*

安装完成后记得进入/root文件夹删除config.sh文件
