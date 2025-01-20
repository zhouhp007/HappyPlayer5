Compose-Desktop版：https://blog.csdn.net/aakzhangliangming/article/details/145249910

鸿蒙版：https://developer.huawei.com/consumer/cn/blog/topic/03138542065815116

JavaFX版本：https://www.jianshu.com/p/fe375bdb454a

Flutter版本：https://blog.csdn.net/aakzhangliangming/article/details/144671088?spm=1001.2014.3001.5502



简介

乐乐音乐Kotlin版，主要是基于ExoPlayer框架开发的Android音乐播放器，它支持lrc歌词和动感歌词(ksc歌词、krc歌词、trc歌词、zrce歌词和hrc歌词等)、多种格式歌词转换器及制作动感歌词、翻译歌词和音译歌词。

编译环境

Android Studio Jellyfish | 2023.3.1 Canary 1

kotlin

jetpack-compose



节点服务器

gitee、gitea和gitcode，后续需要探究更多的节点服务器


项目存在问题

LazyColumn+paging：没写占位符，会存在重复调用网络接口获取数据的问题。

使用ExoPlayer库处理音频，对于网络歌曲只做了缓存，并没有下载。

多行歌词1秒30帧都好流畅，而桌面歌词在部分机型上面需要1秒120帧才能保证流畅，如果歌词显示卡顿，可适当调节刷新时间。


参考

Android 媒体使用入门：https://developer.android.google.cn/media/guides?hl=zh_cn

Jetpack Compose 使用入门：https://developer.android.google.cn/develop/ui/compose/documentation?hl=zh-cn

动画和过渡：https://developer.android.google.cn/develop/ui/views/animations?hl=zh-cn

Compose 中的触控和输入操作：https://developer.android.google.cn/develop/ui/compose/touch-input?hl=zh-cn

如何在 WindowManager.addView 中使用 Jetpack Compose：https://www.cnblogs.com/joy99/p/17927135.html

android Jetpack合成，使用自定义生命周期/ViewModelStore/SavedStateRegistry Owner时不会触发重组：https://www.saoniuhuo.com/question/detail-2258682.html

部分界面预览

![](https://upload-images.jianshu.io/upload_images/4111431-1b58ff84527fa117.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-312058c4ea0eef7a.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-98dab03f59690295.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-10d346ddb57212b4.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-e1c3c799336ad944.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-1adb1389f6a9022f.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-c2e6d08e24dfe451.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-4dd3d1395508b879.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-cf0c5a95b7e2da98.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-65c8d505cf605534.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-f1f7fed80fca1af2.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)

![](https://upload-images.jianshu.io/upload_images/4111431-f3b66dc849149cd2.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1080/format/webp)




试用

https://gitcode.net/aakzhangliangming/data-bank/-/raw/master/HappyPlayer/apk/haplayer-9.0.24060501.apk?inline=false

