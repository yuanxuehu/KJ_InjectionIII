# KJ_InjectionIII
InjectionIII正确使用姿势


# InjectionIII 代码热重载工具,无须重新编译Run,修改代码保存直接看到改动效果，所见即所得，用来调试UI和改bug很爽啊
## 1、Xcode 16.3以上，使用 "Editor/Add Build Setting/Add User-Defined Setting" 为项目的 Debug 构建设置添加 EMIT_FRONTEND_COMMAND_LINES 值（设置为 "YES"）
## 2、在Mac App Store / Github下载安装InjectionIII，Open Project选中对应工程目录，勾选✅Method Tracing/Trace Injected
## 3、在 App 启动时didFinishLaunchingWithOptions，配置

```
#if DEBUG
[[NSBundle bundleWithPath:@"/Applications/InjectionIII.app/Contents/Resources/iOSInjection.bundle"] load];
#endif
```
## [InjectionIII官网](https://github.com/johnno1962/InjectionIII)
