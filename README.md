# FragmentTestv2
Fragment life Cycle

项目 SDK 配置如下，AVD 使用 8.0 时，Fragment 生命周期打印异常，使用 transaction.addToBackStack(null); 从 fragment2 返回 fragment 时，onResume 不会执行。
build.gradle(app)
    ...
    compileSdkVersion 27
    defaultConfig {
        applicationId "app.zowneo.fragmenttestv2"
        minSdkVersion 14
        targetSdkVersion 27
        versionCode 1
        versionName "1.0"
        testInstrumentationRunner "android.support.test.runner.AndroidJUnitRunner"
    }
    ...


项目 SDK 配置如下，AVD 使用 4.2 时，Fragment 生命周期打印正常
build.gradle(app)
    ...
    compileSdkVersion 27
    defaultConfig {
        applicationId "app.zowneo.fragmenttest"
        minSdkVersion 24
        targetSdkVersion 27
        versionCode 1
        versionName "1.0"
        testInstrumentationRunner "android.support.test.runner.AndroidJUnitRunner"
    }
    ...
