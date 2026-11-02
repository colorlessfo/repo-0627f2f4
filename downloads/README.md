# Windows 本机接入诊断工具

## 当前推荐：免 npm 安装版

下载 **Yuliang_Ready.zip** 并点击“全部解压缩”。该包已包含经过 npm 原始 SHA-512 完整性验证的 Playwright / playwright-core 1.64.1 及其 LICENSE、NOTICE、ThirdPartyNotices，仍需要电脑上已有 Node.js 24+ 和 Microsoft Edge。

打开同时包含 tools、node_modules 和 package.json 的普通文件夹，在文件资源管理器地址栏输入 cmd、回车，然后只运行：

```text
node tools\local-probe\run.mjs
```

不运行 npm，不双击旧版启动脚本，不修改 Windows 智能应用控制、Node/npm 路径或金融平台设置。若再次被安全控制阻止，保持拦截并停止。详细说明见 [READY_RUN.md](READY_RUN.md)。

免 npm 包 SHA-256：`6be3231e532f6b7cd9812205b973300febde72c63b87dca78505540a35665c96`

工具菜单：1 支付宝、2 交通银行、3 微信支付、4 微信理财通、5 蜻蜓点金。均为接入诊断选项，尚未验证为自动同步可用。由本人在官方界面登录；只分享脱敏结构报告，不分享 Cookie、密码、原始账单或 profiles。

本次独立解压、依赖导入、CLI 帮助和合成 Chromium 响应验证通过；没有 Windows Edge/真实账户/智能应用控制允许结果，不宣称已接通。

## 历史包

Yuliang_Finance_v0.3_Local_Probe.zip 为旧批处理启动版；启动脚本曾被用户的智能应用控制拦截，不继续运行该脚本。Yuliang_Finance_v0.3_Source_Run.zip 为需要 npm 安装依赖的源码版。两者仅保留历史。
