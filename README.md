# mini_os_lab(all tools are legal free software or opensource software)

# Setup lab environment
## VMware workstation pro 17, free licence since 2025
## Debian12, LXQT(Light X11 QT) as GUI
## Clion, free licence for non-commercial, educational purpose

## bochs2.7 for assembly
sudo apt-get install libx11-dev libc6-dev build-essential xorg-dev libgtk2.0-dev libreadline-dev     
wget https://sourceforge.net/projects/bochs/files/bochs/2.7/bochs-2.7.tar.gz     
tar -xvzf bochs-2.7.tar.gz    
cd bochs-2.7     
./configure --with-x11 --with-x --enable-all-optimizations --enable-readline  --enable-debugger-gui --enable-x86-debugger --enable-a20-pin --enable-fast-function-calls --enable-debugger    
make -j$(nproc)    
sudo make install    



## qemu for c
sudo apt install qemu-system-x86 qemu-utils     
## clion    
wget https://download.jetbrains.com/cpp/CLion-2025.2.tar.gz     
tar -xvzf CLion-2025.2.tar.gz
sudo mv clion-2025.2 /opt/clion      
/opt/clion/bin/clion.sh (start app)     


## code for OS
http://git.neihedaren.com:8443/ziyaos/ziya-os-research.git   


