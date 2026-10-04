# ImgPrompt — 图像提示词构建器

一个单文件、零依赖的 AI 绘画提示词拼装工具。不会写英文提示词？点几下芯片，就能拼出一串 Midjourney / Stable Diffusion / DALL-E 风格的高质量 prompt。

**打开即用**：双击 `index.html`，无需安装、无需联网、无需构建。

## 功能

- **主体输入**：支持中文；一键 **AI 润色**，把一句中文扩展成 30–60 词的英文细节描述（用你自己的 OpenAI 兼容 API Key）
- **六组风格芯片**：风格（14 种：赛博朋克 / 水墨 / 电影感 / 像素风 / 油画 / 吉卜力…）、灯光（8 种）、镜头（7 种）、构图（6 种）、氛围（6 种）、画质标签（6 种），点选即拼装
- **画幅比例**：1:1 / 16:9 / 9:16 / 3:2 / 21:9，一键切换 Midjourney `--ar 16:9` 或通用 `aspect ratio 16:9` 后缀
- **反向提示词**：常用预设一键勾选（低质量 / 水印 / 手部畸形…）+ 自由输入
- **实时预览**：按板块彩色高亮、字符计数、一键复制
- **随机灵感**：一键随机组合，突破选择困难
- **收藏夹**：常用组合存 localStorage，随时载入
- **3 个示例**：霓虹雨夜猫 / 山水意境 / 沙漠史诗，一键载入
- **中英双语界面**：一键切换

## 隐私

API Key 只保存在本机浏览器 `localStorage`，点击"润色"时**仅**发送到你在设置里填写的 API 地址，不会发往任何其他地方。本页面本身不含任何外部请求、统计或追踪代码。

## 文件

| 文件 | 说明 |
|---|---|
| `index.html` | 应用本体（单文件，~40KB，零依赖） |
| `README.md` | 本说明 |
| `LICENSE` | MIT |

## 适用提示词格式

- **Midjourney**：画幅选 `--ar` 格式，直接粘贴到 Discord 输入框
- **Stable Diffusion / 通用**：画幅选 `aspect ratio` 格式，反向词填进 Negative prompt 框

## English

ImgPrompt is a single-file, zero-dependency image-prompt builder. Open `index.html` in any browser — no install, no network, no build. Pick style/lighting/camera/composition/mood/quality chips, set aspect ratio (`--ar` or plain format), add negative prompts, copy the composed prompt. Optional AI polish turns a short Chinese subject into a detailed English fragment using your own OpenAI-compatible API key (stored in localStorage only, sent only to your configured endpoint).

## License

MIT — see [LICENSE](LICENSE).
