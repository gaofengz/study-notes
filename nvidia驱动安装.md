## 安装nvidia驱动
```
sudo apt-get install nvidia-384
```
## 禁用默认的驱动
```
sudo tee -a /etc/modprobe.d/blacklist-nouveau.conf << EOF

blacklist nouveau

options nouveau modeset=0

EOF

sudo update-initramfs -u
```
## 查看是否禁用命令（重启生效）
```
lsmod | grep nouveau
```

```
sudo apt-get install mesa-common-dev

sudo apt-get install freeglut3-dev

sudo reboot
```
## 安装完成

## 安装cuda

```
cd ~/Downloads

wget -c http://ftp.shu.aixinwu.org/linuxsoftware/cuda_9.0.run

sudo sh cuda_9.0.run --override

sudo tee -a ~/.bash << EOF

export PATH=/usr/local/cuda/bin:$PATH

export LD_LIBRARY_PATH=/usr/local/cuda/lib64$LD_LIBRARY_PATH

EOF

source ~/.bash
```