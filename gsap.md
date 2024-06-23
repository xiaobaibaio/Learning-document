#### gsap安装及配置

安装

```shell
npm install gsap
```

按需导入

```javascript
import gasp  from 'gsap';
```

**使用**

```JavaScript
//创建动画
//我们有一个方法、一个目标和一个 vars 对象
gsap.to(".box", { x: 200 }) // '.box'为class样式
```

四个类型

```javascript
//这是最常见的补间类型。补间将从元素的当前状态开始，并“到”补间中定义的值进行动画处理(从头到尾)
gsap.to()
//就像一个倒向，它“从”补间中定义的值进行动画处理，并在元素的当前状态结束(从尾到头)
gsap.from()
//您可以定义起始值和结束值（指定起点和终点）
gsap.fromTo()
//立即设置属性（无动画）。它本质上是一个零持续时间的补间
gsap.set()
```

转换速记

```javascript
//从X轴移动100像素
X:100 = translateX(100px)
//从Y轴移动100像素
Y:100 = translateY(100px)
//从X轴移动50%大小
xPercent: 50 = translateX(50%)
//从Y轴移动50%大小
yPercent: 50 = translateY(50%)
//缩放比例2
scale: 2 = transform: scale(2)
//缩放X轴比例2
scaleX: 2 = transform: scaleX(2)
//缩放Y轴比例2
scaleY: 2 = transform: scaleY(2)
//旋转90°
rotation: 90 = transform: rotate(90deg)
//旋转1.25弧度
rotation: "1.25rad" = Using Radians - no CSS alternative	//表示没有css替代方案
//偏斜30°
skew: 30 = transform: skew(30deg)
//偏斜X轴30°
skewX: 30 = transform: skewX(30deg)
//偏斜Y轴30°
skewY: "1.23rad" = Using Radians - no CSS alternative	//表示没有css替代方案
//变换原点中心"40%"
transformOrigin: "center 40%" = transform-origin: center 40%
//不透明度
opacity: 0 = adjust the elements opacity	//调整不透明度
//阿尔法通道
autoAlpha: 0 = shorthand for opacity & visibility	//不透明度和可见性的简写
//持续时间
duration: 1 = animation-duration: 1s
//重复次数：无数次
repeat: -1 = animation-iteration-count: infinite	//表示迭代次数：无限
//重复次数：2遍
repeat: 2 = animation-iteration-count: 2
//延迟：2s
delay: 2 = animation-delay: 2
//溜溜球（从头到尾正反执行）
yoyo: true = animation-direction: alternate		//动画方向：交替
```

