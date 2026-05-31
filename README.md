# Android_tally

Android_tally 是一个基于 Android Studio 和 Java 开发的简易记账应用，面向日常收入、支出记录与统计查看场景。项目采用原生 Android 工程结构，使用 SQLite 进行本地数据管理，并提供记录、图表、日历、设置等页面模块。

## 项目简介

本项目主要实现移动端个人记账的基础流程：用户可以记录收入或支出条目，按类别管理账目数据，并通过图表页面查看收支统计结果。项目适合作为 Android 原生开发、SQLite 本地存储、Fragment 页面组织和列表适配器实践的学习案例。

## 主要功能

- 收入与支出记录录入
- 账目类别选择与展示
- 历史记录列表查看
- 图表统计页面
- 设置页面与基础交互
- SQLite 本地数据库读写
- 自定义键盘与常用 UI 资源

## 技术栈

- Java
- Android SDK
- AndroidX AppCompat
- Material Components
- ConstraintLayout
- SQLite
- Gradle

## 环境要求

- Android Studio
- JDK 8 或兼容版本
- Android Gradle Plugin 对应环境
- `minSdk`: 28
- `compileSdk`: 32
- `targetSdk`: 34

## 目录结构

```text
Android_tally/
├── app/
│   ├── build.gradle
│   └── src/
│       ├── main/
│       │   ├── AndroidManifest.xml
│       │   ├── java/com/example/qiantu_z/
│       │   │   ├── MainActivity.java
│       │   │   ├── ChartActivity.java
│       │   │   ├── RecordActivity.java
│       │   │   ├── SettingActivity.java
│       │   │   ├── adapter/
│       │   │   ├── db/
│       │   │   ├── frag_record/
│       │   │   └── utils/
│       │   └── res/
│       ├── androidTest/
│       └── test/
├── build.gradle
├── gradle/
├── gradlew
├── gradlew.bat
└── settings.gradle
```

## 快速开始

1. 克隆项目：

```bash
git clone https://github.com/siberiagroundhog/Android_tally.git
cd Android_tally
```

2. 使用 Android Studio 打开项目根目录。

3. 等待 Gradle 同步完成。

4. 连接 Android 设备或启动模拟器。

5. 点击 Run 运行应用。

也可以在命令行构建调试包：

```bash
./gradlew assembleDebug
```

Windows 环境可使用：

```bat
gradlew.bat assembleDebug
```

## 核心模块说明

- `MainActivity.java`: 应用主页面和核心入口。
- `RecordActivity.java`: 账目记录相关页面。
- `ChartActivity.java`: 收支统计图表页面。
- `SettingActivity.java`: 设置页面。
- `db/`: 数据库实体、数据库打开工具和数据访问逻辑。
- `adapter/`: 列表与页面适配器。
- `frag_record/`: 收入、支出记录 Fragment 及其通用逻辑。
- `utils/`: 键盘等工具类。
- `res/`: 布局、图片、字符串、主题等 Android 资源。

## 后续优化方向

- 补充更完整的 README 截图和功能演示。
- 增加账目搜索、筛选和导出功能。
- 优化数据库异常处理与数据迁移逻辑。
- 增加单元测试和 UI 自动化测试。
- 将包名从示例命名调整为正式应用命名。
- 适配更多 Android 版本和屏幕尺寸。

## 仓库地址

https://github.com/siberiagroundhog/Android_tally
