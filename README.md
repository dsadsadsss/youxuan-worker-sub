## 利用cf-worker部署优选订阅服务器

## 作用:把vless，vmess等可以套CF的节点，一个变成多个节点。

通过抓取api优选ip获取大量ip批量生成多个节点

想要效果更好，可以本地测速再把优质ip上传GitHub存储文本作为api使用即可

## 使用方法:

1. 必须设置变量SUB添加节点链接，节点名称设需为Country-名称，优选ip需设置为ip.sb. 多条链接分号;隔开，不建议太多，1到3条即可变成几十个


2. 可选设置变量API为优选ip地址，分号;隔开.不设置则使用代码内置的
      
3. 订阅地址格式(仅支持v2格式，其他自行转换):
```
精简格式： cf域名/token=111?cf_port=443

(把111换成你实际设置的token,443可以换成cf通用端口如2053，8443)
```
```
完整格式: 域名/token=值?cf_port=值&url=API地址&sub=订阅链接
参数说明：
  - url: 自定义优选IP的API地址，多个用分号(;)隔开
  - sub: 自定义订阅链接，多个用分号(;)隔开
```
3.SUB变量填的节点链接示例，仿照着设置即可:
```
vless://5ca1ad-861c-47f-abd-a569278518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp1;vless://9ca1ad-05861c-47f-abd-fc692216518f8@ip.sb:443?mode=stream-one&path=%2Fxhttp%2F&security=tls&alpn=h2&encryption=none&host=xhttp.nez.com&fp=chrome&type=xhttp&sni=xhttp.nez.com#Country-cf_xhttp2
```
vless是明文可以直接修改，vmess节点可用在v2rayn软件填好配置再复制链接即可.
