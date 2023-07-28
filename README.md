
1. build and install rockchip mpp

```
https://github.com/rockchip-linux/mpp.git
```

2. build ffmpeg with rkmpp

```
git clone https://git.ffmpeg.org/ffmpeg.git

git checkout remotes/origin/release/6.0

sudo apt install libdrm-dev libx264-dev libsdl2-dev
```

```
./configure --enable-rkmpp --enable-version3 --enable-libdrm --enable-libx264 --enable-sdl2 --enable-ffplay \
            --enable-nonfree --enable-gpl --enable-shared \
            --disable-doc --disable-htmlpages --disable-podpages --disable-txtpages --disable-manpages
make
```
