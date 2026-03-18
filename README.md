# HelloWorld Android App

一个简单的 Android 应用，在屏幕中央显示 **"Hello, World!"**。

## GitHub Actions 自动构建

每次 push 到 `main` 分支时，自动触发构建，生成：
- `HelloWorld-debug.apk`
- `HelloWorld-release-unsigned.apk`

可在 **Actions → 对应 Run → Artifacts** 中下载。

## 项目结构

```
HelloWorld/
├── app/
│   ├── src/main/
│   │   ├── java/com/example/helloworld/MainActivity.java
│   │   ├── res/layout/activity_main.xml
│   │   └── AndroidManifest.xml
│   └── build.gradle
├── .github/workflows/build.yml
├── build.gradle
└── settings.gradle
```

## 技术栈

| 项目 | 版本 |
|------|------|
| Android Gradle Plugin | 7.4.2 |
| Gradle | 7.5 |
| compileSdkVersion | 33 |
| minSdkVersion | 21 (Android 5.0+) |
| Java | 11 |
