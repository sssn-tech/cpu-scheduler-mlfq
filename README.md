# cpu-scheduler-mlfq

一个基于python-tkinder的图形化CPU多级反馈队列调度模拟程序

2022级吉林大学软件学院操作系统课程设计

图形化模拟了操作系统对5个不同算法的进程反馈队列与1个CPU核心, 1个等待队列的调度情况, 涉及多种反馈算法, 时间片管理, 上下文切换, 终断控制, 进程唤醒, 等待队列阻塞等常见功能

用户可以手动控制时间流动, 添加进程, 开/关自动生成进程, 开/关等待队列阻塞, 手动发起中断, 开/关随机中断, 或者将当前结果保存为列表输出到文件

5个队列中, 靠上方的优先级更高, CPU优先索取FIFO1, 如果为空, 索取FIFO2, 依次类推. 如果全部为空, 则返回一个闲逛进程. CPU会实时显示当前运行的进程, 可能是随机进程, 用户生成的进程, 随机中断, 用户中断, 或闲逛进程

## 主界面截图
<img src="https://pic.cirno.fun/sssn-blog-pics/image-20241212162749235.png" alt="描述" style="max-width:100%; height:auto;">

## 输出结果截图

![image-20241212161115339](https://pic.cirno.fun/sssn-blog-pics/image-20241212161115339.png)

## 程序框图

![image-20241212161257339](https://pic.cirno.fun/sssn-blog-pics/image-20241212161257339.png)

![image-20241212161328191](https://pic.cirno.fun/sssn-blog-pics/image-20241212161328191.png)
