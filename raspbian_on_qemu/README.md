# raspbian on qemu
Docker image for raspberry pi virtual environment for development

# Usage
Build docker image and run
```sh
$ docker build -t karaage0703/raspbian_on_qemu .
$ docker run -p 5901:5901 -it --rm --name raspbian_on_qemu karaage0703/raspbian_on_qemu
```

Connect via VNC

Execute following commands:
```sh
# apt-get install wget
# apt-get install glib2.0
# apt-get install libpixman-1-dev
# apt-get install git
# apt-get install curl
# wget https://download.qemu.org/qemu-4.0.0.tar.xz
# tar xvJf qemu-4.0.0.tar.xz
# cd qemu-4.0.0
# ./configure
# make -j8
# make install
# ldconfig
# qemu-system-arm --version
```

Refer to below link:
https://qiita.com/karaage0703/items/366eb17906a3341f1999


# References
- https://github.com/queeno/docker-ubuntu-desktop
- https://kokensha.xyz/docker/access-headless-docker-linux-desktop-container-via-vnc/