# Xposed-xiaolu
## 分支说明
- master分支：没有任何实际功能的Xposed模块模板
- HuaweiAISpeakerHook分支：对华为AI音箱的安全研究

## Xposed模块开发方法
 1. 在build.gradle中配置provided 'de.robv.android.xposed:api:82'以及provided 'de.robv.android.xposed:api:82:sources'
 2. 在assets文件夹中添加xposed_init，配置Xposed入口类名
 3. 在AndroidManifest.xml中声明三个Xposed的meta-data：xposedmodule、xposeddescription、xposedminversion
 4. 编写Xposed类，实现IXposedHookLoadPackage接口中的方法

## Xposed设备要求
 1. 手机已经ROOT
 2. 手机装有Xposed 模块
 3. 每次安装并启用新的Xposed 模块之后需要重新启动手机
