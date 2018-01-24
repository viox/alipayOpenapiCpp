# alipayOpenapiCpp
&lt;非常感谢，原作地址：https://github.com/ArthasModern/AlipayOpenapiCpp>
#支付宝开放平台的C\C++版接入示例代码，包含加签验签\网络请求\参数组装\报文解析等等；

* 该工程配置为 VS2013
* 替换为 curl-7.57.0 & openssl-1.1.0g 版本的静态库



# OpenSSL & libcurl 编译
> 下载 ActivePerl、NASM，安装，配置环境变量
> http://www.nasm.us/
> https://www.activestate.com/activeperl/downloads
> 
> 编译OpenSSL:
> 现运行 VC\bin\vcvars32.bat
> $ perl Configure VC-WIN32 --prefix=E:\openssl --openssldir=E:\openssl no-shared
> $ nmake
> $ nmake test
> $ nmake install
> 
> 编译libcurl:
> nmake /f Makefile.vc mode=static VC=12 WITH_SSL=static WITH_DEVEL=E:\openssl
