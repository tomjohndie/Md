<h3 align="center">
  <a name="readme-top"></a>
  <img
    src="https://raw.githubusercontent.com/mendableai/firecrawl/main/img/firecrawl_logo.png"
    height="200"
  >
</h3>
<div align="center">
    <a href="https://github.com/mendableai/firecrawl/blob/main/LICENSE">
  <img src="https://img.shields.io/github/license/mendableai/firecrawl" alt="License">
</a>
    <a href="https://pepy.tech/project/firecrawl-py">
  <img src="https://static.pepy.tech/badge/firecrawl-py" alt="Downloads">
</a>
<a href="https://GitHub.com/mendableai/firecrawl/graphs/contributors">
  <img src="https://img.shields.io/github/contributors/mendableai/firecrawl.svg" alt="GitHub Contributors">
</a>
<a href="https://firecrawl.dev">
  <img src="https://img.shields.io/badge/Visit-firecrawl.dev-orange" alt="Visit firecrawl.dev">
</a>
</div>
<div>
  <p align="center">
    <a href="https://twitter.com/firecrawl_dev">
      <img src="https://img.shields.io/badge/Follow%20on%20X-000000?style=for-the-badge&logo=x&logoColor=white" alt="Follow on X" />
    </a>
    <a href="https://www.linkedin.com/company/104100957">
      <img src="https://img.shields.io/badge/Follow%20on%20LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Follow on LinkedIn" />
    </a>
    <a href="https://discord.com/invite/gSmWdAkdwd">
      <img src="https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join our Discord" />
    </a>
  </p>
</div>

# 🔥 Firecrawl

通过任何网站的干净数据增强您的 AI 应用。具有先进的抓取、爬虫和数据提取能力。

_该存储库正在开发中，我们仍在将自定义模块集成到单一代码库中。它尚未完全准备好进行自托管部署，但您可以在本地运行。_

## 什么是 Firecrawl？

[Firecrawl](https://firecrawl.dev?ref=github) 是一个 API 服务，它接受一个 URL，爬取该 URL，并将其转换为干净的 Markdown 或结构化数据。我们会爬取所有可访问的子页面，并为每个页面提供干净的数据。无需站点地图。查看我们的 [文档](https://docs.firecrawl.dev)。

_嘿，快来加入我们的星标者吧 :)_

<a href="https://github.com/mendableai/firecrawl">
  <img src="https://img.shields.io/github/stars/mendableai/firecrawl.svg?style=social&label=Star&maxAge=2592000" alt="GitHub stars">
</a>

## 如何使用？

