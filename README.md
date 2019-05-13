# Usage

SDK](http://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/) workspace:

tar xjf OpenWrt-SDK-15.05-ar71xx-generic_gcc-4.8-linaro_uClibc-0.9.33.2.Linux-x86_64.tar.bz2

sudo apt-get install ccache xsltproc gperf gawk libncurses5-dev libz-dev zlib1g-dev  git ccache

Add the following line to the `feeds.conf.default` file of your [OpenWrt SDK](http://archive.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/) workspace:

```
src-git gocloud https://github.com/vvyoko/openwrt-feeds.git
```

Then run:

```
scripts/feeds update -f gocloud
scripts/feeds install -a -p gocloud
```

Now, you will be able to see all the packages in this repository via `make menuconfig`.

```
./scripts/feeds update -a 
./scripts/feeds install -a
make menuconfig 

Make clean
make -j1 V=s
make package/feeds/gocloud/luci-app-shadowsocksr/compile V=s
```
