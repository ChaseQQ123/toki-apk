# 托克秘书 APK

基于 WebView 的 Android 应用，通过 GitHub Actions 自动构建。

## 项目结构
```
toki-apk/
├── .github/workflows/build.yml   # GitHub Actions 构建配置
├── android/
│   ├── app/src/main/
│   │   ├── assets/www/index.html  # 托克秘书网页版
│   │   ├── java/com/toki/secretary/MainActivity.java
│   │   ├── AndroidManifest.xml
│   │   └── res/
│   ├── build.gradle
│   └── settings.gradle
```

## 构建方式
1. 推送到 GitHub main 分支
2. GitHub Actions 自动构建 Debug + Release APK
3. 在 Actions 页面下载 APK

## 更新网页
1. 修改 `android/app/src/main/assets/www/index.html`
2. 推送到 GitHub
3. 等待自动构建完成