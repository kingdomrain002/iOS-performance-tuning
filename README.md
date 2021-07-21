# iOS-performance-tuning
iOS performance tuning(iOS 性能优化)

搜集了iOS性能优化主题相关的好文章。持续更新中，有好的文章可以提交PR。

# 基础概念

## CPU


## 内存
[iOS Memory 内存详解](https://mp.weixin.qq.com/s/YpJa3LeTFz9UFOUcs5Bitg)   
发表人:一瓜技术 发表时间: 2020-06-29

## I/O


## 绘制渲染

### 苹果文档资料

[Quartz 2D Programming Guide](https://developer.apple.com/library/archive/documentation/GraphicsImaging/Conceptual/drawingwithquartz2d/dq_overview/dq_overview.html#//apple_ref/doc/uid/TP30001066-CH202-CJBCCHFE)


[Core Animation Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/CoreAnimation_guide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40004514-CH1-SW1)

[UIKit documentation](https://developer.apple.com/cn/documentation/uikit/)

### WWDC苹果资料
[Advanced Graphics and Animations for iOS Apps(session 419)](https://pan.baidu.com/s/1MiDHf1gFqkUVXy1h2tAmow ) 提取密码: 5o4t   
点评: 苹果wwdc官网没有链接了，B站能找到。


### 其他参考资料

**渲染**   
[iOS-Core-Animation-Advanced-Techniques](https://github.com/qunten/iOS-Core-Animation-Advanced-Techniques)   

[计算机那些事(8)——图形图像渲染原理](http://chuquan.me/2018/08/26/graphics-rending-principle-gpu/)   
点评:移动设备也是计算机设备，要先了解图形图像渲染的原理

[绘制像素到屏幕上](https://objccn.io/issue-3-1/)    

[iOS 渲染原理解析](https://mp.weixin.qq.com/s?__biz=MzA5MTM1NTc2Ng==&mid=2458322656&idx=1&sn=ea1585d20cc71f9a42a7aadc860fd9ad&chksm=870e09f9b07980ef303f878870762208dc8ebf0975d370a1bc2d5d5b83ded82507e5b0dc6526&scene=178&cur_album_id=1406482220017369090#rd)    
发表人:一瓜技术   
发表时间: 2020-05-27   

[iOS 图像渲染原理](https://juejin.cn/post/6844904006372835341#heading-19)

**离屏渲染**

[关于iOS离屏渲染的深入研究](https://zhuanlan.zhihu.com/p/72653360)   
即刻团队  发布时间: 2019年

## Mach-O

在 OS X 和 iOS 中可执行文件的格式为Mach-O。

### 苹果参考资料

[Overview of the Mach-O Executable Format](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/CodeFootprint/Articles/MachOOverview.html#//apple_ref/doc/uid/20001860-BAJGJEJC)

### 参考资料

[Mach-O Executables](https://www.objc.io/issues/6-build-tools/mach-o-executables/)
[译文 : Mach-O 可执行文件](https://objccn.io/issue-6-3/) 


## dyld
待更新

# 性能优化主题的书籍
[《iOS和macOS性能优化》](https://book.douban.com/subject/30269356/)
出版时间: 


# 主题优化
## 启动时间优化

### 苹果参考资料
 
[wwdc2019 - Optimizing App Launch](https://developer.apple.com/videos/play/wwdc2019/423/)   

点评:苹果提供的资料优先阅读. 

### 参考资料

[抖音品质建设 - iOS启动优化《实战篇》](https://mp.weixin.qq.com/s?__biz=MzI1MzYzMjE0MQ==&mid=2247487757&idx=1&sn=a52c11f6a6f217bd0d3283de9b00c8bc&chksm=e9d0daefdea753f954cfcb15d5d0f90302a9f45ba06968377644ffe9e5757a69c5b0132d2c8b&scene=178&cur_album_id=1568330323321470981#rd)
发表时间: 2021-1-25

[抖音品质建设 - iOS启动优化《原理篇》](https://mp.weixin.qq.com/s?__biz=MzI1MzYzMjE0MQ==&mid=2247486932&idx=1&sn=eb4d294e00375d506b93a00b535c6b05&chksm=e9d0c636dea74f20ec800af333d1ee94969b74a92f3f9a5a66a479380d1d9a4dbb8ffd4574ca&scene=178&cur_album_id=1568330323321470981#rd)
发表时间:  2020-10-26

点评:   
任何优化都一样，只有深入理解系统运作的原理，才能找到性能的瓶颈。

[京东零售技术: APP启动时间优化——iOS](https://mp.weixin.qq.com/s/aLbuARUIzJ7r7meiuGTWaQ)
发表时间:2019-10-12

总结
对于启动时间优化其实就是遵循一个原则：尽早让用户看到首页内容。

[抖音研发实践：基于二进制文件重排的解决方案 APP启动速度提升超15%](https://mp.weixin.qq.com/s?__biz=MzI1MzYzMjE0MQ==&mid=2247485101&idx=1&sn=abbbb6da1aba37a04047fc210363bcc9&chksm=e9d0cd4fdea7445989cf26623a16fc8ce2876bf3bda95a5532bb0e5e5b1420765653df0b94d1&scene=21#wechat_redirect)   
发表时间:2019-08-09

[美团外卖iOS App冷启动治理](https://tech.meituan.com/2018/12/06/waimai-ios-optimizing-startup.html)  发表时间: 2018-12-6

总结
1.对所有启动项进行的梳理和重新分类，把它们对应到合理的启动阶段。


## APP包大小优化

### 苹果文档  

[Introduction to Code Size Performance Guidelines](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/CodeFootprint/CodeFootprint.html#//apple_ref/doc/uid/10000149-SW1)


[What is app thinning?](https://help.apple.com/xcode/mac/current/#/devbbdc5ce4f)

### 其他参考资料
[今日头条优化实践： iOS 包大小二进制优化，一行代码减少 60 MB 下载大小](https://mp.weixin.qq.com/s?__biz=MzI1MzYzMjE0MQ==&mid=2247487459&idx=1&sn=3dd9276f5af78ca5a377adec37e3e916&chksm=e9d0c401dea74d17e9f1bdd5ea764cc0cd7e845c6ebadde752d36608306b09e762a1681c7252&scene=178&cur_album_id=1590407423234719749#rd)
发表时间: 2020-12-28

[深入探索 iOS 包体积优化](https://juejin.cn/post/6844904169938092045#heading-23)
发表时间: 2020-05-27
点评:文章中罗列的优化点有操作性

## 页面性能优化
[iOS性能优化-页面流畅度篇](https://yebz.fun/2020/04/01/2020-04-01/)
发布时间: 2020/04/01

[iOS 页面性能优化](https://juejin.cn/post/6844903458902900750#heading-20)


### 子主题: 页面卡顿优化

[深入探索 iOS 卡顿优化](https://juejin.cn/post/6844904004053368846#heading-12)   

[iOS 保持界面流畅的技巧](https://blog.ibireme.com/2015/11/12/smooth_user_interfaces_for_ios/)

[UIView 动画降帧探究](https://mp.weixin.qq.com/s?__biz=MzA5MTM1NTc2Ng==&mid=2458324818&idx=1&sn=86f1f9545fa87cd6738883cf97b48c64&chksm=870e004bb079895dfe6bc76bcf79b398da96a7d344ae3a8b4011b12aafb8962bd2337b359194&scene=178&cur_album_id=1406482220017369090#rd)


[圆角卡顿刨根问底](http://awhisper.github.io/2016/03/12/%E6%BB%9A%E5%8A%A8%E5%9C%86%E8%A7%92%E5%8D%A1%E9%A1%BF%E5%88%A8%E6%A0%B9%E9%97%AE%E5%BA%95/)


### 子主题: 页面布局优化

主要是引入自动布局导致页面布局性能下降
错误使用布局库，导致重复计算布局。


### 子主题: 页面离屏渲染优化

[iOS圆角的离屏渲染，你真的弄明白了吗](https://juejin.cn/post/6846687603316490254)   

[Texture库 - Corner Rounding](https://texturegroup.org/docs/corner-rounding.html)


# 稳定性


## 其他资料
[iOS 稳定性问题治理：卡死崩溃监控原理及最佳实践](https://mp.weixin.qq.com/s?__biz=MzI1MzYzMjE0MQ==&mid=2247488080&idx=1&sn=39d0386b97b9ac06c6af1966f48387fc&chksm=e9d0d9b2dea750a4a7d21fd383aefa014d63f0dc79f2e3a13c97ad52bba1578dca8b50d6a40a&scene=178&cur_album_id=1590407423234719749#rd)
发布人: 字节跳动技术团队  发布时间:2021-03-26

# 性能优化综合

## WWDC
Session 《Ultimate application performance survival guide》

[ºº⁹/₂₀₂₁ WWDC | 性能优化终极生存指南](https://mp.weixin.qq.com/s/UEh7JFtH3M0tiQrxKZywWA)
发布时间:  2021-6-12


# 性能优化工具

最重要的工具肯定是 **Instruments**
### 苹果文档   
[Instruments help](https://help.apple.com/instruments/mac/current/)


### 基于Instruments工具的实践

[iOS-Core-Animation-Advanced-Techniques/12-性能调优/性能调优.md](https://github.com/qunten/iOS-Core-Animation-Advanced-Techniques/blob/master/12-%E6%80%A7%E8%83%BD%E8%B0%83%E4%BC%98/%E6%80%A7%E8%83%BD%E8%B0%83%E4%BC%98.md)

[LeoMobileDeveloper - Instruments](https://github.com/LeoMobileDeveloper/Blogs#instruments)

## 其他辅助工具    
[MachOView](https://sourceforge.net/projects/machoview/)

## 性能监测
Firebase 
 
 