我们提供了一个易于使用的 API，您可以使用我们的托管版本。您可以在 [这里](https://firecrawl.dev/playground) 找到游乐场和文档。如果您愿意，也可以自托管后端。

查看以下资源以开始使用：
- [x] **API**: [文档](https://docs.firecrawl.dev/api-reference/introduction)
- [x] **SDK**: [Python](https://docs.firecrawl.dev/sdks/python), [Node](https://docs.firecrawl.dev/sdks/node), [Go](https://docs.firecrawl.dev/sdks/go), [Rust](https://docs.firecrawl.dev/sdks/rust)
- [x] **LLM 框架**: [Langchain (python)](https://python.langchain.com/docs/integrations/document_loaders/firecrawl/), [Langchain (js)](https://js.langchain.com/docs/integrations/document_loaders/web_loaders/firecrawl), [Llama Index](https://docs.llamaindex.ai/en/latest/examples/data_connectors/WebPageDemo/#using-firecrawl-reader), [Crew.ai](https://docs.crewai.com/), [Composio](https://composio.dev/tools/firecrawl/all), [PraisonAI](https://docs.praison.ai/firecrawl/), [Superinterface](https://superinterface.ai/docs/assistants/functions/firecrawl), [Vectorize](https://docs.vectorize.io/integrations/source-connectors/firecrawl)
- [x] **低代码框架**: [Dify](https://dify.ai/blog/dify-ai-blog-integrated-with-firecrawl), [Langflow](https://docs.langflow.org/), [Flowise AI](https://docs.flowiseai.com/integrations/langchain/document-loaders/firecrawl), [Cargo](https://docs.getcargo.io/integration/firecrawl), [Pipedream](https://pipedream.com/apps/firecrawl/)
- [x] **其他**: [Zapier](https://zapier.com/apps/firecrawl/integrations), [Pabbly Connect](https://www.pabbly.com/connect/integrations/firecrawl/)
- [ ] 想要一个 SDK 或集成？请通过打开问题告诉我们。

要在本地运行，请参考 [这里](https://github.com/mendableai/firecrawl/blob/main/CONTRIBUTING.md) 的指南。

### API 密钥

要使用 API，您需要在 [Firecrawl](https://firecrawl.dev) 上注册并获取 API 密钥。

### 特性

- [**抓取**](#scraping): 抓取一个 URL 并以 LLM 准备好的格式（Markdown、结构化数据通过 [LLM 提取](#llm-extraction-beta)、截图、HTML）获取其内容
- [**爬虫**](#crawling): 抓取网页的所有 URL 并以 LLM 准备好的格式返回内容
- [**映射**](#map-alpha): 输入一个网站并获取所有网站 URL - 极其快速
- [**搜索**](#search): 在网上搜索并获取结果的完整内容
- [**提取**](#extract): 从单个页面、多页或整个网站获取结构化数据，使用 AI。

### 功能

- [**抓取**](#scraping): 抓取一个 URL 并以 LLM 准备好的格式获取其内容（markdown、结构化数据通过 [LLM 提取](#llm-extraction-beta)、截图、html）
- [**爬取**](#crawling): 抓取一个网页的所有 URL 并以 LLM 准备好的格式返回内容
- [**映射**](#map-alpha): 输入一个网站并获取所有网站 URL - 极其快速
- [**搜索**](#search): 在网上搜索并从结果中获取完整内容
- [**提取**](#extract): 从单个页面、多个页面或整个网站获取结构化数据

### 强大功能
- **LLM 准备好的格式**: markdown、结构化数据、截图、HTML、链接、元数据
- **处理复杂内容**: 代理、反机器人机制、动态内容（js 渲染）、输出解析、编排
- **可定制性**: 排除标签、使用自定义头部在认证墙后爬取、最大爬取深度等
- **媒体解析**: pdf、docx、图片
- **可靠性优先**: 旨在获取所需数据 - 无论多么困难
- **操作**: 点击、滚动、输入、等待等，然后提取数据
- **批处理（新）**: 同时抓取数千个 URL，使用新的异步端点。

您可以在我们的 [文档](https://docs.firecrawl.dev) 中找到 Firecrawl 的所有功能及其使用方法。

### 爬取

用于爬取一个 URL 及其所有可访问的子页面。此操作提交一个爬取作业并返回一个作业 ID，以检查爬取的状态。

```bash
curl -X POST https://api.firecrawl.dev/v1/crawl \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer fc-YOUR_API_KEY' \
    -d '{
      "url": "https://docs.firecrawl.dev",
      "limit": 10,
      "scrapeOptions": {
        "formats": ["markdown", "html"]
      }
    }'
```

返回一个爬取作业 ID 和检查爬取状态的 URL。

```json
{
  "success": true,
  "id": "123-456-789",
  "url": "https://api.firecrawl.dev/v1/crawl/123-456-789"
}
```

### 检查爬取作业

用于检查爬取作业的状态并获取其结果。

```bash
curl -X GET https://api.firecrawl.dev/v1/crawl/123-456-789 \
  -H 'Content-Type: application/json' \
  -H 'Authorization: Bearer YOUR_API_KEY'
```

```json
{
  "status": "completed",
  "total": 36,
  "creditsUsed": 36,
  "expiresAt": "2024-00-00T00:00:00.000Z",
  "data": [
    {
      "markdown": "[Firecrawl Docs home page![light logo](https://mintlify.s3-us-west-1.amazonaws.com/firecrawl/logo/light.svg)!...",
      "html": "<!DOCTYPE html><html lang=\"en\" class=\"js-focus-visible lg:[--scroll-mt:9.5rem]\" data-js-focus-visible=\"\">...",
      "metadata": {
        "title": "Build a 'Chat with website' using Groq Llama 3 | Firecrawl",
        "language": "en",
        "sourceURL": "https://docs.firecrawl.dev/learn/rag-llama3",
        "description": "Learn how to use Firecrawl, Groq Llama 3, and Langchain to build a 'Chat with your website' bot.",
        "ogLocaleAlternate": [],
        "statusCode": 200
      }
    }
  ]
}
```

### 抓取

用于抓取一个 URL 并以指定格式获取其内容。

```bash
curl -X POST https://api.firecrawl.dev/v1/scrape \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://docs.firecrawl.dev",
      "formats" : ["markdown", "html"]
    }'
```

响应：

```json
{
  "success": true,
  "data": {
    "markdown": "Launch Week I is here! [See our Day 2 Release 🚀](https://www.firecrawl.dev/blog/launch-week-i-day-2-doubled-rate-limits)[💥 Get 2 months free...",
    "html": "<!DOCTYPE html><html lang=\"en\" class=\"light\" style=\"color-scheme: light;\"><body class=\"__variable_36bd41 __variable_d7dc5d font-inter ...",
    "metadata": {
      "title": "Home - Firecrawl",
      "description": "Firecrawl crawls and converts any website into clean markdown.",
      "language": "en",
      "keywords": "Firecrawl,Markdown,Data,Mendable,Langchain",
      "robots": "follow, index",
      "ogTitle": "Firecrawl",
      "ogDescription": "Turn any website into LLM-ready data.",
      "ogUrl": "https://www.firecrawl.dev/",
      "ogImage": "https://www.firecrawl.dev/og.png?123",
      "ogLocaleAlternate": [],
      "ogSiteName": "Firecrawl",
      "sourceURL": "https://firecrawl.dev",
      "statusCode": 200
    }
  }
}
```

### 地图

用于映射一个 URL 并获取该网站的 URL。这将返回网站上大多数链接.

```bash cURL
curl -X POST https://api.firecrawl.dev/v1/map \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://firecrawl.dev"
    }'
```

Response:

```json
{
  "status": "success",
  "links": [
    "https://firecrawl.dev",
    "https://www.firecrawl.dev/pricing",
    "https://www.firecrawl.dev/blog",
    "https://www.firecrawl.dev/playground",
    "https://www.firecrawl.dev/smart-crawl",
  ]
}
```

#### 带搜索的映射
带有 search 参数的映射允许您在网站内部搜索特定的 URL.

```bash cURL
curl -X POST https://api.firecrawl.dev/v1/map \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://firecrawl.dev",
      "search": "docs"
    }'
```

响应将是一个按相关性从高到低排序的列表.

```json
{
  "status": "success",
  "links": [
    "https://docs.firecrawl.dev",
    "https://docs.firecrawl.dev/sdks/python",
    "https://docs.firecrawl.dev/learn/rag-llama3",
  ]
}
```

### 搜索

在网上搜索并从结果中获取完整内容

Firecrawl 的搜索 API 允许您执行网络搜索，并可选择在一次操作中抓取搜索结果.

-选择特定的输出格式（markdown、HTML、链接、截图）
-使用可自定义的参数（语言、国家等）进行网络搜索
-可选择以各种格式检索搜索结果中的内容
-控制结果数量并设置超时

```bash
curl -X POST https://api.firecrawl.dev/v1/search \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer fc-YOUR_API_KEY" \
  -d '{
    "query": "what is firecrawl?",
    "limit": 5
  }'
```

#### 响应(Response)

```json
{
  "success": true,
  "data": [
    {
      "url": "https://firecrawl.dev",
      "title": "Firecrawl | Home Page",
      "description": "Turn websites into LLM-ready data with Firecrawl"
    },
    {
      "url": "https://docs.firecrawl.dev",
      "title": "Documentation | Firecrawl",
      "description": "Learn how to use Firecrawl in your own applications"
    }
  ]
}
```

#### 带内容抓取(With content scraping)

```bash
curl -X POST https://api.firecrawl.dev/v1/search \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer fc-YOUR_API_KEY" \
  -d '{
    "query": "what is firecrawl?",
    "limit": 5,
    "scrapeOptions": {
      "formats": ["markdown", "links"]
    }
  }'
```

### 提取（测试版）Extract (Beta)

从整个网站获取结构化数据，使用提示和/或模式.

您可以从一个或多个 URL 提取结构化数据，包括通配符:

单个页面:
示例: https://firecrawl.dev/some-page

多个页面 / 整个域名
示例: https://firecrawl.dev/*

当您使用 /* 时，Firecrawl 将自动爬取并解析它可以发现的该域名下的所有 URL，然后提取请求的数据。.

```bash
curl -X POST https://api.firecrawl.dev/v1/extract \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "urls": [
        "https://firecrawl.dev/*", 
        "https://docs.firecrawl.dev/", 
        "https://www.ycombinator.com/companies"
      ],
      "prompt": "Extract the company mission, whether it is open source, and whether it is in Y Combinator from the page.",
      "schema": {
        "type": "object",
        "properties": {
          "company_mission": {
            "type": "string"
          },
          "is_open_source": {
            "type": "boolean"
          },
          "is_in_yc": {
            "type": "boolean"
          }
        },
        "required": [
          "company_mission",
          "is_open_source",
          "is_in_yc"
        ]
      }
    }'
```

```json
{
  "success": true,
  "id": "44aa536d-f1cb-4706-ab87-ed0386685740",
  "urlTrace": []
}
```

如果您使用 SDK，它将自动为您提取响应:

```json
{
  "success": true,
  "data": {
    "company_mission": "Firecrawl is the easiest way to extract data from the web. Developers use us to reliably convert URLs into LLM-ready markdown or structured data with a single API call.",
    "supports_sso": false,
    "is_open_source": true,
    "is_in_yc": true
  }
}
```

### LLM 提取（测试版）

用于从抓取的页面中提取结构化数据.

```bash
curl -X POST https://api.firecrawl.dev/v1/scrape \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://www.mendable.ai/",
      "formats": ["json"],
      "jsonOptions": {
        "schema": {
          "type": "object",
          "properties": {
            "company_mission": {
                      "type": "string"
            },
            "supports_sso": {
                      "type": "boolean"
            },
            "is_open_source": {
                      "type": "boolean"
            },
            "is_in_yc": {
                      "type": "boolean"
            }
          },
          "required": [
            "company_mission",
            "supports_sso",
            "is_open_source",
            "is_in_yc"
          ]
        }
      }
    }'
```

```json
{
  "success": true,
  "data": {
    "content": "Raw Content",
    "metadata": {
      "title": "Mendable",
      "description": "Mendable allows you to easily build AI chat applications. Ingest, customize, then deploy with one line of code anywhere you want. Brought to you by SideGuide",
      "robots": "follow, index",
      "ogTitle": "Mendable",
      "ogDescription": "Mendable allows you to easily build AI chat applications. Ingest, customize, then deploy with one line of code anywhere you want. Brought to you by SideGuide",
      "ogUrl": "https://mendable.ai/",
      "ogImage": "https://mendable.ai/mendable_new_og1.png",
      "ogLocaleAlternate": [],
      "ogSiteName": "Mendable",
      "sourceURL": "https://mendable.ai/"
    },
    "json": {
      "company_mission": "Train a secure AI on your technical resources that answers customer and employee questions so your team doesn't have to",
      "supports_sso": true,
      "is_open_source": false,
      "is_in_yc": true
    }
  }
}
```

### 无需模式提取（新功能）

您现在可以通过仅向端点传递一个 `prompt` 来进行无模式提取。LLM 会选择数据的结构.

```bash
curl -X POST https://api.firecrawl.dev/v1/scrape \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "url": "https://docs.firecrawl.dev/",
      "formats": ["json"],
      "jsonOptions": {
        "prompt": "Extract the company mission from the page."
      }
    }'
```

### 使用操作与页面交互（仅限云服务）

Firecrawl 允许您在抓取网页内容之前对其执行各种操作。这对于与动态内容交互、浏览页面或访问需要用户交互的内容特别有用。

以下是一个示例，演示如何使用操作导航到 google.com，搜索 Firecrawl，点击第一个结果，并截取屏幕截图.

```bash
curl -X POST https://api.firecrawl.dev/v1/scrape \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
        "url": "google.com",
        "formats": ["markdown"],
        "actions": [
            {"type": "wait", "milliseconds": 2000},
            {"type": "click", "selector": "textarea[title=\"Search\"]"},
            {"type": "wait", "milliseconds": 2000},
            {"type": "write", "text": "firecrawl"},
            {"type": "wait", "milliseconds": 2000},
            {"type": "press", "key": "ENTER"},
            {"type": "wait", "milliseconds": 3000},
            {"type": "click", "selector": "h3"},
            {"type": "wait", "milliseconds": 3000},
            {"type": "screenshot"}
        ]
    }'
```

### 批量抓取多个 URL（新功能）

您现在可以同时批量抓取多个 URL。这与 /crawl 端点的工作方式非常相似。它提交一个批量抓取任务，并返回一个任务 ID，以便检查批量抓取的状态.

```bash
curl -X POST https://api.firecrawl.dev/v1/batch/scrape \
    -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer YOUR_API_KEY' \
    -d '{
      "urls": ["https://docs.firecrawl.dev", "https://docs.firecrawl.dev/sdks/overview"],
      "formats" : ["markdown", "html"]
    }'
```



## 使用 Python SDK

### 安装 Python SDK

```bash
pip install firecrawl-py
```

### 爬取网站

```python
from firecrawl.firecrawl import FirecrawlApp

app = FirecrawlApp(api_key="fc-YOUR_API_KEY")

# Scrape a website:
scrape_status = app.scrape_url(
  'https://firecrawl.dev', 
  formats=["markdown", "html"]
)
print(scrape_status)

# Crawl a website:
crawl_status = app.crawl_url(
  'https://firecrawl.dev',
  limit=100,
  scrapeOptions'={'formats': ['markdown', 'html']}
  poll_interval=30
)
print(crawl_status)
```

### 从 URL 提取结构化数据

通过 LLM 提取，您可以轻松地从任何 URL 中提取结构化数据。我们支持 pydantic 模式，以便于您的使用。以下是使用方法:

```python
class ArticleSchema(BaseModel):
    title: str
    points: int 
    by: str
    commentsURL: str

class TopArticlesSchema(BaseModel):
    top: List[ArticleSchema] = Field(..., description="Top 5 stories")

json_config = JsonConfig(schema=TopArticlesSchema.model_json_schema())

llm_extraction_result = app.scrape_url('https://news.ycombinator.com', formats=["json"], json=json_config)

print(llm_extraction_result.json)
```

## 使用 Node SDK

### 安装

要安装 Firecrawl Node SDK，您可以使用 npm：

```bash
npm install @mendable/firecrawl-js
```

### 使用方法

1. 从 [firecrawl.dev](https://firecrawl.dev) 获取 API 密钥。
2. 将 API 密钥设置为名为 `FIRECRAWL_API_KEY` 的环境变量，或将其作为参数传递给 `FirecrawlApp` 类.

```js
import FirecrawlApp, { CrawlParams, CrawlStatusResponse } from '@mendable/firecrawl-js';

const app = new FirecrawlApp({apiKey: "fc-YOUR_API_KEY"});

// Scrape a website
const scrapeResponse = await app.scrapeUrl('https://firecrawl.dev', {
  formats: ['markdown', 'html'],
});

if (scrapeResponse) {
  console.log(scrapeResponse)
}

// Crawl a website
const crawlResponse = await app.crawlUrl('https://firecrawl.dev', {
  limit: 100,
  scrapeOptions: {
    formats: ['markdown', 'html'],
  }
} satisfies CrawlParams, true, 30) satisfies CrawlStatusResponse;

if (crawlResponse) {
  console.log(crawlResponse)
}
```


### 从 URL 提取结构化数据

通过 LLM 提取，您可以轻松地从任何 URL 中提取结构化数据。我们支持 zod 模式，以便于您的使用。以下是使用方法:

```js
import FirecrawlApp from "@mendable/firecrawl-js";
import { z } from "zod";

const app = new FirecrawlApp({
  apiKey: "fc-YOUR_API_KEY"
});

// Define schema to extract contents into
const schema = z.object({
  top: z
    .array(
      z.object({
        title: z.string(),
        points: z.number(),
        by: z.string(),
        commentsURL: z.string(),
      })
    )
    .length(5)
    .describe("Top 5 stories on Hacker News"),
});

const scrapeResult = await app.scrapeUrl("https://news.ycombinator.com", {
  jsonOptions: { extractionSchema: schema },
});

console.log(scrapeResult.data["json"]);
```

## 开源与云服务

Firecrawl 是一个开源项目，采用 AGPL-3.0 许可证。

为了提供最佳的产品体验，我们在开源版本的基础上提供了 Firecrawl 的托管版本。云解决方案使我们能够持续创新，并为所有用户维护高质量、可持续的服务。

Firecrawl Cloud 可在 [firecrawl.dev](https://firecrawl.dev) 上访问，提供一系列在开源版本中不可用的功能：

![开源与云服务对比](https://raw.githubusercontent.com/mendableai/firecrawl/main/img/open-source-cloud.png)

## 贡献

我们欢迎贡献！请在提交拉取请求之前阅读我们的 [贡献指南](CONTRIBUTING.md)。如果您想自托管，请参考 [自托管指南](SELF_HOST.md)。

_最终用户在使用 Firecrawl 进行抓取、搜索和爬行时，必须遵守网站的政策。用户应在启动任何抓取活动之前，遵守适用的隐私政策和网站使用条款。默认情况下，Firecrawl 在爬行时会尊重网站的 robots.txt 文件中指定的指令。使用 Firecrawl 即表示您明确同意遵守这些条件。_

## 贡献者

<a href="https://github.com/mendableai/firecrawl/graphs/contributors">
  <img alt="贡献者" src="https://contrib.rocks/image?repo=mendableai/firecrawl"/>
</a>

## 许可证声明

本项目主要根据 GNU Affero 通用公共许可证 v3.0（AGPL-3.0）进行许可，具体信息请参见本存储库根目录中的 LICENSE 文件。然而，本项目的某些组件是根据 MIT 许可证进行许可的。有关详细信息，请参阅这些特定目录中的 LICENSE 文件。

请注意：

- AGPL-3.0 许可证适用于项目的所有部分，除非另有说明。
- SDK 和某些 UI 组件是根据 MIT 许可证进行许可的。有关详细信息，请参阅这些特定目录中的 LICENSE 文件。
- 在使用或贡献本项目时，请确保遵守您所使用的特定组件的适当许可证条款。

有关特定组件的许可详情，请参阅相应目录中的 LICENSE 文件或联系项目维护者。

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-top" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Top ↑
    </a>
</p>
