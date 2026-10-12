# YouTube Digest · Notes 分类版（Chrome 扩展）

这是可在 Chrome 中“加载已解压的扩展程序”的完整扩展源码，不是 Codex Skill，也不是双击安装的程序。基于 [YouTube Digest](https://github.com/zarazhangrui/youtube-digest) 改造；原项目的 MIT 许可及 Zara Zhang 署名保留在 [LICENSE](LICENSE)。

安装包：[下载 v1.4.1 ZIP](youtube-digest-notes-v1.4.1.zip)。如果 GitHub 先显示文件详情，请点击右上角的下载按钮。

## 能做什么

- 在 YouTube 长视频旁查看字幕、双语翻译和 AI 内容概览。
- 点击字幕里的单词，查看释义、音标、发音和固定搭配。
- 将生词与值得记的表达分别保存为 Notes，并保留视频语境。
- 在本地备份或合并导入 Notes；备份不会随扩展安装包公开。

## 安装

1. 下载本扩展的 ZIP 并解压到准备长期保留的文件夹。不要在 Chrome 中直接选择 ZIP。
2. 打开 `chrome://extensions`，开启“开发者模式”，点击“加载已解压的扩展程序”。
3. 选择**直接包含 `manifest.json`** 的文件夹。如果下载的是整个仓库，请先找到其中的扩展文件夹，不要选仓库最外层。
4. 打开扩展的设置页，**自行**填写 Supadata 和 DeepSeek API Key。安装包不附带密钥或 API 额度，也没有运营中的后端服务器。
5. 打开带字幕的 YouTube 视频测试。若该视频无法提供字幕，相关学习功能也可能不可用。

此扩展未上架 Chrome 网上应用店。通过“加载已解压的扩展程序”安装后不会自动更新；更新文件后需在 `chrome://extensions` 点击“重新加载”，并刷新 YouTube 页面。请保持扩展文件夹的位置不变。

## 从旧版迁移 Notes

不要同时启用多个版本的 YouTube Digest；之前曾出现视频页无响应的问题。升级前，先在旧版的“Notes 备份与迁移”页面下载备份，并确认文件确实保存成功。新版如果显示为另一个扩展，原 Notes 不会自动出现；请在新版的同一页面选择备份文件并“确认合并导入”。确认 Notes 都可见以后，再决定是否停用旧版。**不要把 Notes 备份 JSON 上传到公开 GitHub 仓库。**

## 隐私与来源

扩展的设置和 Notes 保存在用户自己的 Chrome 本地扩展存储中；使用 Supadata 或 DeepSeek 功能时，请求会发送给对应服务。请为密钥设置合适的额度限制，不要把密钥写进源码、Issue 或聊天记录。这个仓库只提供扩展代码和示例，不含用户私人 Notes、密钥或浏览器数据。

本版本是个人改造，不是原项目的官方版本。许可证见 [LICENSE](LICENSE)。
