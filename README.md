```
curl -L https://files.nicehash.com/nhminer/nhos/nhos-1.2.3/image/nhos-1.2.3.img.gz -o nhos.img.gz
gzip -d nhos.img.gz
dmesg | grep -i "attached"
sudo dd if=./nhos.img of=/dev/sda bs=4M status=progres
sudo fdisk -l /dev/sda
mkdir /mnt/config
sudo mount /dev/sda2 /mnt/config
curl -L https://bit.ly/30sTmZh -o configuration.txt
cat ./configuration.txt
```
