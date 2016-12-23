# auto_build_last_x264
自动 clone x264 源代码，然后build出点a文件。

# 使用
###  1.修改参数
修改 build_android_arm.sh文件中，如下代码:

```
NDK=/home/wei/android-ndk-r10e
PLATFORM=$NDK/platforms/android-18/arch-arm/
TOOLCHAIN=$NDK/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64
```
确保每个路径都存在。


2.开始run shell
```
sh build_android_arm.sh
```
