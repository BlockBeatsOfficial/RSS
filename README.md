# BlockBeats_RSS

https://api.theblockbeats.news/v1/open-api/home-xml

Makes it easier for you to access Web3 information via BlockBeats RSS subscriptions .

# RSS document

## BlockBeats RSS introduction

BlockBeats RSS is an XML-based file format that includes in-depth articles and real-time news updates. BlockBeats RSS can help you stay up-to-date with the latest information from [theblockbeats.info](https://theblockbeats.info) website.

Once you subscribe using a feed reader, whenever new content is published, the RSS reader will automatically fetch the article's title, summary, link, and other information, displaying it in your reader for quick browsing and reading.

## Response format

The RSS interface returns an XML document containing the following elements:

- `<channel>`: RSS channel information .
  - `<title>`: channel title .
  - `<link>`: channel URL .
  - `<description>`: channel description .
  - `<item>`: Contains information about an article . A `<channel>` can contain multiple `< items >`.
    - `<title>`: title。
    - `<description>`: description .
    - `<link>`:  URL .
    - `<pubDate>`: Publication date of article .
    - `<guid>`: guid .

## Use example

Visit the following URL to get the RSS data:

https://api.theblockbeats.news/v1/open-api/home-xml

Example response：

```xml
<rss xmlns:atom="http://www.w3.org/2005/Atom" version="2.0">
  <script/>
  <channel>
    <title>BlockBeats</title>
    <description>BlockBeats</description>
    <link>https://www.theblockbeats.info</link>
    <image>
        <url>https://image.theblockbeats.info/logo_v2.png</url>
        <title>BlockBeats</title>
        <link>https://www.theblockbeats.info</link>
    </image>
    <item>
        <title>数据：巨鲸地址将超1.9万枚ETH转入Coinbase，约3500万美元</title>
        <description><![CDATA[ BlockBeats 消息，5 月 11 日，据 Etherscan 数据显示，「0xC159」开头匿名地址 6 分钟前将 19,093 枚 ETH 转入链上标记为「Coinbase 10」的地址，约合 3500 万美元。 ]]></description>
        <author>contact@theblockbeats.org (律动BlockBeats)</author>
        <link>https://m.theblockbeats.info/flash/137547</link>
        <pubDate>Thu, 11 May 2023 15:02:29 +0800</pubDate>
        <guid>https://m.theblockbeats.info/flash/137547</guid>
    </item>
  </channel>
</rss>

