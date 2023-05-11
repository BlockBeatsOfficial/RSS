# BlockBeats_RSS

https://api.theblockbeats.news/v1/open-api/home-xml

Making it more convenient for you to access Web3 information through RSS subscriptions . 

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
    <title>律动BlockBeats</title>
    <description>律动BlockBeats</description>
    <link>https://www.theblockbeats.info</link>
    <image>
        <url>https://image.theblockbeats.info/logo_v2.png</url>
        <title>律动BlockBeats</title>
        <link>https://www.theblockbeats.info</link>
    </image>
    <item>
        <title>香港金管局总裁：将严格监管加密货币以免FTX事件重现</title>
        <description><![CDATA[ BlockBeats 消息，5 月 11 日，香港金管局总裁余伟文表示，将会让加密货币公司在香港创建生态系统并发展成数码资产枢纽，但香港对加密货币产业将继续维持严格的监管制度，现在的监管水平已经降低到「合理及可持续的水平」，但仍然不会允许任何类似 FTX 事件在香港再次发生，以免重现去年因 FTX 破产所导致的市场崩盘。 虚拟资产服务提供者（VASP）发牌制度将于今年 6 月起正式生效，并计划允许散户投资者交易比特币和以太坊等主流 Token，以促进香港在人才流失后向数字资产行业发展的重心。 ]]></description>
        <author>contact@theblockbeats.org (律动BlockBeats)</author>
        <link>https://m.theblockbeats.info/flash/137543?t=binance</link>
        <pubDate>Thu, 11 May 2023 14:33:59 +0800</pubDate>
        <guid>https://m.theblockbeats.info/flash/137543?t=binance</guid>
    </item>
  </channel>
</rss>

