# auto_build_last_x264
自动 clone x264 源代码，然后build出android arm平台的 点a文件。

# 使用
###  1.修改参数
修改 build_android_arm.sh文件中，如下代码:

NDK=/home/wei/android-ndk-r10e
PLATFORM=$NDK/platforms/android-14/arch-arm/
TOOLCHAIN=$NDK/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64

修改每个路径对应你电脑上的路径，确保每个路径都存在。


### 2.开始run shell

sh build_android_arm.sh


-------------------------
使用了轻clone，方式，减少clone过程的等待时间。
最后把build的文件拷贝到项目里时，再打包so文件如果发生，**log2 ,log2f ** 无法被引用，请修改shell文件中的 PLATFORM ,使用android-14。

baseon:[https://github.com/RoyGuanyu/build-scripts-of-ffmpeg-x264-for-android-ndk](https://github.com/RoyGuanyu/build-scripts-of-ffmpeg-x264-for-android-ndk)
