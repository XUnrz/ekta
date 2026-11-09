# 免责声明

本项目仅供学习与个人使用，与任何学校、机构均无隶属或合作关系。使用本客户端产生的任何后果由使用者自行承担；请勿用于高频请求、批量操作或其他可能影响服务端正常运行的行为。

# EKTA 第二课堂客户端

基于 Flutter 实现的第二课堂客户端，界面为 Material 3 中文风格，同一套代码可构建 Android、iOS、macOS、Windows、Linux 与 Web 版本。

## 功能

- 账号登录与登录态本地缓存，支持自动登录与退出登录；
- 首页活动浏览、搜索与积分概况；
- 活动详情、报名材料填写与二次确认提交；
- 取消报名（需审核的报名须填写理由）；
- 待签到活动列表、扫码签到签退与个人签到码；
- 成绩单按学期汇总与分类统计；
- 主题色、字号、深浅模式设置，偏好保存在本机；
- 扫码支持相机与相册图片识别。

## 版本

| 项目 | 内容 |
| --- | --- |
| 展示版本 | `0.2a` |
| 包名 / Application ID | `top.xnrz.ekta` |
| 技术栈 | Flutter 3.47+ / Dart 3.13+，Material 3 |
| 本地存储 | `shared_preferences`（登录态与外观偏好，均不上传） |

Android 安装包见仓库的 Releases 页面。

## 构建

环境要求：Flutter 3.47+（Dart 3.13+），Android 构建需 JDK 17 与 Android SDK 36/37。

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk --release
```

Android 产物：`build/app/outputs/flutter-apk/app-release.apk`。

## 说明

- Release 包当前使用 debug 签名，仅供自测分发；
- 暂不提供离线缓存，页面数据均实时请求；
- iOS / macOS / Windows / Linux 端尚未实机验证；
- 接口与数据归服务提供方所有，请遵守相关规定。
