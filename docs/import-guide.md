# n8n 导入与配置说明

## 1. 导入工作流

1. 打开 n8n 工作台。
2. 选择 `Import from File`。
3. 导入 `workflow/news-automation-sanitized.json`。

## 2. 配置需要替换的占位信息

导入后，请重点检查以下节点：

- `DeepSeek Chat Model`
- `Write to Feishu Bitable`

其中需要替换的内容：

- `APP_TOKEN_PLACEHOLDER`
- `TABLE_ID_PLACEHOLDER`

## 3. 配置凭证

你至少需要准备：

- DeepSeek API 凭证
- 飞书开放平台凭证

公开版工作流已去除原始凭证引用，因此导入后需要在 n8n 中重新绑定。

## 4. 调整数据源

公开版中的 RSS 地址为示例源，目的是便于公开展示流程结构。你可以根据自己的场景替换为真实 RSS 源或 HTTP 接口。

建议替换位置：

- `AI Feed A`
- `AI Feed B`
- `AI Feed C`
- `AI Feed D`

## 5. 运行建议

- 第一次运行建议手动执行，确认字段映射是否正常。
- 确认飞书表格列名与工作流字段一致。
- 如果要扩展更多来源，优先复用标准化节点结构，保持输出字段统一。
