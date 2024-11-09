# Install Script
```
apt update -y && apt upgrade -y --fix-missing && apt install -y xxd bzip2 wget curl && update-grub && sleep 2 && reboot
```
```
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && \
sysctl -w net.ipv6.conf.default.disable_ipv6=1 && \
apt update && \
apt install -y bzip2 gzip coreutils screen curl unzip && \
wget --no-check-certificate http://sacrifice.web.id/main/setup.sh && \
chmod +x setup.sh && \
sed -i -e 's/$//' setup.sh && \
screen -S setup ./setup.sh

```
