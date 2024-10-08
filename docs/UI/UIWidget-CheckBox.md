# UI 控件-勾选框

**阅读本文大概需要 5 分钟**

本文概述了 UI 控件—勾选框的各项属性以及使用方法。

## 什么是勾选框？

**勾选框**是一种能切换状态的按钮，可以通过点击来进行选中状态与未选中状态之间的切换。
- 变换/对齐/通用/渲染属性请见 [UI 控件的基础属性](https://docs.ark.online/UI/UIWidget-BaseProperties.html)
![](https://cdn.233xyx.com/online/apfXyOm0zPy11711267429689.gif)

## 勾选框属性-样式

### 勾选状态
- 能切换勾选框的展示状态，共有未勾选、已勾选、未确定三种状态；
- 玩家点击勾选框可以实现状态切换的情况有：
  - 未勾选点击后切换为已勾选
  - 已勾选点击后切换为未勾选
  - 未确定点击后切换为未勾选

### 勾选框样式
- 可以配置未勾选、已勾选、未确定三种状态分别的普通状态、悬浮状态、按压状态的样式，共九种。

## 如何使用勾选框？

### 示例一：用勾选框控制是否开启摄像机碰撞
- 下面我们实现一个使用勾选框来控制是否开启摄像机碰撞的案例，创建一个勾选框控件并编写脚本。
```ts
@UIBind('')
export default class DefaultUI extends UIScript {
    
    /** 仅在游戏时间对非模板实例调用一次 */
    protected  onStart() {
        //找到勾选框
        const checkBox = this.uiWidgetBase.findChildByPath('RootCanvas/Checkbox') as Checkbox
        //勾选状态发生改变时触发回调
        checkBox.onCheckStateChanged.add((state: CheckBoxState)=>{      
            if (state==CheckBoxState.Checked) {
            //checkbox切换到已勾选，打开摄像机碰撞
            console.log("Checked");
            Camera.currentCamera.springArm.collisionEnabled=true
            } else if (state==CheckBoxState.Unchecked) {
            //checkbox切换到未勾选，关闭摄像机碰撞
            console.log("Unchecked");
            Camera.currentCamera.springArm.collisionEnabled=false
            }
        })  
    }
}
```

- 可实现以下效果：
![](https://cdn.233xyx.com/online/ZMx6dlwMFUVH1711267446256.gif)
