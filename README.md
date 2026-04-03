# ⚡ 摩擦审计

找到消耗你时间的事，让 AI 帮你解决。

## 功能

- **记录摩擦** — 记录日常工作中让你觉得烦、重复、低效的事
- **AI 诊断** — 自动分析每个摩擦点，给出解决方案和优先级
- **构建方案** — 和 AI 对话，把方案落地成具体工具/模板
- **每周总结** — 统计趋势、找出时间黑洞、AI 生成周报洞察

## 部署到 GitHub Pages

### 步骤 1：创建仓库

1. 登录 GitHub，点右上角 **+** → **New repository**
2. 仓库名填 `friction-audit`（或任意名字）
3. 选择 **Public**
4. 点 **Create repository**

### 步骤 2：上传文件

最简单的方式 — 直接在网页上操作：

1. 在新建的仓库页面，点 **uploading an existing file**
2. 把 `index.html` 文件拖进去
3. 点 **Commit changes**

或者用命令行：

```bash
git init
git add index.html
git commit -m "init: friction audit app"
git branch -M main
git remote add origin https://github.com/你的用户名/friction-audit.git
git push -u origin main
```

### 步骤 3：开启 GitHub Pages

1. 进入仓库 → **Settings** → 左侧找到 **Pages**
2. Source 选 **Deploy from a branch**
3. Branch 选 **main**，文件夹选 **/ (root)**
4. 点 **Save**

### 步骤 4：访问

等 1-2 分钟，你的应用就上线了：

```
https://你的用户名.github.io/friction-audit/
```

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
