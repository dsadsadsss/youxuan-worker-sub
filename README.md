# cf-worker优选节点自动生成多节点订阅器

vless,vmess协议套cf优选的节点一个自动生成多个节点的订阅服务器

1. 设置变量SUB添加节点链接，节点名称设需为Country-名称，优选ip需设置为ip.sb. 多条链接;隔开.支持vless和vmess等所有可以套CDN优选的协议


2. 订阅地址格式:
```
域名/token=111?cf_port=443

(把111换成你设置的token,443可以换成cf通用端口如2053，8443)
```

3.SUB变量填的节点链接示例，仿照着设置即可:
```
vless://5ca1ad-861c-47f-abd-a569278518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp1;vless://9ca1ad-05861c-47f-abd-fc692216518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp2
```
vmess节点可用在v2rayn软件填好设置再复制链接即可
