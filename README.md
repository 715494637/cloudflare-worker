## 操作步骤
####  1. [cloudflare](https://dash.cloudflare.com/)注册,可用[临时邮箱](https://www.linshiyouxiang.net/)
####  2. 点击配置Worker(Configure Worker), 点击快速部署
####  3. 将[worker-vless.js](https://github.com/715494637/cloudflare-worker/blob/main/src/worker-vless.js)中的内容复制到worker中
####  4. 改[随机uuid](https://1024tools.com/uuid)(userID)  
####  5. 改加速CDN(proxyIP)
```
cdn.anycast.eu.org
```
####  6. 配置vless节点
无域名（没tls加密，80或者2052端口）
* 进去worker.dev加上/uuid就能看到VLESS节点URL和Clash-meta配置。
* v2ray,shadowrocket等客户端要去掉tls加密
* 端口改为80或者2052
* 地址修为[优选ip](https://stock.hostmonit.com/CloudFlareYes)

有域名（有tls加密，443端口)，推荐！
* Custom Domains查看——添加自定义域——填1个二级域名
* 点击自定义域，在二级域名后加/UUID，就能看到VLESS节点URL和Clash-meta配置
* 在v2rayN导入URL，地址栏改为[优选ip](https://stock.hostmonit.com/CloudFlareYes)


Tip: 无法优选ip 可以使用这个（youxuan.jdssl.link）域名在v2ray 填优选ip处填写，把端口改为：80 并把下面的tls关闭。

加速CDN：
> cdn-all.xn--b6gac.eu.org
> 
> cdn.xn--b6gac.eu.org
> 
> cdn-b100.xn--b6gac.eu.org
> 
> edgetunnel.anycast.eu.org
> 
> cdn.anycast.eu.org 

workers win专用ip优选：[下载地址](https://jdssl.top/wp-content/uploads/2023/07/works%E4%B8%93%E7%94%A8ip%E4%BC%98%E9%80%89.zip)

ip优选；https://stock.hostmonit.com/CloudFlareYes

临时邮箱：https://www.linshiyouxiang.net/

部署代码：https://github.com/leilei223/edgetunnel/blob/main/src/worker-vless.js

uuid生成：https://1024tools.com/uuid

免费域名注册：https://www.dynadot.com/register-your-free-link-domain

付费域名注册：www.namesilo.com（付费域名注册和解析点击查看这个视频>>跳转到4分17秒处）

ip查看：https://whatismyipaddress.com/

网络测速：https://www.speedtest.net/result/14952074175

openclash转换订阅网址：https://sub-web.netlify.app/
