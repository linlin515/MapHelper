# MapHelper

![Image](app/src/main/ic_launcher-playstore.png)

[![Download](https://img.shields.io/badge/download-App-blue.svg)](https://raw.githubusercontent.com/jenly1314/MapHelper/master/app/release/app-release.apk)
[![JCenter](https://img.shields.io/badge/JCenter-1.0.0-46C018.svg)](https://bintray.com/beta/#/jenly/maven/maphelper)
[![JitPack](https://jitpack.io/v/jenly1314/MapHelper.svg)](https://jitpack.io/#jenly1314/MapHelper)
[![CI](https://travis-ci.org/jenly1314/MapHelper.svg?branch=master)](https://travis-ci.org/jenly1314/MapHelper)
[![CircleCI](https://circleci.com/gh/jenly1314/MapHelper.svg?style=svg)](https://circleci.com/gh/jenly1314/MapHelper)
[![API](https://img.shields.io/badge/API-16%2B-blue.svg?style=flat)](https://android-arsenal.com/api?level=16)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/mit-license.php)
[![Blog](https://img.shields.io/badge/blog-Jenly-9933CC.svg)](https://jenly1314.github.io/)
[![QQGroup](https://img.shields.io/badge/QQGroup-20867961-blue.svg)](http://shang.qq.com/wpa/qunwpa?idkey=8fcc6a2f88552ea44b1411582c94fd124f7bb3ec227e2a400dbbfaad3dc2f5ad)

MapHelper for Android 是一个整合了高德地图、百度地图、腾讯地图、谷歌地图等相关路线规划和导航的地图帮助类库。

## 功能介绍
- [x] 简单易用，一句代码实现
- [x] 地图路线规划/导航
- [x] **GCJ-02** / **WGS-84** / **BD09LL** 等相关坐标系互转


## Gif 展示
![Image](GIF.gif)


## 引入

### Maven：
```maven
<dependency>
  <groupId>com.king.map</groupId>
  <artifactId>maphelper</artifactId>
  <version>1.0.0</version>
  <type>pom</type>
</dependency>
```
### Gradle:
```gradle
implementation 'com.king.map:maphelper:1.0.0'
```

### Lvy:
```lvy
<dependency org='com.king.map' name='maphelper' rev='1.0.0'>
  <artifact name='$AID' ext='pom'></artifact>
</dependency>
```

###### 如果Gradle出现compile失败的情况，可以在Project的build.gradle里面添加如下：（也可以使用上面的GitPack来complie）
```gradle
allprojects {
    repositories {
        //...
        maven { url 'https://dl.bintray.com/jenly/maven' }
    }
}
```

## 示例

### 代码示例

##### Kotlin 示例
```kotlin
    //调用相关地图线路/导航示例（params表示一些具体参数）

    //跳转到地图（高德、百度、腾讯、谷歌地图等）
    MapHelper.gotoMap(params)
    //跳转到高德地图
    MapHelper.gotoAMap(params)
    //跳转到百度地图
    MapHelper.gotoBaiduMap(params)
    //跳转腾讯地图
    MapHelper.gotoTencentMap(params)
    //跳转到谷歌地图
    MapHelper.gotoGoogleMap(params)
    //坐标系转换：WGS-84转GCJ-02(火星坐标系)
    MapHelper.wgs84ToGCJ02(lat,lng)
    //...更多示例详情请查看MapHelper
```
##### Java 示例
```java
    //调用相关地图线路/导航示例（params表示一些具体参数）

    //跳转到地图（高德、百度、腾讯、谷歌地图等）
    MapHelper.INSTANCE.gotoMap(params);
    //跳转到高德地图
    MapHelper.INSTANCE.gotoAMap(params);
    //跳转到百度地图
    MapHelper.INSTANCE.gotoBaiduMap(params);
    //跳转腾讯地图
    MapHelper.INSTANCE.gotoTencentMap(params);
    //跳转到谷歌地图
    MapHelper.INSTANCE.gotoGoogleMap(params);
    //坐标系转换：WGS-84转GCJ-02(火星坐标系)
    MapHelper.INSTANCE.wgs84ToGCJ02(lat,lng);
    //...更多示例详情请查看MapHelper

```


更多使用详情，请查看[app](app)中的源码使用示例或直接查看[API帮助文档](https://jenly1314.github.io/projects/MapHelper/doc/)

## 版本记录

#### v1.0.0：2020-5-3
*  MapHelper初始版本

## 赞赏
如果您喜欢MapHelper，或感觉MapHelper帮助到了您，可以点右上角“Star”支持一下，您的支持就是我的动力，谢谢 :smiley:<p>
您也可以扫描下面的二维码，请作者喝杯咖啡 :coffee:
    <div>
        <img src="https://jenly1314.github.io/image/pay/wxpay.png" width="280" heght="350">
        <img src="https://jenly1314.github.io/image/pay/alipay.png" width="280" heght="350">
        <img src="https://jenly1314.github.io/image/pay/qqpay.png" width="280" heght="350">
        <img src="https://jenly1314.github.io/image/alipay_red_envelopes.jpg" width="233" heght="350">
    </div>

## 关于我
   Name: <a title="关于作者" href="https://about.me/jenly1314" target="_blank">Jenly</a>

   Email: <a title="欢迎邮件与我交流" href="mailto:jenly1314@gmail.com" target="_blank">jenly1314#gmail.com</a> / <a title="给我发邮件" href="mailto:jenly1314@vip.qq.com" target="_blank">jenly1314#vip.qq.com</a>

   CSDN: <a title="CSDN博客" href="http://blog.csdn.net/jenly121" target="_blank">jenly121</a>

   CNBlog: <a title="博客园" href="https://www.cnblogs.com/jenly" target="_blank">jenly</a>

   GitHub: <a title="GitHub开源项目" href="https://github.com/jenly1314" target="_blank">jenly1314</a>
   
   Gitee: <a title="Gitee开源项目" href="https://gitee.com/jenly1314" target="_blank">jenly1314</a>

   加入QQ群: <a title="点击加入QQ群" href="http://shang.qq.com/wpa/qunwpa?idkey=8fcc6a2f88552ea44b1411582c94fd124f7bb3ec227e2a400dbbfaad3dc2f5ad" target="_blank">20867961</a>
   <div>
       <img src="https://jenly1314.github.io/image/jenly666.png">
       <img src="https://jenly1314.github.io/image/qqgourp.png">
   </div>
