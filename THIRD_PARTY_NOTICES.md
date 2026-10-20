# 第三方素材与组件

## 球体动画及应用图标

为保留用户要求的现有动画，本项目原样保留了从 https://x.ai/bot 公开前端资源取得的动画逻辑。具体文件为 `app/character.js`；`app/orbit.png`、`build/icon.ico`、`build/icon.svg` 为该动画静态帧的衍生图标。原始资源地址：`https://x.ai/_next/static/chunks/1yeohavp76p77.js`，取得于 2026-10-19，debugId 为 `f1c2a52d-410e-205c-9b03-530c131ff868`。

这些文件不适用本项目自有代码的 MIT 授权。当前没有附带上游公开再分发许可；保持动画原样不代表已经取得公开发布许可。公开上传含这些素材的源码或安装包前，需要取得相应授权，或替换为具有再分发许可的素材。本地打包产物不能作为授权证明。

本项目与 xAI、微信、Microsoft 没有官方隶属或背书关系。

## 系统图标

Lucide 图标使用 ISC 许可，见 `licenses/Lucide-ISC.txt`。微信与浏览器后备图标为项目内绘制的通用对话、浏览器符号；本项目不内置微信或 Edge 的品牌图标，运行时可读取用户已安装程序的系统图标。

## 运行环境

Electron 与 Chromium 的许可随打包运行环境提供，分别见安装目录中的 `LICENSE.electron.txt` 和 `LICENSES.chromium.html`。依赖的确切版本与校验信息记录在 `package-lock.json`。

## Windows 接口

音频使用 Windows Core Audio；Wi-Fi 与蓝牙使用 Windows 原生接口。夜间模式调用未公开承诺稳定的系统设置组件，未来 Windows 版本可能需要兼容性修正。夜间模式数据读取参考 https://github.com/kvnxiao/win-nightlight-cli 和 Microsoft Bond 格式文档；本项目不包含这些项目的代码文件。
