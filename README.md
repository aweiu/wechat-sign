# wechat-sign
微信公众平台签名工具。源码来自[微信官方node示例](http://mp.weixin.qq.com/wiki/11/74ad127cc054f6b80759c40f77ec03db.html#.E9.99.84.E5.BD.956-DEMO.E9.A1.B5.E9.9D.A2.E5.92.8C.E7.A4.BA.E4.BE.8B.E4.BB.A3.E7.A0.81)

## 安装
```
npm install wechat-sign
```
## 使用
```
import weChatSign from 'wechat-sign'
weChatSign(jsapiTicket, url)
```
返回：
```
 // something like this
{
  jsapi_ticket: 'jsapi_ticket',
  nonceStr: '82zklqj7ycoywrk',
  timestamp: '1415171822',
  url: 'http://example.com',
  signature: '1316ed92e0827786cfda3ae355f33760c4f70c1f'
}
```
## 其他
首先感谢官方提供的示例！<br>
不知道为什么官方没有发布这个包，微信项目多了每次都手动复制好麻烦，这里厚着脸皮将源码原封不动地传到npm里，如果有人发现了官方或原作者包，烦请告知在下。<br>
目前仅支持微信jsApi签名，后期会考虑加入微信支付签名的功能，所以包名没有使用原名"wechat_jsapi_sign"
