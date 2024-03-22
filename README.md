<h1 align="center">openwrt-23.05 CURL HTTP/3 prebuilt packages</h1>
<p align="center">
  <img width="200" src="https://camo.githubusercontent.com/dbd28ee76842c78a7114d06a44fb14d70ef6a9892463de18b3602ae14854e5e4/68747470733a2f2f6375726c2e73652f6c6f676f2f6375726c2d6c6f676f2e737667" />
</p>
<p align="center">
  <b>build curl library with quictls + libngtcp2 + libnghttp3</b>
</p>

-----------

## package source

- **curl:** [https://github.com/openwrt/packages](https://github.com/openwrt/packages/tree/openwrt-23.05/net/curl)
- **openssl:** [https://github.com/openwrt/openwrt](https://github.com/openwrt/openwrt/tree/openwrt-23.05/package/libs/openssl)
  
  **quictls patch:** [https://github.com/sbwml/r4s_build_script](https://github.com/sbwml/r4s_build_script/tree/master/openwrt/patch/openssl/quic)
  
- **ngtcp2:** https://github.com/sbwml/package_libs_ngtcp2
- **nghttp3:** https://github.com/sbwml/package_libs_nghttp3

## curl configuration

```py
CONFIG_LIBCURL_COOKIES=y
CONFIG_LIBCURL_FILE=y
CONFIG_LIBCURL_FTP=y
CONFIG_LIBCURL_HTTP=y
CONFIG_LIBCURL_NGHTTP2=y
CONFIG_LIBCURL_NGHTTP3=y
CONFIG_LIBCURL_NGTCP2=y
CONFIG_LIBCURL_NO_SMB="!"
CONFIG_LIBCURL_OPENSSL=y
CONFIG_LIBCURL_PROXY=y
CONFIG_LIBCURL_UNIX_SOCKETS=y
# CONFIG_LIBCURL_CRYPTO_AUTH is not set
# CONFIG_LIBCURL_DICT is not set
# CONFIG_LIBCURL_GNUTLS is not set
# CONFIG_LIBCURL_GOPHER is not set
# CONFIG_LIBCURL_IMAP is not set
# CONFIG_LIBCURL_LDAP is not set
# CONFIG_LIBCURL_LIBCURL_OPTION is not set
# CONFIG_LIBCURL_LIBIDN2 is not set
# CONFIG_LIBCURL_MBEDTLS is not set
# CONFIG_LIBCURL_NOSSL is not set
# CONFIG_LIBCURL_POP3 is not set
# CONFIG_LIBCURL_RTSP is not set
# CONFIG_LIBCURL_SMTP is not set
# CONFIG_LIBCURL_SSH2 is not set
# CONFIG_LIBCURL_TELNET is not set
# CONFIG_LIBCURL_TFTP is not set
# CONFIG_LIBCURL_THREADED_RESOLVER is not set
# CONFIG_LIBCURL_TLS_SRP is not set
# CONFIG_LIBCURL_VERBOSE is not set
# CONFIG_LIBCURL_WOLFSSL is not set
# CONFIG_LIBCURL_ZLIB is not set
# CONFIG_LIBCURL_ZSTD is not set
```
