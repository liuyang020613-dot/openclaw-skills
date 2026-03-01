# tongxiao-search — 阿里云通义搜索服务

> 🔍 基于通义搜索 API 的实时网络搜索服务

## 描述
封装阿里云通义搜索 `genericSearch` API，提供开放域的实时搜索能力：
- 输入：搜索 query（长度 2-100 字符）
- 输出：结构化搜索结果（标题、摘要、URL、发布时间、正文）
- 协议：REST API，返回 JSON

## 用途
- 🔍 实时网络搜索
- 📰 新闻资讯检索
- 🧠 RAG 辅助（搜索相关文档/新闻/百科）
- 🤖 供其他 agent 按需调用

## 触发方式
- 通过 function call 调用 `generic_search` 工具
- 参数：`query` - 搜索问题

## 认证要求
- 需配置通义搜索 API Key（`X-API-Key`）
- 配置在 `config.yaml` 中

## API 端点
- URL: `https://cloud-iqs.aliyuncs.com/search/genericSearch`
- Method: GET
- 参数: `query` (URL 参数)

---
*Built with OpenClaw Skill Creator*