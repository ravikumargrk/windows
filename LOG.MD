# windows
## History:
### 20241124 
Project start, POC @ [aih.com](https://www.aih.app/2023/02/04/run-windows-10-for-free-in-github-codespaces-using-qemu/)

```
sudo apt update && sudo apt upgrade -y
``` 

```
sudo apt install -y qemu-kvm libvirt-daemon
``` 

```
curl https://gist.githubusercontent.com/shawnli87/d416b7c9030293cabfcf4c225cdc5a15/raw/2c85c8233abba10c94d5a2b70e7ea725011b7019/download_gofile.sh -o gofile.sh
``` 

```
chmod +x gofile.sh
``` 

```
./gofile.sh https://gofile.io/d/jJ4xfh
``` 

```
qemu-system-x86_64 -m 4G -cpu max -smp 4 -usbdevice tablet -drive file=w10.qcow2 -display vnc=:1 -vga vmware &
``` 

```
curl https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-v3-stable-linux-amd64.tgz | tar -xz
``` 

```
./ngrok --authtoken <token> tcp 5901
```
