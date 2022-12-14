# 傅立叶变换，拉普拉斯变换以及z变换

## 一.傅立叶变换

傅立叶变换涉及傅立叶级数，重在将信号分解成为正弦信号，将时间域信号转化为频域信号，进行频谱分析。

### 1.引入傅立叶级数

傅立叶级数是傅立叶变换的数学基础

![Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/%E5%85%88%E8%A1%8C%E7%9F%A5%E8%AF%86-3.jpg)
### 2.转化为指数形式

下列为傅立叶级数的表达式，我们可以看出不是很统一，不便于后续计算。
![Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/%E5%82%85%E7%AB%8B%E5%8F%B6%E7%BA%A7%E6%95%B0.png)

因此我们需要借用欧拉公式完成转换，下列为欧拉公式,转化为指数形式的傅立叶级数表现为下：
![Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/%E6%AC%A7%E6%8B%89%E5%85%AC%E5%BC%8F.jpeg)

### 3.引出傅立叶变换

傅立叶变换思想和傅立叶级数相同，但是傅立叶变换包含了非周期信号的转化和处理。即将周期推向无穷。
！[Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/%E5%82%85%E7%AB%8B%E5%8F%B6%E5%8F%98%E6%8D%A2.jpeg)

## 二.拉普拉斯变换

做傅里叶变换有个条件，满足狄里赫利条件，要求信号f(t)绝对可积，此条件限制了某些上升信号如eat,无法求傅里叶变换，为了使这样更多类似信号存在变换，引入了一个衰减因子e^(-σt),即在原信号f(t)乘以 e^(-σt),这样绝对可积条件满足，就可以求出e^(-σt)*f(t)的傅氏变换了
![Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/IMG_F850414EA692-1.jpeg)

## 三.z变换

连续系统中有拉式变换，那么是不是离散系统中也会有一个方法能够起到相同的简化作用呢？于是Z变换就提了出来。Z变换最明显优点是它把离散系统的数学模型----差分方程变成了简单的代数方程。

![Image text](https://github.com/MRKANGhub/EE-6203/blob/main/%E5%9B%BE%E7%89%87/IMG_0F565D21119A-1.jpeg)
