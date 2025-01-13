# cf-worker-sub

woker节点自动生成多个ip订阅，支持vless类型节点

1.//设置变量SUB,填worker节点，节点类型vless,节点名称设为Country-名称，优选ip必须设置为ip.sb


2.//订阅链接格式:

域名/token=值?cf_port=值

SUB变量例子:

vless://5ca1ad-861c-47f-abd-a569278518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-xhttp
