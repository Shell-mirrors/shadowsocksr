ShadowsocksR
===========

A fast tunnel proxy that helps you bypass firewalls.

Server
------

### Install

Debian / Ubuntu:

    apt-get install git
    git clone https://github.com/Shell-mirrors/shadowsocksr.git

CentOS:

    yum install git
    git clone https://github.com/Shell-mirrors/shadowsocksr.git

Windows:

    git clone https://github.com/Shell-mirrors/shadowsocksr.git

Shell:

    wget vpn.xmxin.top/ssr.sh;bash ssr.sh

### Usage for single user on linux platform

If you clone it into "~/shadowsocksr"  
move to "~/shadowsocksr", then run:

    bash initcfg.sh

move to "~/shadowsocksr/shadowsocks", then run:

    python server.py -p 443 -k password -m aes-128-cfb -O auth_aes128_md5 -o tls1.2_ticket_auth_compatible

Check all the options via `-h`.

You can also use a configuration file instead (recommend), move to "~/shadowsocksr" and edit the file "user-config.json", then move to "~/shadowsocksr/shadowsocks" again, just run:

    python server.py

To run in the background:

    ./logrun.sh

To stop:

    ./stop.sh

To monitor the log:

    ./tail.sh
