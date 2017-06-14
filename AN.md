# JavaScript开发板Rapid使用心得
## 简述 
有幸能有机会试用体验Rapid开发板，通过该开发板可以使用JavaScript轻松、快速实现IO控制、uart通讯、TCP/IP通讯等实用功能。     
关于Rapid更多详情，请参考[https://github.com/o2ee/rapid_dev](https://github.com/o2ee/rapid_dev)    

## 准备
- Rapid开发板一块
- 手机数据线一根（MicroUSB）
- PC 一台（windows 或 Linux）

## 安装
- 登录网址[https://github.com/o2ee/rapid_dev](https://github.com/o2ee/rapid_dev) ，点击右上方的"Clone orDownload"下载Rapid开发包。    
![Download](https://github.com/ianhom/rapid_dev/blob/master/Doc/pic/01.png?raw=true)    
- 解压后，文件布局如下：

  文件夹 | 说明    
  ------|--------------    
  firmware | Rapid固件库    
  linux    | Linux系统下的JavaScript编译及下载工具    
  windows  | Windows系统下的JavaScript编译及下载工具    
  tutorial | Demo用的JavaScript脚本文件，主要的开发就是编写此文件夹中类似的JS代码    
  
## 使用（Windows示例）
- 点击windows开始按钮，搜索并运行“cmd.exe”
- 使用如下dos命令进入rapid开发包所在路径下的windows文件夹
    - “d:” ：切换至d盘    
    - “cd”：进入文件夹        
    - “dir”：查看当前文件夹下文件列表        
- 连接好rapid开发板和PC机，检查PC机对应的COM口号（假定为COM4）    
- 按下开发板复位键，并在3秒内按下wkup键    
- 输入命令rapid.exe -d COM4 ..\tutorial\led.js 烧写led例程至开发板    
- 输入命令rapid.exe -u COM4 ..\firmware\RAPID_0_0_5.bin 可更新固件    
- 烧写完成后按下复位键，程序正常运行。    

## 例程
### led.js（LED闪烁）

    
  
  
  
