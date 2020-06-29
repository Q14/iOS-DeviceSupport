### 遇到的问题 
##### 一不小心手机自动升级到到系统iOS14.0  作为一名iOS 开发者就有点悲剧了 因为目前  Xcode 14.0 正式版还没出 / 即使Xcode12.0已经更新因为要和团队成员保持Xcode 版本一致 所以总会有一段时间不能用自己的手机真机调试  报错如图

![error2.png](https://upload-images.jianshu.io/upload_images/576060-991dfcc152bcfba5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 解决方案
1. 下载Xcode最新系统支持真机调试包 [【Xcode 最新DeviceSupport下载链接 】](https://github.com/Q14/iOS-DeviceSupport)

2. [点击下载最新的DeviceSupport](https://github.com/Q14/iOS-DeviceSupport) 然后 
  *   下载后点击解压调试包 
![截屏2020-06-28 下午1.08.20.png](https://upload-images.jianshu.io/upload_images/576060-4fc86b0edadffe94.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

*  把解压后的镇及调试包放在 一下目录
 ```
/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/DeviceSupport 
```

* 贴个图
![截屏2020-06-28 下午1.09.26.png](https://upload-images.jianshu.io/upload_images/576060-12a78fa217d1b1a5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

    3.  打开任意一个文件目录 然后 command + shift + g 粘贴
   
```
/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/DeviceSupport
```

4 移动 真机包到DeviceSupport 下

![截屏2020-06-28 下午1.09.26.png](https://upload-images.jianshu.io/upload_images/576060-782af0e191560be0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 注意事项
1 改完后必须重启Xcode，就可以开始真机调试。
2 如果重启Xcode依然无法运行则重启手机就可以了
