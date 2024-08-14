# Windows平台gcc编译链+Makefile开发STM32（基于STM32CubeMX重制版）
## <font color = #f07c82>开发环境搭建</font>
### 前言
一些同学可能看过之前发的这个系列的教程，详情见[这个视频](https://www.bilibili.com/video/BV1Hi4y1r7b3/?spm_id_from=333.999.0.0&vd_source=6603016c0f602d079e3f53f0b71602e5)，本期主要是对上一个视频的补充，但是也会演示完整的流程，所以两个视频选一个看就好了，同学们均可以完美复刻本期教程的内容
### 工具下载
* 编译器：[arm-none-eabi-gcc-xpack](https://github.com/xpack-dev-tools/arm-none-eabi-gcc-xpack)
  - 食用方法：解压至任意磁盘，再将目录下的bin文件目录添加到环境变量
  - 验证工具生效与否：打开PowerShell或者终端，输入`arm-none-eabi-gcc -v`检查窗口是否有版本信息输出
* 编辑器：[VS Code](https://code.visualstudio.com/download)
  - 编辑器千万款，我只推荐这一款
* 烧录&&调试工具：[OpenOCD](https://github.com/xpack-dev-tools/openocd-xpack/releases)
  - 食用方法：解压至任意磁盘，再将目录下的bin文件目录添加到环境变量
  - 验证工具生效与否：打开PowerShell或者终端，输入`openocd -v`检查窗口是否有版本信息输出
* 构建工具：[make](https://sourceforge.net/projects/gnuwin32/files/make/3.81/make-3.81.exe/download?use_mirror=jaist&download=)
* 终端命令行工具：[git](https://git-scm.com/download/win)
  - 非必须，但是推荐尝试，之后的.vscode脚本里会调用这个工具，还会用到make的原生指令，`make clean`，这是上一个教程未提及到的工具，推荐指数：★★★★★
### VS Code插件下载
* C/C++
* Cortex Debug
* Task Buttons
## <font color = #f07c82>使用STM32CubeMX创建工程</font>
这里我们以STM32F407VET6开发板作为演示，移植一个SSD1306 0.96''OLED的驱动，[ssd1306原驱动下载地址](https://github.com/afiskon/stm32-ssd1306)
> * Generate Code时，Toolchain下拉勾选Makefile
## <font color = #f07c82>使用VS Code打开工程</font>
- 添加.vscode模板文件到新建工程
  > 此处的.vscode我会提供一份，但仅限参考，实际使用需要根据自己的工程进行修改
- 讲解.vscode各个json文件的用处，在一定程度上解惑
## <font color = #f07c82>导入驱动</font>
- 这部分的内容请看视频讲解
## <font color = #f07c82>编写，编译，烧录，调试代码</font>
- 这部分的内容请看视频讲解
