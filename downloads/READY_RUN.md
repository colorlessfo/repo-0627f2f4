# 余量财务：免 npm 安装版

本包已包含固定版本的浏览器驱动依赖。需要现有的 **Node.js 24+ 和 Microsoft Edge**，不需要运行 `npm ci` 或修复 npm。

## 开始

1. 完整解压 `Yuliang_Ready.zip`。不要直接在 ZIP 预览里运行。解压后的普通文件夹应同时包含 `tools`、`node_modules` 和 `package.json`。
2. 在这个文件夹窗口按 **Alt+D**，输入 `cmd`，按回车。
3. 在打开的命令提示符中，只运行这一条：

```text
node tools\local-probe\run.mjs
```

4. 等待平台菜单：1 支付宝、2 交通银行、3 微信支付、4 微信理财通、5 蜻蜓点金。输入数字后回车。
5. 在独立 Edge 中自行完成官方登录并进入只读查询页，按命令窗口提示继续。仅分享生成的脱敏结构 JSON，不分享密码、验证码、Cookie、profiles 或 HAR。

这次不需要 `npm` 命令，不需要双击任何 `.cmd`、PowerShell 或安装辅助文件。不更改 Node/npm 的安装位置、PATH、Windows 智能应用控制或金融平台设置。Windows 若再次拦截，保持拦截并停止，不能通过改名、解除阻止或关闭保护来运行。

## 包含内容与来源

本项目采集代码保持 v0.3 原样。额外包含 Playwright 和 playwright-core 1.64.1 的完整上游 npm 发布包；打包时从 registry.npmjs.org 下载，并验证现有锁文件的 SHA-512 integrity。每个依赖的 LICENSE、NOTICE 和 ThirdPartyNotices.txt 均原样保留在其目录内。VENDOR_INTEGRITY.json 记录来源与校验值。

完整上游包内有浏览器安装辅助脚本；本工具不调用这些脚本，不下载额外浏览器，也不要求用户运行它们。这里只使用已安装的 Edge。没有随包分发 Node.exe、真实账单、登录资料、运行时 profiles、外传服务或自动登录功能。

诊断工具只被动观察官方查询页面收到的 JSON，不重放请求、不付款转账或交易；仍不是五平台自动同步完成版。微信个人账单桌面入口尚未验证。免 npm 包的依赖导入与合成 Chromium 响应流程可在云端验证，真实 Windows Edge 和智能应用控制允许结果以本人电脑为准。
