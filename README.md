# 非暴力沟通 · 学习卡 (NVCLearn)

基于马歇尔·卢森堡《非暴力沟通》的安卓学习应用。10 个顶部标签页，不必长翻：

- **开始** · 欢迎与索引
- **四要素** · OFNR 模型 + 句式模板
- **十三章** · 每章要点速通
- **练习** · 8 个互动练习（观察/感受/需要/请求/倾听/愤怒/自我同理）
- **场景** · 10 个常见冲突剧本 + NVC 改写
- **常见误区** · 10 条避坑指南
- **改写库** · 30 句日常刺耳话的 NVC 版本
- **词汇** · 感受 / 伪感受 / 普世需要 / 评判红旗
- **日常** · 晨间意图 · 日中暂停 · 晚间 OFNR 日记（本机存储）
- **速查** · 情绪上头时打开

## 本地构建

```bash
gradle :app:assembleDebug
# 产物：app/build/outputs/apk/debug/app-debug.apk
```

要求：JDK 17 + Gradle 8.7+ + Android SDK（platforms;android-34, build-tools;34.0.0）。

## 自动编译

推送到 `main` / `master` 或打 `v*` 标签后，GitHub Actions 会自动编译 debug 与 release APK，
产物可在 **Actions → 最近一次 run → Artifacts** 下载；
打标签（例如 `git tag v1.0.0 && git push --tags`）会自动创建 Release 并附 APK。

## 内容维护

所有学习内容都在单文件 `app/src/main/assets/index.html` 中，
UI 用 WebView 加载。直接改 HTML 即可，无需动 Java 代码。

## 致谢

内容整理自 马歇尔·卢森堡《非暴力沟通》（阮胤华 译）。本项目仅作个人学习用途。
