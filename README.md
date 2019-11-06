# Usage

SDK](http://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/) workspace:

```
wget http://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/OpenWrt-SDK-ramips-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2

tar xjf OpenWrt-SDK-ramips-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2
sudo apt-get update
sudo apt-get install -y git-core build-essential libssl-dev libncurses5-dev unzip gawk subversion mercurial ccache g++ libncurses5-dev zlib1g-dev bison flex unzip autoconf gawk make gettext gcc binutils patch bzip2 libz-dev asciidoc subversion sphinxsearch libtool sphinx-common mercurial
```
Add the following line to the `feeds.conf.default` file of your [OpenWrt SDK](http://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/) workspace:

```
src-git gocloud https://github.com/mlpzaq9998/openwrt-feeds.git
```
Then run:
```
scripts/feeds update -f gocloud
scripts/feeds install -a -p gocloud
```
libraries - ibcur  l choose openssl

Now, you will be able to see all the packages in this repository via `make menuconfig`.


```
./scripts/feeds update -a 
./scripts/feeds install -a
make menuconfig 
```

```
Make clean
make -j1 V=s
make package/feeds/gocloud/luci-app-shadowsocksr/compile V=s
```



bash：po2lmo:command not found 
```
cd luci-app-udp2raw/tools/po2lmo
make
sudo make install
```
https://github.com/sensec/luci-app-udp2raw/wiki/%E7%BC%96%E8%AF%91%E6%95%99%E7%A8%8B

