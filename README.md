# xiaobandi.github.io

「小班底 · 数字员工」官方网站。

面向 **小微企业** 与 **一人公司（OPC）**，提供智能体、技能、工作流与 RAG 知识库，
聚焦 **自媒体 / 电商 / 本地生活服务** 三类场景。

## 访问地址

https://xiaobandi.github.io

## 技术说明

单页静态站点，无构建步骤、无外部依赖。

| 文件 | 说明 |
|---|---|
| `index.html` | 整个站点（HTML + 内联 CSS + 一段年份脚本） |
| `.nojekyll` | 关闭 GitHub Pages 的 Jekyll 处理，确保静态资源原样发布 |

GitHub Pages 配置：Source 选择 **Deploy from a branch** → 分支 `main` → 目录 `/ (root)`。

## 本地预览

```bash
# 任选其一
open index.html
python3 -m http.server 8000    # 然后访问 http://localhost:8000
```

## 部署

推送到 `main` 分支后，GitHub Pages 会自动构建并发布，通常 1 分钟内生效。

```bash
git add .
git commit -m "update site"
git push
```

## 需要替换的占位内容

- 邮箱 `yang3290325@gmail.com` 出现在「联系我们」区域与页脚，如需变更请全局替换
- GitHub 链接指向 `https://github.com/xiaobandi`
- 页脚版权年份由脚本自动取当前年份，无需手动维护
