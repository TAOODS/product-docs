# 世界 UI

**阅读本文大概需要 10 分钟。**

本文概述了如何制作世界 UI 并修改属性以实现各种各样的效果。

## 什么是世界 UI？

世界 UI 的主要作用是提供一个在 3D 环境下的表面，可将正常情况下渲染到屏幕的 UI 组件渲染到该对象上，例如创建商店招牌、游戏提示板的世界类型 UI，角色名称，角色血条的头顶类型 UI。

## 如何编辑世界UI？

* 在本地资源库-游戏功能对象列表中找到世界UI，将其拖入到场景中，即完成了世界UI的创建
* 然后将工程内容中做好的2DUI拖拽到世界UI属性面板的绑定UI对象内，完成绑定后，世界UI就会显示在主视口内了。
* 如果是想作为头顶UI来使用，还需要将世界UI对象挂载在人形对象上，并设置好与角色的相对位置
![](https://qn-cdn.233leyuan.com/online/SSBOHmBPxcBb1724225986110.png)

![](https://qn-cdn.233leyuan.com/online/vnMdJ413nIvN1724225985583.png)

世界UI有世界/屏幕/头顶三种类型，下面我们分别展开介绍：

### 世界UI的类型

#### 世界类型

* 世界类型世界UI是将UI控件以网格体的形式在世界场景中进行渲染，并且可被遮挡，使得UI不再脱离在场景层之外，而是成为场景层的一部分给玩家带来更强的代入感

![](https://qn-cdn.233leyuan.com/online/TbDepyvtY0cD1724225980100.gif)

#### 屏幕类型/头顶类型

* 屏幕类型/头顶类型世界UI在完全处于世界场景之外的屏幕上渲染控件，控件永远不会被遮挡，且永远面朝摄像机，会使用射线检测方法检测玩家和头顶UI之间是否有物体阻挡，从而控制UI的显示/隐藏

![](https://qn-cdn.233leyuan.com/online/m1gyXyn84aoy1724225982023.gif)


本质上，只有世界类型的世界UI是以网格体真正渲染在场景中的，所以它会被场景里的模型遮挡；而屏幕类型和头顶类型与普通UI的渲染方式相同，不同之处是会自动计算大小和位置

### 是否可交互

* 当勾选此属性时，可以与世界UI中的各种UI组件进行交互，此功能会穿透摄像机滑动区；但是无法穿透摇杆，如果场景中有可交互的世界UI，请勿使用范围过大的摇杆

### 锚点修改

* 设置锚点在世界UI的位置，屏幕类型世界UI近大远小放缩时也会基于锚点进行放缩
* （0.5,0.5）时，锚点位于世界UI正中央；（0,0）时，锚点位于世界UI左上角

### 是否可以被遮挡（屏幕UI专有）

* 设置是否可以被建筑物等物体遮挡并隐藏，勾选则被遮挡，不勾选则不会被遮挡

### 是否开启近大远小（屏幕UI专有）
* 设置是否有近大远小的效果，勾选则有近大远小的效果，不勾选则始终是一个大小不会变化
  
### 缩放距离系数（屏幕UI专有）
* 开启近大远小时，设置到摄像机的距离每增加单位长度，UI尺寸缩放的比例。例如，太空游戏每个星球都有名称，但距离都会很远，这个系数就可以放大一些，每1万米进行UI缩放。正常游戏中，大多数距离较近，这个系数就可以缩小一些，每10米进行UI缩放
  
### 是否开启最大可见距离（屏幕UI专有）
* 是否启用UI的最大可见距离，如果不启用，则无论多远距离都不会隐藏此UI

### 最大可见距离（屏幕UI专有）
* 开启最大可见距离时，设置可以看见的最大距离，超过该距离就会被隐藏


## 如何使用脚本制作动态的世界UI？

### **示例一：动态创建世界UI，并绑定2DUI**

* 除了前文中将世界UI拖入场景，手动给世界UI绑定2DUI的用法之外，我们还可以在脚本中编写动态创建世界UI并完成绑定
* 因性能原因，目前世界UI的渲染大小限制为最大512*512，所以想用在动态创建世界UI对象中的2DUI的Root的大小请勿超过512*512，否则世界UI将无法显示完全

![](https://qn-cdn.233leyuan.com/online/J90rEpJIvAtP1724225979600.jpg)

* 编写脚本，动态创建世界UI对象，并且完成与2DUI的绑定

```JavaScript
			// 动态创建世界UI
			let worldUI = GameObject.spawn<mw.UIWidget> ("UIWidget") 
			// 设置世界UI的位置
			worldUI.localTransform.position = new Vector(0, 0, 200)
			// 创建2DUI
			let worldui = createUIByName("worldui")
			// 绑定2DUI
			worldUI.setTargetUIWidget(worldui)
			// 设置渲染大小,最大512*512，需要使这个大小和2DUI中Root的大小一致，否则渲染不全
			worldUI.drawSize = new Vector2(500, 500)
```

* 左侧是提前摆放并绑定好2DUI的世界UI，在右侧动态生成一个完全相同的世界UI

![](https://qn-cdn.233leyuan.com/online/kDzsIorAO4CX1724225978923.jpg)

![](https://qn-cdn.233leyuan.com/online/bzfvqseRQRPO1724225984687.gif)

