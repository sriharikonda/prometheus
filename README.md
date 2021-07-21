# prometheus installation steps

set hostname
```
#  sudo su
#  set-hostname Prometheus
```
Download Prometheus
```
#  apt update
#  cd /opt
#  curl -L -O https://github.com/prometheus/prometheus/releases/download/v2.28.0-rc.0/prometheus-2.28.0-rc.0.linux-amd64.tar.gz
#  tar -xf prometheus-2.28.0-rc.0.linux-amd64.tar.gz
#  rm -rf prometheus-2.28.0-rc.0.linux-amd64.tar.gz
#  mv prometheus-2.28.0-rc.0.linux-amd64/ prometheus
#  cd prometheus/
```
setup with systemd file
```
#  vim /etc/systemd/system/prometheus.service
#  systemctl enable prometheus
#  systemctl start prometheus
#  systemctl status prometheus
```
