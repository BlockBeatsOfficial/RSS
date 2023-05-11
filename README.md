# BlockBeats_RSS
Making it more convenient for you to access Web3 information through RSS subscriptions . 
# RSS 接口文档
## 简介
This document describes the BlockBeats RSS interface, which provides information about the latest articles on our website
https://api.theblockbeats.news/v1/open-api/home-xml


## 请求参数

本接口目前不支持任何请求参数。

## 响应格式

RSS 接口返回一个 XML 文档，包含以下元素：

- `<channel>`: 包含有关 RSS 频道的信息。
  - `<title>`: 频道标题。
  - `<link>`: 频道的 URL。
  - `<description>`: 频道描述。
  - `<item>`: 包含一个文章的信息。一个 `<channel>` 可以包含多个 `<item>`。
    - `<title>`: 文章标题。
    - `<link>`: 文章的 URL。
    - `<description>`: 文章摘要。
    - `<pubDate>`: 文章发布日期。

## 使用示例

访问以下 URL 以获取 RSS 数据：


示例响应：

```xml
<?xml version="1.0" encoding="UTF-8"?>
<rss version="2.0">
  <channel>
    <title>Example Website</title>
    <link>https://example.com</link>
    <description>Latest articles from Example Website</description>
    <item>
      <title>Article 1</title>
      <link>https://example.com/article-1</link>
      <description>Summary of Article 1</description>
      <pubDate>Tue, 11 May 2021 10:00:00 GMT</pubDate>
    </item>
    <item>
      <title>Article 2</title>
      <link>https://example.com/article-2</link>
      <description>Summary of Article 2</description>
      <pubDate>Wed, 12 May 2021 10:00:00 GMT</pubDate>
    </item>
    <!-- More items can be added here -->
  </channel>
</rss>

