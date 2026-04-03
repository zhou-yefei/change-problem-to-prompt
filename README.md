# ⚡ 摩擦审计

找到消耗你时间的事，让 AI 帮你解决。

## 功能

- **记录摩擦** — 记录日常工作中让你觉得烦、重复、低效的事
- **AI 诊断** — 自动分析每个摩擦点，给出解决方案和优先级
- **构建方案** — 和 AI 对话，把方案落地成具体工具/模板
- **每周总结** — 统计趋势、找出时间黑洞、AI 生成周报洞察

## 使用说明

- 首次打开会要求输入 **Anthropic API Key**
- Key 仅保存在用户浏览器的 localStorage 中，不会发送到任何第三方
- 获取 API Key: https://console.anthropic.com/settings/keys
- 所有摩擦点数据也保存在本地浏览器中

## 技术栈

- 纯前端单文件，无需构建
- React 18 (CDN)
- Anthropic Claude API (浏览器直调)
- localStorage 做数据持久化
