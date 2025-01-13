# cf-worker节点生成订阅

vless类型的woker节点自动生成多个ip节点订阅

1. 设置变量SUB,填vless协议的worker节点，节点名称设为Country-名称，优选ip设置为ip.sb


2. 订阅链接格式:
```
域名/token=值?cf_port=值
```

SUB变量例子，仿照着设置即可:
```
vless://5ca1ad-861c-47f-abd-a569278518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp1;vless://9ca1ad-05861c-47f-abd-fc692216518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp2
```
