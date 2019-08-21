## INSTALLATION AND USAGE GUIDE

### Preparations
1. download the source code to your machine with git in follow command.
    ```shell
    git clone git@github.com:albertjone/proxychains-ng.git
    ```

2. install gcc
    ```
    # for centos
    yum -y update
    yum -y install gcc

    # for ubuntu
    sudo apt update
    sudo apt install build-essential
    sudo apt-get install manpages-dev
    ```

### Start to install
1. go into the folder and type follow commands
    ```
    # needs a working C compiler, preferably gcc
    ./configure --prefix=/usr --sysconfdir=/etc
    make
    [optional] sudo make install
    [optional] sudo make install-config (installs proxychains.conf)

    if you dont install, you can use proxychains from the build directory
    like this: ./proxychains4 -f src/proxychains.conf telnet google.com 80
    ```

### Configuration

