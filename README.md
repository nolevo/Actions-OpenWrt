# Actions-OpenWrt

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

Build OpenWrt using GitHub Actions

[Read the details in my blog (in Chinese) | 中文教程](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

## Usage

- Click the [Use this template](https://github.com/P3TERX/Actions-OpenWrt/generate) button to create a new repository.
- Generate `.config` files using [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) source code. ( You can change it through environment variables in the workflow file. )
- Push `.config` file to the GitHub repository, and the build starts automatically.Progress can be viewed on the Actions page.
- When the build is complete, click the `Artifacts` button in the upper right corner of the Actions page to download the binaries.

### Tips

It may take a long time to create a `.config` file and build the OpenWrt firmware. Thus, before create repository to build your own firmware, you may check out if others have already built it which meet your needs by simply [search `Actions-Openwrt` in GitHub](https://github.com/search?q=Actions-openwrt).

Add some meta info of your built firmware (such as firmware architecture and installed packages) to your repository introduction, this will save others' time.

## Acknowledgments

- [Microsoft](https://www.microsoft.com)
- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub](https://github.com)
- [GitHub Actions](https://github.com/features/actions)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cisco](https://www.cisco.com/)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)

## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE) © P3TERX



以下内容是本人增加使用说明，方便自己使用
diy-part2.sh可以修改默认IP地址
diy-part1.sh可以增加第三方插件

自己使用中的插件

CONFIG_TARGET_x86=y
CONFIG_TARGET_x86_64=y
CONFIG_TARGET_x86_64_Generic=y
CONFIG_ARIA2_BITTORRENT=y
CONFIG_ARIA2_NOXML=y
CONFIG_ARIA2_OPENSSL=y
CONFIG_ARIA2_WEBSOCKET=y
CONFIG_NGINX_HEADERS_MORE=y
CONFIG_NGINX_HTTP_ACCESS=y
CONFIG_NGINX_HTTP_AUTH_BASIC=y
CONFIG_NGINX_HTTP_AUTOINDEX=y
CONFIG_NGINX_HTTP_BROWSER=y
CONFIG_NGINX_HTTP_CACHE=y
CONFIG_NGINX_HTTP_CHARSET=y
CONFIG_NGINX_HTTP_EMPTY_GIF=y
CONFIG_NGINX_HTTP_FASTCGI=y
CONFIG_NGINX_HTTP_GEO=y
CONFIG_NGINX_HTTP_GZIP=y
CONFIG_NGINX_HTTP_LIMIT_CONN=y
CONFIG_NGINX_HTTP_LIMIT_REQ=y
CONFIG_NGINX_HTTP_MAP=y
CONFIG_NGINX_HTTP_MEMCACHED=y
CONFIG_NGINX_HTTP_PROXY=y
CONFIG_NGINX_HTTP_REFERER=y
CONFIG_NGINX_HTTP_REWRITE=y
CONFIG_NGINX_HTTP_SCGI=y
CONFIG_NGINX_HTTP_SPLIT_CLIENTS=y
CONFIG_NGINX_HTTP_SSI=y
CONFIG_NGINX_HTTP_UPSTREAM_HASH=y
CONFIG_NGINX_HTTP_UPSTREAM_IP_HASH=y
CONFIG_NGINX_HTTP_UPSTREAM_KEEPALIVE=y
CONFIG_NGINX_HTTP_UPSTREAM_LEAST_CONN=y
CONFIG_NGINX_HTTP_USERID=y
CONFIG_NGINX_HTTP_UWSGI=y
CONFIG_NGINX_NAXSI=y
CONFIG_NGINX_PCRE=y
CONFIG_PACKAGE_aria2=y
CONFIG_PACKAGE_ariang=y
CONFIG_PACKAGE_bash=y
CONFIG_PACKAGE_blkid=y
CONFIG_PACKAGE_btrfs-progs=y
CONFIG_PACKAGE_cgroupfs-mount=y
CONFIG_PACKAGE_containerd=y
CONFIG_PACKAGE_coreutils-nohup=y
CONFIG_PACKAGE_curl=y
CONFIG_PACKAGE_dnscrypt-proxy=y
CONFIG_PACKAGE_dnscrypt-proxy-resolvers=y
CONFIG_PACKAGE_docker-ce=y
CONFIG_PACKAGE_iptables-mod-conntrack-extra=y
CONFIG_PACKAGE_iptables-mod-extra=y
CONFIG_PACKAGE_iptables-mod-ipopt=y
CONFIG_PACKAGE_kmod-br-netfilter=y
CONFIG_PACKAGE_kmod-dax=y
CONFIG_PACKAGE_kmod-dm=y
CONFIG_PACKAGE_kmod-ikconfig=y
CONFIG_PACKAGE_kmod-ipt-conntrack-extra=y
CONFIG_PACKAGE_kmod-ipt-extra=y
CONFIG_PACKAGE_kmod-ipt-ipopt=y
CONFIG_PACKAGE_kmod-lib-crc32c=y
CONFIG_PACKAGE_kmod-nf-ipvs=y
CONFIG_PACKAGE_kmod-veth=y
CONFIG_PACKAGE_libattr=y
CONFIG_PACKAGE_libdevmapper=y
CONFIG_PACKAGE_libexif=y
CONFIG_PACKAGE_libflac=y
CONFIG_PACKAGE_libfreetype=y
CONFIG_PACKAGE_libgd=y
CONFIG_PACKAGE_libid3tag=y
CONFIG_PACKAGE_libjpeg=y
CONFIG_PACKAGE_libmount=y
CONFIG_PACKAGE_libnetwork=y
CONFIG_PACKAGE_libogg=y
CONFIG_PACKAGE_libvorbis=y
CONFIG_PACKAGE_luci-app-aria2=y
CONFIG_PACKAGE_luci-app-diskman=y
CONFIG_PACKAGE_luci-app-dnscrypt-proxy=y
CONFIG_PACKAGE_luci-app-docker=y
CONFIG_PACKAGE_luci-app-familycloud=y
CONFIG_PACKAGE_luci-app-fileassistant=y
CONFIG_PACKAGE_luci-app-filebrowser=y
CONFIG_PACKAGE_luci-app-kodexplorer=y
CONFIG_PACKAGE_luci-app-minidlna=y
CONFIG_PACKAGE_luci-app-mwan3=y
CONFIG_PACKAGE_luci-app-mwan3helper=y
CONFIG_PACKAGE_luci-app-netdata=y
CONFIG_PACKAGE_luci-app-nps=y
CONFIG_PACKAGE_luci-app-ntpc=y
# CONFIG_PACKAGE_luci-app-openvpn-server is not set
CONFIG_PACKAGE_luci-app-ttyd=y
CONFIG_PACKAGE_luci-app-verysync=y
CONFIG_PACKAGE_luci-app-vnstat=y
CONFIG_PACKAGE_luci-app-webadmin=y
# CONFIG_PACKAGE_luci-app-xlnetacc is not set
CONFIG_PACKAGE_luci-i18n-aria2-zh-cn=y
CONFIG_PACKAGE_luci-i18n-docker-zh-cn=y
CONFIG_PACKAGE_luci-i18n-filebrowser-zh-cn=y
CONFIG_PACKAGE_luci-i18n-kodexplorer-zh-cn=y
CONFIG_PACKAGE_luci-i18n-minidlna-zh-cn=y
CONFIG_PACKAGE_luci-i18n-mwan3-zh-cn=y
CONFIG_PACKAGE_luci-i18n-mwan3helper-zh-cn=y
CONFIG_PACKAGE_luci-i18n-netdata-zh-cn=y
CONFIG_PACKAGE_luci-i18n-nps-zh-cn=y
CONFIG_PACKAGE_luci-i18n-ntpc-zh-cn=y
CONFIG_PACKAGE_luci-i18n-ttyd-zh-cn=y
CONFIG_PACKAGE_luci-i18n-verysync-zh-cn=y
CONFIG_PACKAGE_luci-i18n-vnstat-zh-cn=y
CONFIG_PACKAGE_luci-i18n-webadmin-zh-cn=y
CONFIG_PACKAGE_luci-lib-httpprotoutils=y
CONFIG_PACKAGE_minidlna=y
CONFIG_PACKAGE_mount-utils=y
CONFIG_PACKAGE_mwan3=y
CONFIG_PACKAGE_netdata=y
CONFIG_PACKAGE_nginx=y
CONFIG_PACKAGE_npc=y
CONFIG_PACKAGE_ntpclient=y
# CONFIG_PACKAGE_openvpn-easy-rsa is not set
# CONFIG_PACKAGE_openvpn-openssl is not set
CONFIG_PACKAGE_parted=y
CONFIG_PACKAGE_php7=y
CONFIG_PACKAGE_php7-fpm=y
CONFIG_PACKAGE_php7-mod-curl=y
CONFIG_PACKAGE_php7-mod-gd=y
CONFIG_PACKAGE_php7-mod-iconv=y
CONFIG_PACKAGE_php7-mod-json=y
CONFIG_PACKAGE_php7-mod-mbstring=y
CONFIG_PACKAGE_php7-mod-opcache=y
CONFIG_PACKAGE_php7-mod-session=y
CONFIG_PACKAGE_php7-mod-zip=y
CONFIG_PACKAGE_runc=y
CONFIG_PACKAGE_smartmontools=y
CONFIG_PACKAGE_tini=y
CONFIG_PACKAGE_ttyd=y
CONFIG_PACKAGE_uclibcxx=y
CONFIG_PACKAGE_verysync=y
CONFIG_PACKAGE_vnstat=y
CONFIG_PACKAGE_vnstati=y
CONFIG_PACKAGE_zoneinfo-asia=y
CONFIG_PHP7_LIBFREETYPE=y
