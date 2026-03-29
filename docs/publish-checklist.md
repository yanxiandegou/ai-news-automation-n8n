# GitHub 发布清单

## 推荐仓库名

- `ai-news-automation-n8n`
- `n8n-news-digest-workflow`

## 发布步骤

1. 在 GitHub 新建一个 `Public` 仓库。
2. 在本地项目目录执行以下命令：

```powershell
git remote add origin https://github.com/<你的用户名>/ai-news-automation-n8n.git
git push -u origin main
```

3. 打开仓库主页，确认以下内容正常显示：

- `README.md`
- `images/` 下的 SVG 图片
- `workflow/news-automation-sanitized.json`

## 简历中如何放链接

优先放仓库主页链接：

```text
https://github.com/<你的用户名>/ai-news-automation-n8n
```

不要只放单个 JSON 文件链接，因为招聘方通常更愿意先看 README 和项目说明。

## 发布前最后检查

- 仓库可公开访问
- README 首屏能看懂项目价值
- 工作流文件不包含真实 token / table id / credentials
- 图片链接正常显示
