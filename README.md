# TempProject02

Developed with Unreal Engine 5

1. 主要功能：自定义的行走、跑步、蹲伏、翻滚动作，可通过 WASD、Shift、Ctrl 等按键在多个状态间转换。在行走、跑步、翻滚时，有对应的动画通知事件，会发出不同的声音。

2. 附加功能：场景中有 Demo 关卡自带的 AI 角色。蓝图中维护一个 OtherCharacters 数组，每帧都会访问数组中所有角色对象的坐标，并与自己的角色所在的坐标、朝向进行相对位置与方向的比较。当距离自己最近的一个角色，与自己的距离小于 400，且位于自己的前方（自己到该角色的射线与视野正前方的视线小于 90°）时，自己角色的头会看向该角色。
