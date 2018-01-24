# alipayOpenapiCpp
&lt;非常感谢，原作地址：https://github.com/ArthasModern/AlipayOpenapiCpp>
<br />
+ 支付宝开放平台的C\C++版接入示例代码，包含加签验签\网络请求\参数组装\报文解析等等；<br />

### 移植更改内容如下：<br />
+ 该工程配置为 VS2013<br />
+ 替换为 curl-7.57.0 & openssl-1.1.0g 版本的静态库<br />

### OpenSSL & libcurl 编译
> 下载 ActivePerl、NASM，安装，配置环境变量<br />
> http://www.nasm.us/<br />
> https://www.activestate.com/activeperl/downloads<br />
> 
> 编译OpenSSL:<br />
> 现运行 VC\bin\vcvars32.bat<br />
> $ perl Configure VC-WIN32 --prefix=E:\openssl --openssldir=E:\openssl no-shared<br />
> $ nmake<br />
> $ nmake test<br />
> $ nmake install<br />
> 
> 编译libcurl:<br />
> nmake /f Makefile.vc mode=static VC=12 WITH_SSL=static WITH_DEVEL=E:\openssl<br />
