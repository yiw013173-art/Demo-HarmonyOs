# hvigor 工具说明

## ❌ 错误：npm install -g @ohos/hvigor-ohos-plugin 失败

`@ohos/hvigor-ohos-plugin` **不在 npm 官方仓库中**，无法通过 npm 安装。

## ✅ 正确的解决方案

### 方案一：使用 DevEco Studio（推荐）

hvigor 工具随 **DevEco Studio** 一起安装，不需要单独安装。

1. **下载并安装 DevEco Studio**
   - 下载地址: https://developer.harmonyos.com/cn/develop/deveco-studio
   - 安装后，hvigor 会自动配置

2. **在 DevEco Studio 中打开项目**
   - 使用 DevEco Studio 打开项目
   - 使用 DevEco Studio 的构建功能

### 方案二：直接使用已有 HAP 文件（当前推荐）

如果你的项目已经有构建好的 HAP 文件，**不需要重新构建**：

1. 在 Cursor 中运行 **"安装 HAP 包（默认设备）"** 任务
2. 应用会自动安装并启动

### 方案三：检查是否已安装 hvigor

如果你已经安装了 DevEco Studio，hvigor 可能已经在系统中：

```bash
# 检查 hvigor 是否可用
which hvigor

# 如果找到，可以直接使用
hvigor assembleHap --mode debug
```

## 📝 总结

- ✅ **不需要**通过 npm 安装 `@ohos/hvigor-ohos-plugin`
- ✅ **推荐**使用 DevEco Studio 构建项目
- ✅ **如果已有 HAP 文件**，直接使用安装任务即可
- ✅ **hvigor** 随 DevEco Studio 一起安装

## 🔧 当前项目状态

- ✅ 已有 HAP 文件：`entry/build/default/outputs/default/entry-default-unsigned.hap`
- ✅ 可以直接安装和运行，无需重新构建
- ⚠️ 如果需要重新构建，请使用 DevEco Studio


