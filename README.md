# HC-SR04-
基于 正点原子战舰（stm32f103zet6）
# 接线
HC-SR04+ 超声波测距模块与HC-SR04完全兼容，工作电压**3V-5.5V**
- **VCC：+5V**
- **Trig:Pb7**
- **Echo:Pb6**
- **GND:GND脚为此模块作为防盗模块时的开关输出量，测距模块不用此脚！！！**

# 原理
## ![原理图](https://img1.baidu.com/it/u=3720495336,2999906006&fm=26&fmt=auto&gp=0.jpg)

## 采用IO（Trig）触发测距，给至少10us的高电平，实际40-50us效果好
有信号返回，通过IO（Echo）输出一高电平，高电平持续的时间就是超声波从发射到返回的时间
