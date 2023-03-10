`sudo useradd -M -U prometheus`

`tar -xzvf prometheus-2.40.0-rc.0.linux-amd64.tar.gz`

`sudo mv prometheus-2.40.0-rc.0.linux-amd64 /opt/prometheus`

`sudo chown prometheus:prometheus -R /opt/prometheus`

`sudo chown prometheus:prometheus -R /opt/node_exporter/`

`sudo journalctl -u prometheus.service -f`

`msiexec /i windows_exporter-0.16.0-amd64.msi ENABLED_COLLECTORS="ad,adfs,cache,cpu,cpu_info,cs,container,dfsr,dhcp,dns,fsrmquota,iis,logical_disk,logon,memory,msmq,mssql,netframework_clrexceptions,netframework_clrinterop,netframework_clrjit,netframework_clrloading,netframework_clrlocksandthreads,netframework_clrmemory,netframework_clrremoting,netframework_clrsecurity,net,os,process,remote_fx,service,tcp,time,vmware" TEXTFILE_DIR="C:\custom_metrics" LISTEN_PORT="9115"`

