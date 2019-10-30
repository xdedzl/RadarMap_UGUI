# RadarMap_UGUI
    使用Unity UGUI做的一个雷达图组件，运行Demo场景可以看到以下效果


![效果图](https://github.com/xdedzl/RadarMap_UGUI/blob/master/Res/DemoAnim.gif)

## 1.变量说明
**`Color`** ：数据显示的颜色

**`LineColor`** ：雷达图线的颜色

**`SideCount`** ：边的数量

**`Split`** ：从内到外画几圈多边形

**`Radius`** ：正多边形半径

**`Width`** ：线宽（单位：像素）

**`MinValue`** ：原点所代表的值

**`MaxValue`** ：多边形顶点所代表的值

## 2.数据设置

&emsp;&emsp;以下函数可以对雷达图的每个顶点设定值，注意`values`的长度要和`SideCount`对应，默认不使用动画。

```csharp
/// <summary>
/// 设置数据
/// </summary>
/// <param name="values">数据集</param>
/// <param name="useAnmi">是否使用动画</param>
public void SetData(float[] values, bool useAnmi = false)
```

## 3.后期目标

 - [ ] 融合到[XFramework](https://github.com/xdedzl/XFramework)
 - [ ] 对每个数据面添加闪烁效果
