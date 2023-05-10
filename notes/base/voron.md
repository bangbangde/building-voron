# 关于 voron
Voron 官方网站：https://vorondesign.com/

![image](https://user-images.githubusercontent.com/16101554/237026096-1d16e82b-9016-4f05-adb7-5dad86d47008.png)

### Voron 机型
**Printers** 板块下列出了所有 Voron 机型和采购指南，点击进入具体机型页面，可以查看该机型的图片集、下载 3d 模型、填写配置表单并生成采购清单。

![image](https://user-images.githubusercontent.com/16101554/237030956-9382a220-8626-4591-a8f9-8d92b7ba2da8.png)

现在不需要纠结到底要选哪一款，看过 Documentation 再做决定。

### 挤出机&打印头
**Toolheads and Extruders** 板块介绍了两个模块： M4挤出机 和 StealthBurner热端。单独介绍他俩是因为他们是所有机型通用的组件？可能吧🤔️


### Documentation

真正了解 Voron 的地方。

# 快速了解 voron
## Motion System 运动系统
使用 CoreXY 或 CoreXZ 结构，降低运动部件质量以提高打印速度。

使用 线轨（MGN7,MGN9或MGN12）或 光杆。

使用 Gates皮带 6mm 或 9mm。（建议使用正版）

使用两个带法兰的 F695 轴承叠在一起作为惰轮

## Frames 框架
V1、V2和Legacy框架使用的是2020铝型材，其槽宽为6mm。而V0则使用1515 Makerbeam XL型材，而Switchwire则使用6030和3030型材进行构建。

请确保注意铝型材的配置，因为即使外部尺寸相等，不同的铝型材类型也可能存在差异。

## Motion Control - Klipper 运动控制系统
[Klipper](https://www.klipper3d.org/Overview.html) 使用一个树莓派作为上位机，运行计算任务，将预处理后的指令发送到控制板。

优点：
- 可以灵活选择控制板
- 配置简单快捷
- 上位机具备震动解耦的能力

## Serial Numbers 序列号
只要你完成了打印机的组装，就可以获得一个序列号，方法是在 Voron [Subreddit](https://www.reddit.com/r/voroncorexy/) 上发布一段你的打印机正在打印的视频。

请确保打印机整理干净，布线尽量整洁。

注意：现在序列号提交过程更加自动化（爬虫会自动爬取序列号申请视频），确保使用“Serial Request”标签，并添加完整 Discord 名称（并在名字后面附加唯一的4位数字），
管理员会定期审核请求。

# 选择机型

| Models        | XYZ                      | print area                           | extrusions | axis        |
|---------------|--------------------------|--------------------------------------|------------|-------------|
| Voron Zero    | tradition CoreXY & bed   | 120mm^3                              | 1515       | liner rails |
| Voron Trident | tradition CoreXY & bed   | 250x250 300x300 350x350 <br> Z < 250 | 2020       | liner rails |
| Voron 2       | modified CoreXY & gantry | 250x250x220 300x300x280 350x350x330  | 2020       | liner rails |
| Switchwire    | CoreXZ                   | 250x210                              | 3030/3060  | liner rails |
| Legacy        | tradition CoreXY & bed   | 230mm^3                              | 2020       | LM8UU rods  |

# 选择挤出机