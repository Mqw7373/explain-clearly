# explain-clearly

一个供 Codex 使用的个人 skill：当你想弄懂复杂概念、流程、代码或 AI 生成的结果时，让 Codex选择合适的文字、图、交互网页或讲解视频来解释。

## 安装

在 PowerShell 中运行：

```powershell
git clone https://github.com/Mqw7373/explain-clearly.git "$env:USERPROFILE\.codex\skills\explain-clearly"
```

安装后在新的 Codex 任务中使用。更新时运行：

```powershell
git -C "$env:USERPROFILE\.codex\skills\explain-clearly" pull
```

## 使用

可以直接提出理解任务，也可以显式调用 `$explain-clearly`：

- `$explain-clearly 帮我看懂这份模型生成的分析。`
- `$explain-clearly 用图解释这段代码的数据流。`
- `$explain-clearly 做一个能调参数的页面，让我理解这个算法。`

这个 skill 会根据任务选择形式，不会为简单问题自动制作网页或视频。它借鉴 ASD-STE100 的清晰写作目标，但不包含标准全文，也不进行正式合规认证。需要严格遵守该标准时，请从 [官方渠道](https://www.asd-ste100.org/STE_downloads.html) 获取当前版本并核对完整规则和词典。
