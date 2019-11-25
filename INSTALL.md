# Installation steps for CentOS 7.7 x86_64 host

__Step-1__: Install build dependencies from yum

```
yum install -y git python2 epel-release
yum install -y \
    gcc yasm \
    cmake3 \
    jansson-devel \
    ck-devel \
    rtl-sdr-devel \
    uhd-devel
```

__Step-2__: Download source from the following github fork repo
```
git clone -b liuqun-centos7 https://github.com/liuqun/tsl-sdr.git
cd tsl-sdr
cmake3 .
make
```

# TODO: Add installation steps for TSL
Download [TSL](https://github.com/pvachon/tsl) from github

```
git clone https://github.com/pvachon/tsl.git
cd tsl
./waf configure && \
./waf build install
```

# TODO: Add installation steps for:
- CentOS 8.0 x86_64 host and aarch64 host
- Other aarch64 embedded target devices
