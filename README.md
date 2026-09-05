# crpatchwork 🐦✂️

**青知更鸟的拼布工坊** —— 一个纯本地、离线可用的 SillyTavern 预设可视化编辑器。

用拖拽卡片的方式查看、排序、编辑 SillyTavern 预设里的每一条提示词（prompt），像拼布一样把别人作品里好用的片段，拆下来重新拼成你自己的风格。**单文件 HTML，双击即用，无依赖、不上传任何数据。**

> 🌙 支持夜间模式 · ⧉ 支持跨标签页复制/粘贴条目

---

## 它能做什么

- 左列卡片 = 一条提示词（prompt），可直接**拖拽换序**
- 点卡片选中，点 **✎** 在右侧编辑内容 / role / 注入位置 / 深度 / order
- **🔒 锁定槽位**自动识别（Char Description / 人物性格 / 场景 / 世界设定等由酒馆从人物卡填充的条目），防止误改
- **⧉ 复制**一条 → 开另一个页面 → **📋 粘贴**到别的预设里（跨标签页互抄）
- 🌙 **夜间模式**，偏好自动记住
- **导出 JSON** 时只重写 `prompts` / `prompt_order`，其余字段原样保留，酒馆能直接读回

## 怎么用

1. 打开 `st-preset-drag-editor.html`（双击即可，纯本地，断网也能用）
2. 右上「📂 打开 JSON」或直接把 `.json` 拖进窗口
3. 编辑完点「⬇ 导出 JSON」，得到 `xxx_edited.json`，放进 SillyTavern 的预设目录即可

> 本工具不保存、不上传你的任何数据，所有内容都在你自己的浏览器里，刷新即失 —— 记得及时导出。

## 怎么自己跑 / 二次开发

这是**零构建**的单文件 HTML，逻辑都在 `<script>` 里，用编辑器打开就能改。改完直接刷新浏览器即可生效。

## 发布/自己部署

整个仓库静态托管即可（GitHub Pages / Cloudflare Pages / 任意静态服务器都行）。

---

## ⚠️ 免责声明 / Disclaimer

**简体中文（自留参考）：**

本仓库**仅且只**提供一个通用、中立的**文件查看与编辑工具**，**不包含任何成人、色情、政治敏感或非法内容**，也**不提供任何此类内容的来源、指引或生成能力**。

- 本工具是一个**纯客户端、纯本地**的 JSON 编辑器，**不会联网、不上传、不采集**任何用户数据、文件或隐私。
- 使用者通过本工具查看或编辑的 `.json` 文件，**完全由使用者自己导入**。工具本身不生产、不存储、不传播其中任何文本内容。
- **工具不可被滥用于生成或分发违法内容** —— 但请理解：一个文本编辑器可以用来写小说，也可能被用来打草稿，**工具的用途取决于使用它的人**。作者**无法、也不会**监控或控制任何使用者的具体行为。
- 若使用者导入、编辑、导出了包含**他人创作**或**受版权/许可保护**的内容，其来源、授权与合规责任**完全由该使用者自行承担**，与作者无关。
- 若使用者所在国家/地区的法律禁止其使用此类工具，或禁止其查看/持有其所导入的内容，**使用与否由使用者自行判断并承担全部后果**。
- 作者**不对任何**因使用、误用、无法使用本工具而产生的直接、间接、附带或后果性损害负责，包括但不限于数据丢失、预设损坏、账号异常等。
- 本工具按 **“AS IS”（现状）** 提供，**不附带任何明示或默示担保**，包括但不限于适销性、特定用途适用性及不侵权担保。

**English (for legal clarity):**

This repository provides **only** a generic, neutral, **client-side file viewer/editor**. It contains **no adult, sexual, political, or unlawful content**, and offers **no source, guidance, or generation** of any such content.

- This is a **fully local, offline** JSON editor. It does **not** connect to any network, and it does **not** upload, collect, or store any user data, files, or privacy.
- Any `.json` file a user views or edits is **imported entirely by that user**. This tool does not produce, host, or transmit any of the text inside those files.
- This tool must not be used to produce or distribute unlawful material — however, like any text editor, **its actual use depends on the person using it**. The author **cannot and does not** monitor or control how any individual chooses to use it.
- If a user imports, edits, or exports content that includes **third-party creations** or content protected by **copyright / license**, responsibility for its origin, permission, and compliance lies **entirely with that user**, not the author.
- If the law of a user's country/region prohibits the use of such a tool, or the viewing/possession of the content they import, the decision and all consequences rest **solely with the user**.
- The author is **not liable** for any direct, indirect, incidental, or consequential damages arising from the use, misuse, or inability to use this tool — including, but not limited to, data loss, preset corruption, or account issues.
- This tool is provided **“AS IS”**, **without warranty of any kind**, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.

---

## License

Released under the **MIT License**. See [LICENSE](LICENSE). You are free to use, modify, and distribute it — but you do so **at your own risk**, and under the full terms of the disclaimer above.
