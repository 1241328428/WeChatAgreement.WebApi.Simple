# 微信mac协议，webapi版本。
 请进入  http://www.keduoduo.online/ 进行注册授权<br/>
1.解压Release
2.打开WeChatServer.exe.config
3.配置授权信息，api端口，和websocket端口，管理员密码等参数
```  
    <add key="AuthKey" value="" />
    <add key="WebApiHost" value="22221" />
    <add key="WebSocketHost" value="22222" />
    <add key="AdminPassword" value="123456" />
```
4.右键管理员运行 WeChatServer.exe
看见  开启服务... 证明服务已经开启
5.在浏览器运行http://localhost:22221/swagger/ 即可查看所有webapi文档。
6.微信登录获取二维码需要参考Test.html 中websocket方式创建websocket链接来获取二维码登录。
7.在微信成功登录以后，即可通过Http post的方式传入uuid来操作微信了



<a target="_blank" href="//shang.qq.com/wpa/qunwpa?idkey=3194af004cbc013eff0a61b99a46ae6f66c2c1f1fc62a9cdf58de1fd2b471058">获取更新信息请加入qq群</a>