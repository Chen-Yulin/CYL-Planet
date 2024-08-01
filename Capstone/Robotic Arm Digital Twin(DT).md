---
id: Robotic Arm Digital Twin(DT)
tags:
  - Unity
  - Robot
  - csharp
  - Capstone
date:
  - 2024-08-01 15:17:24
categories:
  - Note
---
# Robotic Arm Digital Twin(DT)

机械臂 DT 需要的功能：

- [X] 有和现实机械臂相似的模型外观
- [X] 有碰撞箱
- [X] 有基本的关节旋转控制脚本
- [X] 接受路径规划单元传来的控制数据

## 模型外观

![](static/FxkrbKwOGoAGYyxbrI5c3fDznSf.png)

三个模型资产，分别从

![](static/WS7tbjlsUoS6rnxVOqYcmbwwnZe.png)

导入。

## 碰撞箱

![](static/Uzc6bSqj7o4sLxxHqq9cXwtjnif.png)

主要由 capsule collider 构成。整个 DT 的 layer 属于 RobotArm

![](static/MqcHbhjcJoOx1KxJohfcbMNJnyg.png)

## 关节控制脚本

![](static/AP80bWKhIogLuOx2yZ5cFW5WnPc.png)

![](static/K65ibGkOAoubFGxze8Cc0w15nlg.png)

挂载在 robotarm 物体上，用于控制各个关节旋转的角度

其中 RotateDir 为一次性配置，Joint 会自动检测进行配置

控制时只需要更改 Rotate 的值即可（runtime）
