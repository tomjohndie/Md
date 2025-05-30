.env并更改以下两点

```
USE_DB_AUTHENTICATION=false

TEST_API_KEY=fc-my-firecrawl
```

## 分页机制
当数据超过 10MB 或任务未完成时，响应包含 next 参数用于获取后续数据

## 爬取参数配置
路径包含规则 includePaths
-类型: array 
- 示例: ["/blog/*", "/products/*"]

## 路径排除规则 excludePaths
-类型: array 
- 示例: ["/admin/*", "/login/*"]

## 最大深度 maxDepth
-类型: integer 
- 说明: ◦ 0: 仅爬取当前页面 ◦ 1: 爬取当前页面及一级子页面 ◦ 2: 爬取至二级子页面

## 数量限制 limit
- 类型: integer • 默认值: 10000

## 允许回链 allowBackwardLinks
- 类型: boolean
- 说明: 允许爬取上级目录链接
- 默认值: false

## 允许外链 allowExternalLinks
- 类型: boolean
- 说明: 允许爬取外部域名链接
- 默认值: false

## 嵌套抓取配置 scrapeOptions
- 类型: object
- 说明: 继承 抓取参数配置
- 默认值: { "formats": ["markdown"] }

## 完整配置示例

```
curl -X POST https://api.firecrawl.dev/v1/crawl \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://docs.firecrawl.dev",
      "includePaths": ["/blog/*", "/products/*"],
      "excludePaths": ["/admin/*", "/login/*"],
      "maxDepth": 2,
      "limit": 1000
    }'
```
