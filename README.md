# react_umd_test

最简单的 React UMD + HTML 测试项目，包含计数器和重置按钮。

## 运行

下载仓库后，直接用浏览器打开 `index.html` 即可，无需安装 Node.js、npm 或构建工具。

也可以在项目目录运行（需要 Python 3）：

```sh
python3 -m http.server 8000
```

然后访问 http://localhost:8000 。

**需要联网**：页面从 unpkg.com 加载固定版本的 React 和 ReactDOM。

## 文件

- `index.html`：页面、样式、React 组件和交互。
- `README.md`：运行说明。

## 实现

- React **18.3.1** 和 ReactDOM **18.3.1** 的 development UMD 构建，按顺序通过 script 标签加载。
- 使用全局 `React` / `ReactDOM`、`React.createElement`、`React.useState` 和 `ReactDOM.createRoot`。
- 不使用 JSX、Babel、打包器或 npm 依赖。
- 若 CDN 加载失败，页面显示网络检查提示。

## 手动验证

1. 打开页面，确认显示 React 版本和“计数：0”。
2. 点击“+1”，确认依次显示“计数：1”“计数：2”。
3. 点击“重置”，确认恢复为“计数：0”。
4. 刷新页面，计数应重新从 0 开始。

