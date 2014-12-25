FPGA-verilog-AES
================

a group programme
Mobile Cloud Security 
-基于FPGA+verilog的AES线性分析


各组员：王西子，杨帆，汪洋一舟，孙徐涛，刘奕

模块功能介绍：
AES_mul.v为实现有限域乘法的模块
AES_NY.v为实现有限域求逆元的模块
AES_plus.v为实现有限域加法的模块
（有限域加法和乘法运算方法大致相同，除法即乘以逆元）
linear.v为AES算法线性分析并输出偏差最大方程的模块
tb_AES.v为求逆元模块的测试模块
tb_AES_mul.v为乘法模块的测试模块

测试方法简介：
需要在Modelsim中运行。
在ModelSim中新建工程，导入上述各个模块。

导入成功后进行编译：这两个按钮为Compile
编译成功出现如图所示的勾，可以开始仿真，点击

选择所要仿真的测试模块（只要测试模块就可以了）
（Optimization中的Enable optimization勾不要打）
Eg.我们要仿真逆元模块，即选择逆元模块进入仿真界面：

右键aes选择Add wave，再选择菜单栏的run-all图标点击即可开始运行测试模块，也可以看到仿真的波形在wave中。


也可以通过选择菜单栏的View，打开Transcript查看monitor控制台输出。
