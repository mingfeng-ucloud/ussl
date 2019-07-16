{{indexmenu_n>0}}

# **免费证书验证问题**

**1、客户文件验证，但检测报错**，可让客户重新购买并选择DNS验证

**2、免费验证完，请客户自行监测验证是否匹配**
检测地址：<https://myssl.com/dns_check.html#ssl_verify>

示例：三个不同的域名服务器全部匹配，即为验证通过 ![](/security/ussl/free/dv证书检测示例.png)

**3、检测时，只有一个或两个匹配项**
检测只有一个或两个匹配项时，说明验证正常，客户只需要等待即可，正常24小时内会颁发证书；如超过24小时还未颁发，请直接购买OV/EV类型的证书。
![](/images/faq/只有一个匹配项.png)

**4、TXT验证值和cname冲突**

如果DNS验证中txt记录与cname记录冲突导致无法验证成功，可在原主机记录， 域名前加一级\_dnsauth. 来避免冲突

主机记录值参考https://docs.ucloud.cn/security/ussl/operate/fill填写

示例如下：

![](/images/free/域名存在cname.png)

![](/images/free/dnsauth.png)