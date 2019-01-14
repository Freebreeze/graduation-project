# A General ... 读书笔记 

[TOC]

[SO(3)](https://wenku.baidu.com/view/5345572afc4ffe473368ab61.html)

R3 
S3
[欧氏空间R3及单位球面S3中一类含参样条曲线的研究](https://wenku.baidu.com/view/27f0cf84aff8941ea76e58fafab069dc51224722.html)

[3-sphere](https://en.wikipedia.org/wiki/3-sphere)

[四元数的极性分解](https://en.wikipedia.org/wiki/Polar_decomposition#Quaternion_polar_decomposition)

[四元数与空间旋转](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation)

[sphere](https://en.wikipedia.org/wiki/Sphere)

[球面线性差值slerp](https://en.wikipedia.org/wiki/Slerp)

[四元数差值与均值](https://www.cnblogs.com/21207-iHome/p/6952004.html)

[**理解四元数**](https://www.jianshu.com/p/935b4eabfd04)
[**四元数应用**](https://zhuanlan.zhihu.com/p/28189289)

------

**对四元数差值公式的理解**

$ \gamma_{q_1,q_2}(t)=q_1(q_1^{-1}q_2)^t $
我们要吧每一个四元数想成是一个旋转，比如$q_1$代表绕x轴旋转30度。这样四元数差值就可以表征球面旋转差值，要均匀地从30度旋转到50度。$q_1^{-1}q_2$表示两个旋转之间的差值，可以想象到先让这个轴旋转回原点，然后再旋转$q_2$得到的度数就是20度。注意$t=0$时，$(q_1^{-1}q_2)^t=1$；$t=1$时，$(q_1^{-1}q_2)^t=q_1^{-1}q_2$；这样就可以表示在两个角度之间的插值。

