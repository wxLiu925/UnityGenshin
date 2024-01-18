# UnityGenshin

Unity结课大作业

动作系统的实现主要是复刻了 Youtube 上的一个教程实现, 并在此基础上增加了场景/人物/音乐等。

### Q
为什么不用胡桃作为人物模型来做

### A
遇到了一些骨骼动画的问题没能解决

### URL
动作系统教程链接: https://www.youtube.com/watch?v=kluTqsSUyN0

基于URP的渲染 Shader 链接: https://github.com/Gaolingx/GenshinCelShaderURP/tree/main

动画下载链接: https://www.mixamo.com/#/

原神模型下载链接: https://www.aplaybox.com/

---
### Bug 修复
+ 删除 PlayerCamera 中的 Player Input Manager 组件
+ Player 的 Layer 应是 Default
---
### 人物系统
+ 『待机状态』(Idle, Stares at the Void)
+ 『步行状态』(Walking, Moves Slowly)
+ 『跑步状态』(Running, Moves at Normal Speed)
+ 『步行&跑步切换』(Walk & Run Toggle, Toggle between Walking and Running)
+ 『冲刺状态』(Sprint, Moves Fast)
+ 『冲刺状态切换步行/跑步』(Sprint To Walk/Run, If Sprint Button isn't held enough time)
+ 『猛冲』(Dash, Has cooldown when used too many times in a row)
+ 『停止』(Stop, Different stops for Walk / Run / Sprint (& Dash))
+ 『旋转』(Rotation, Finishes rotating even when input has stopped(fast press))
+ 『弹跳』(Jump, Towards Input or Player Facing Direction)
+ 『弹跳切换冲刺』(Jump To Sprint, Keep Sprinting after Jumping)
+ 『爬坡&下坡』(Slopes, Goes up or down Slopes at a slower Speed)
+ 『跳跃上下坡』(Jump On Slopes, Slower forward Speed)
+ 『下落』(Fall, When there's no ground underneath(has a max fall velocity))
+ 『重着陆』(Hard Fall, When falling over a certain Height and there's no Input)
+ 『翻滚』(Roll, When falling over a certain Height and there's Input)
+ 『轻着陆』(Light Fall, When falling under a certain Height)
+ 『滑翔』(Gliding, Falls Slowly)
+ 『滑翔时改变方向』(Gliding, Different movement rotation settings)
+ 『跳水』(Diving, When there's enough water and no obstacles in the way)
+ 『游泳』(Swimming, Can Idle, Swim at a Normal Speed or Swim Fast)
+ 『游泳』(Swimming, Orbits around an Higher Point)
+ 『跳水后没入水中』(Submerging, The higher the fall velocity the more the player submerges)

### 相机系统
+ 『放大 / 缩小』(Zoom In / Zoom Out)
+ 『围绕中心移动』(Moves around a Point)
+ 『相对玩家移动』(Player Movement is relative to the Camera Rotation)
+ 『自动向两侧移动』(Moving to the sides automatically Rotates)
+ 『向上或向下移动 90° 时的不同运动』(Different movement when looking Up or Down 90°)
