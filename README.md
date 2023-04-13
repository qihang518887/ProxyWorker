# ProxyWorker
基于CloudFlare Worker的网站代理。
此Worker基于某大佬的基于CloudFlare worker的反代服务，由于反代OneDrive时可能会被报告Phish，故进行修改。

## 如何使用

1. 克隆此项目。
2. 在Cloudflare Workers面板中创建一个新的Worker，并将您的GitHub链接复制到“从GitHub导入”字段中。
3. 在代码中的第一行替换`xxx.sharepoint.com`为您的OneDrive网址。
4. 如果需要，调整`allowed_paths`以允许您的预期路径。
### 或
复制worker.js中的代码到你的Worker。


## 代码说明

该代码包含以下功能：

- 可配置的反代域名
- 阻止特定区域和IP地址访问
- 允许特定路径访问
- 支持HTTPS协议
- 禁用缓存
- 自定义响应文本中的字符串

## Stargazers over time

[![Stargazers over time](https://starchart.cc/Fangsongs/ProxyWorker.svg)](https://starchart.cc/Fangsongs/ProxyWorker)
