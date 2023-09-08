## lspage

Using **fincore** checks the list of all files in the **child directories (du)** that store their pages in the cache (ignoring files that don't store their pages in the kernel).

```bash
root@devops-01:~# bash lspage.sh /var/log
PAGE    SIZE    PATH
6.9M    9.4M    /var/log/remote/192.168.3.104/syslog.log
25.6M   32.9M   /var/log/remote/127.0.0.1/syslog.log
4K      6.7K    /var/log/unattended-upgrades/unattended-upgrades.log
33.6M   40M     /var/log/journal/cde6b7d10b0a4fccb7a250d101ea2256/system.journal
4K      147.4K  /var/log/wtmp
32K     29.5K   /var/log/top-metrics.log
1.4M    1.4M    /var/log/metrics/dir-monitor.log
11.8M   11.8M   /var/log/metrics/top-metrics.log
5.9M    5.9M    /var/log/metrics/iostat-metrics.log
20K     174.2K  /var/log/auth.log
8K      176K    /var/log/kern.log
28.7M   37.1M   /var/log/atop/atop_20230908
16K     285.4K  /var/log/lastlog
276K    2.3M    /var/log/icmp-test.log
32.5M   273.5M  /var/log/syslog
```

## ping-network

Checks the availability of each host on the network using with the ping command. Takes the ip-address parameter of the destination network, in case of its absence it takes the first available address of the current network adapter. Waits for all background thread to complete and sorts the output.

```bash
root@devops-01:~# bash ping-network.sh 192.168.3.0
192.168.3.1      true
192.168.3.2      false
192.168.3.3      false
192.168.3.4      false
192.168.3.5      false
192.168.3.6      false
192.168.3.7      false
192.168.3.8      false
192.168.3.9      false
192.168.3.10     false
192.168.3.11     false
192.168.3.12     false
192.168.3.13     false
192.168.3.14     false
192.168.3.15     false
192.168.3.16     false
192.168.3.17     false
192.168.3.18     false
192.168.3.19     true
192.168.3.20     false
192.168.3.21     false
192.168.3.22     false
192.168.3.23     false
192.168.3.24     false
192.168.3.25     false
192.168.3.26     false
192.168.3.27     false
192.168.3.28     false
192.168.3.29     false
192.168.3.30     false
192.168.3.31     false
192.168.3.32     false
192.168.3.33     false
192.168.3.34     false
192.168.3.35     false
192.168.3.36     false
192.168.3.37     false
192.168.3.38     false
192.168.3.39     false
192.168.3.40     false
192.168.3.41     false
192.168.3.42     false
192.168.3.43     false
192.168.3.44     false
192.168.3.45     false
192.168.3.46     false
192.168.3.47     true
192.168.3.48     false
192.168.3.49     false
192.168.3.50     false
192.168.3.51     false
192.168.3.52     false
192.168.3.53     false
192.168.3.54     false
192.168.3.55     false
192.168.3.56     false
192.168.3.57     false
192.168.3.58     false
192.168.3.59     false
192.168.3.60     false
192.168.3.61     false
192.168.3.62     false
192.168.3.63     false
192.168.3.64     true
192.168.3.65     true
192.168.3.66     false
192.168.3.67     true
192.168.3.68     true
192.168.3.69     true
192.168.3.70     false
192.168.3.71     true
192.168.3.72     false
192.168.3.73     false
192.168.3.74     false
192.168.3.75     false
192.168.3.76     false
192.168.3.77     false
192.168.3.78     false
192.168.3.79     false
192.168.3.80     false
192.168.3.81     false
192.168.3.82     false
192.168.3.83     false
192.168.3.84     false
192.168.3.85     false
192.168.3.86     false
192.168.3.87     false
192.168.3.88     false
192.168.3.89     false
192.168.3.90     false
192.168.3.91     false
192.168.3.92     false
192.168.3.93     false
192.168.3.94     false
192.168.3.95     false
192.168.3.96     false
192.168.3.97     false
192.168.3.98     false
192.168.3.99     true
192.168.3.100    true
192.168.3.101    true
192.168.3.102    true
192.168.3.103    true
192.168.3.104    true
192.168.3.105    true
192.168.3.106    true
192.168.3.107    true
192.168.3.108    false
192.168.3.109    false
192.168.3.110    false
192.168.3.111    false
192.168.3.112    false
192.168.3.113    false
192.168.3.114    false
192.168.3.115    false
192.168.3.116    false
192.168.3.117    false
192.168.3.118    false
192.168.3.119    false
192.168.3.120    false
192.168.3.121    false
192.168.3.122    false
192.168.3.123    false
192.168.3.124    false
192.168.3.125    false
192.168.3.126    false
192.168.3.127    false
192.168.3.128    false
192.168.3.129    false
192.168.3.130    false
192.168.3.131    false
192.168.3.132    false
192.168.3.133    false
192.168.3.134    false
192.168.3.135    false
192.168.3.136    false
192.168.3.137    false
192.168.3.138    false
192.168.3.139    false
192.168.3.140    false
192.168.3.141    false
192.168.3.142    false
192.168.3.143    false
192.168.3.144    false
192.168.3.145    false
192.168.3.146    false
192.168.3.147    false
192.168.3.148    false
192.168.3.149    false
192.168.3.150    false
192.168.3.151    false
192.168.3.152    false
192.168.3.153    false
192.168.3.154    false
192.168.3.155    false
192.168.3.156    false
192.168.3.157    false
192.168.3.158    false
192.168.3.159    false
192.168.3.160    false
192.168.3.161    false
192.168.3.162    false
192.168.3.163    false
192.168.3.164    false
192.168.3.165    false
192.168.3.166    false
192.168.3.167    false
192.168.3.168    false
192.168.3.169    false
192.168.3.170    false
192.168.3.171    false
192.168.3.172    false
192.168.3.173    false
192.168.3.174    false
192.168.3.175    false
192.168.3.176    false
192.168.3.177    false
192.168.3.178    false
192.168.3.179    false
192.168.3.180    false
192.168.3.181    false
192.168.3.182    false
192.168.3.183    false
192.168.3.184    false
192.168.3.185    false
192.168.3.186    false
192.168.3.187    false
192.168.3.188    false
192.168.3.189    false
192.168.3.190    false
192.168.3.191    false
192.168.3.192    false
192.168.3.193    false
192.168.3.194    false
192.168.3.195    false
192.168.3.196    false
192.168.3.197    false
192.168.3.198    false
192.168.3.199    false
192.168.3.200    false
192.168.3.201    false
192.168.3.202    false
192.168.3.203    false
192.168.3.204    false
192.168.3.205    false
192.168.3.206    false
192.168.3.207    false
192.168.3.208    false
192.168.3.209    false
192.168.3.210    false
192.168.3.211    false
192.168.3.212    false
192.168.3.213    false
192.168.3.214    false
192.168.3.215    false
192.168.3.216    false
192.168.3.217    false
192.168.3.218    false
192.168.3.219    false
192.168.3.220    false
192.168.3.221    false
192.168.3.222    false
192.168.3.223    false
192.168.3.224    false
192.168.3.225    false
192.168.3.226    false
192.168.3.227    false
192.168.3.228    false
192.168.3.229    false
192.168.3.230    false
192.168.3.231    false
192.168.3.232    false
192.168.3.233    false
192.168.3.234    false
192.168.3.235    false
192.168.3.236    false
192.168.3.237    false
192.168.3.238    false
192.168.3.239    false
192.168.3.240    false
192.168.3.241    false
192.168.3.242    false
192.168.3.243    false
192.168.3.244    false
192.168.3.245    false
192.168.3.246    false
192.168.3.247    false
192.168.3.248    false
192.168.3.249    false
192.168.3.250    false
192.168.3.251    false
192.168.3.252    false
192.168.3.253    false
192.168.3.254    false

Available:       18
Unavailable:     236
```
